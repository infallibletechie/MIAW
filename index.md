<html>
  <body>
    <script type='text/javascript'>
      function initEmbeddedMessaging() {
        try {
          embeddedservice_bootstrap.settings.language = ''; // For example, enter 'en' or 'en-US'
          embeddedservice_bootstrap.init('00D8Z000000sp44', 'MIAW_for_GitHub', 'https://infallibletechiemiaw.my.site.com/ESWMIAWforGitHub1656612431237', {
            scrt2URL: 'https://infallibletechiemiaw.my.salesforce-scrt.com'
          });
        } catch (err) {
          console.error('Error loading Embedded Messaging: ', err);
        }
      };
    </script>
    <script type='text/javascript' src='https://infallibletechiemiaw.my.site.com/ESWMIAWforGitHub1656612431237/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'>
    </script>
  </body>
</html>
