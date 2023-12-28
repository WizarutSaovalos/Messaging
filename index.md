<html>
  <body>
    <script type='text/javascript'>
    	function initEmbeddedMessaging() {
    		try {
    			embeddedservice_bootstrap.settings.language = 'en_US';
    			embeddedservice_bootstrap.init(
    				'00D0T0000000Nru',
    				'POC_MessagingForIn_AppAndWeb',
    				'https://scbprotectneworg--newptdev.sandbox.my.site.com/ESWPOCMessagingForInApp1703145720194',
    				{
    					scrt2URL: 'https://scbprotectneworg--newptdev.sandbox.my.salesforce-scrt.com'
    				}
    			);
    		} catch (err) {
    			console.error('Error loading Embedded Messaging: ', err);
    		}
    	};
    </script>
    <script type='text/javascript' src='https://scbprotectneworg--newptdev.sandbox.my.site.com/ESWPOCMessagingForInApp1703145720194/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>
