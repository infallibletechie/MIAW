<html>
   <body>
	<script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
				
    				window.addEventListener( "onEmbeddedMessagingConversationClosed", () => {
            
					console.log( "Inside Conversation End" );
					embeddedservice_bootstrap.userVerificationAPI.clearSession( true ).then( () => {
						embeddedservice_bootstrap.utilAPI.removeAllComponents()
					});
					
				} );
	
				embeddedservice_bootstrap.init(
					'00Dau000002ItPt',
					'MIAW',
					'https://infallibletechiemiaworg.my.site.com/ESWMIAW1720544291552',
					{
						scrt2URL: 'https://infallibletechiemiaworg.my.salesforce-scrt.com'
					}
				);
			} catch (err) {
				console.error('Error loading Embedded Messaging: ', err);
			}
		};
	</script>
	<script type='text/javascript' src='https://infallibletechiemiaworg.my.site.com/ESWMIAW1720544291552/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>	
   </body>
</html>
