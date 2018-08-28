# KeyCloak Integration

oauthenticator


```bash
$ helm upgrade --install jhub jupyterhub/jupyterhub --version 0.7.0-beta.2 -f jh-config.yml

$ helm upgrade --install --name keycloak --namespace keycloak stable/keycloak -f kc-config.yml
```