#PHPMyAdmin for Cloudfoundry

This is PHPMyAdmin Web Console for mysql or mariadb, wich can be pushed to Cloudfoundry and the user can administrate his database :). 
You can use this as your dashboard_url, to provide sso see:
https://docs.google.com/document/d/1ojU5lFgVcLf9BCKIO481xdweFAb-Y3Vj1CM6KhmqSis

## Config and push process

1. edit config file config.inc.php
  * Change parameters: $cfg['Servers'][$i]['host'], 
  * $cfg['Servers'][$i]['user']
  * $cfg['Servers'][$i]['password']

2. push app to cf use php buildpack
  * recommended buildpack: https://github.com/iphoting/heroku-buildpack-php-tyler
