<html>
   <body>
	<script type='text/javascript'>		
		    window.addEventListener("onEmbeddedMessagingReady", () => {
	               console.log("onEmbeddedMessagingReady emitted");
	            });
		    window.addEventListener("onEmbeddedMessagingWindowMaximized", (e) => {
			console.log("Received the onEmbeddedMessagingWindowMaximized event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingWindowMinimized", (e) => {
			console.log("Received the onEmbeddedMessagingWindowMinimized event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingButtonClicked", (e) => {
			console.log("Received the onEmbeddedMessagingButtonClicked event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingConversationRouted", (e) => {
			console.log("Received the onEmbeddedMessagingConversationRouted event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingConversationStarted", (e) => {
			console.log("Received the onEmbeddedMessagingConversationStarted event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingPreChatLoaded", (e) => {
			console.log("Received the onEmbeddedMessagingPreChatLoaded event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingPreChatSubmitted", (e) => {
			console.log("Received the onEmbeddedMessagingPreChatSubmitted event…" + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingConversationParticipantChanged", (e) => {
			console.log(`Received the onEmbeddedMessagingConversationParticipantChanged event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessageSent", (e) => {
			console.log(`Received the onEmbeddedMessageSent event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingTranscriptRequested", (e) => {
			console.log(`Received the onEmbeddedMessagingTranscriptRequested event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingTranscriptRequestFailed", (e) => {
			console.log(`Received the onEmbeddedMessagingTranscriptRequestFailed event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingTranscriptDownloadSuccessful", (e) => {
			console.log(`Received the onEmbeddedMessagingTranscriptDownloadSuccessful event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessagingConversationClosed", (e) => {
			console.log(`Received the onEmbeddedMessagingConversationClosed event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessageDelivered", (e) => {
			console.log(`Received the onEmbeddedMessageDelivered event…` + JSON.stringify(e.detail));
		    });
		    window.addEventListener("onEmbeddedMessageRead", (e) => {
			console.log(`Received the onEmbeddedMessageRead event…` + JSON.stringify(e.detail));
		    });
		   window.addEventListener("onEmbeddedMessagingLinkClicked", (e) => {
			console.log(`Received the onEmbeddedMessagingLinkClicked event…` + JSON.stringify(e.detail));
		    });
	</script>	   
	<script type='text/javascript'>
  
		function initEmbeddedMessaging() {
			try {
				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
	
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
