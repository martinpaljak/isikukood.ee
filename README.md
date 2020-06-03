# isikukood.ee/38207162722
Simple service that deals with Estonian ID-code, implemented as a simple proxy of eID LDAP.
## JSON

Query certificates in PEM format, wrapped in JSON. Non-valid ID-code results in 404.


    $ curl -s https://isikukood.ee/38207162722/json/pem | jq

## WHOIS

For lazy and nostalgic UNIX folks

    $ whois -h isikukood.ee 38207162722
    $ whois -h isikukood.ee 38207162722/ssh

## SSH

For usage with OpenSSH

    $ curl -s https://isikukood.ee/38207162722/ssh >> ~/.ssh/authorized_keys
    
After what you can access your account with ID-card

    $ ssh -I /usr/lib/opensc-pkcs11.so you@example.com

## Contact
* martin@martinpaljak.net
