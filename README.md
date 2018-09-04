# KeyCloak Integration

oauthenticator


```bash
$ helm upgrade --install jhub jupyterhub/jupyterhub --version 0.7.0-beta.2 -f jh-config.yml

$ helm upgrade --install --name keycloak --namespace keycloak stable/keycloak -f kc-config.yml
```

# Steps
 - Setup `JupyterHub` client within KC
    - Login Theme: keycloak
    - Client Protoco: openid-connect
    - Access Type: confidential
    - Set Valid Redirect URLs:
      - http://a04425a66aa3a11e89952021d923673c-183303353.us-west-2.elb.amazonaws.com/hub/oauth_callback
    - 