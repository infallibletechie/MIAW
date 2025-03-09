<html>
   <body>
	<script type='text/javascript'>
		function initEmbeddedMessaging() {
			try {
				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
				
    				window.addEventListener( "onEmbeddedMessageSent", ( event ) => {

					console.log( "START:: Message Sent" );
     					console.log( "Event detail: ", JSON.stringify( event.detail ) );
     					
					let tempContent = event.detail;

      					if ( tempContent.conversationEntry.sender.role ) {
	   
						let strRole = tempContent.conversationEntry.sender.role;
      						console.log( 'strRole =>', strRole );

	 					if ( strRole == 'Agent' ) {
	
							if ( tempContent.conversationEntry.entryPayload ) {
							
								tempContent = JSON.parse( tempContent.conversationEntry.entryPayload );
							
								if ( tempContent.abstractMessage.staticContent.text ) {
									
									let strMessage = tempContent.abstractMessage.staticContent.text;
									console.log( strMessage );
									
									if ( strMessage.includes( 'Redirect to Payment Page:' ) ) {
							
										window.open( 'https://www.infallibletechie.com', '_self' );
							
									}
								}
							
							}

      						}

     					}
   
					console.log( "END:: Message Sent" );
				
					
				
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
