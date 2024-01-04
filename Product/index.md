<html>
  <style>
    /* Basic styling for the chat button */
    .salesforce-chat-button {
        background-color: #0070d2; /* Salesforce blue */
        color: white;
        border: none;
        padding: 10px 20px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        margin: 4px 2px;
        cursor: pointer;
        border-radius: 8px;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
    }
    /* Hover effect */
    .salesforce-chat-button:hover {
        background-color: #005fb8; /* Darker blue */
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.3);
    }
  </style?
  <body>
    <script type='text/javascript'>
    	function initEmbeddedMessaging() {
    		try {
    			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
          window.addEventListener("onEmbeddedMessagingReady", () => {            
          	console.log( "Inside Prechat API!!" );
            const currentUrl = window.location.href;
            console.log('currentUrl = ',currentUrl);
          	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "PageURL" : currentUrl } );
          });
    			embeddedservice_bootstrap.init(
    				'00D0T0000000Nru',
    				'POC_MessagingForWeb_GithubWebTest',
    				'https://scbprotectneworg--newptdev.sandbox.my.site.com/ESWPOCMessagingForWebGi1704338454659',
    				{
    					scrt2URL: 'https://scbprotectneworg--newptdev.sandbox.my.salesforce-scrt.com'
    				}
    			);
    		} catch (err) {
    			console.error('Error loading Embedded Messaging: ', err);
    		}
    	};
  </script>
  <script type='text/javascript' src='https://scbprotectneworg--newptdev.sandbox.my.site.com/ESWPOCMessagingForWebGi1704338454659/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

  </body>
</html>
