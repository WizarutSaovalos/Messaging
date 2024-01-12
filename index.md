<html>
  <head>
    <style type="text/css">
      lightning-button.embedded-messaging-menu-item-option > button.slds-button:hover:after {
          text-decoration: none !important;
      }
    </style>
  </head>
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
