# KeyCloak

Pre-requisite: Setup Keycloak server in local
=============================================
First setup local Keycloak server using this post: https://codehumsafar.wordpress.com/2018/09/11/keycloak-local-setup/
The server will be running at https://localhost:8443/

Setup Keycloak client in local
==============================
Download the repository.
Add realm by importing example-realm.json provided in KeyCloak admin console.
Select the "Example" realm in KeyCloak Admin Console.
Go to Identity Providers --> Google --> Update Client Id and Client Secret with yours.
To get Client Id and Client Secret, Check this link: https://www.keycloak.org/docs/2.5/server_admin/topics/identity-broker/social/google.html
Host the application code of repository in IIS at https://localhost:8888/
Now, Browse the application and you will be redirected to Keycloak login page.
You will see a Google button as well for login.
Click that button.
Enter email id and password and hit enter.
Hurray!! Your have just done social login using Google.

References:
===========
https://github.com/keycloak/keycloak/tree/master/examples/js-console
