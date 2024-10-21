<html>
  <style type='text/css'>
    .embeddedServiceHelpButton .helpButton .uiButton {
      background-color: #005290;
      font-family: "Arial", sans-serif;
    }
    .embeddedServiceHelpButton .helpButton .uiButton:focus {
      outline: 1px solid #005290;
    }
  </style>
  <script type='text/javascript'>
    function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DVB000000nrJJ',
				'Kryterion_In_App_Messaging_Web_Chat',
				'https://kryterion--solvd.sandbox.my.site.com/ESWKryterionInAppMessa1717008769777',
				{
					scrt2URL: 'https://kryterion--solvd.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};

    if(!window.embeddedservice_bootstrap) {
      var s = document.createElement('script');
      s.setAttribute('src','https://kryterion--solvd.sandbox.my.site.com/ESWKryterionInAppMessa1717008769777/assets/js/bootstrap.min.js');
      s.onload = function() {
        initEmbeddedMessaging(null);
      };
      document.body.appendChild();
    } else {
      initEmbeddedMessaging('https://service.force.com');
    }
  
  </script>
</html>
