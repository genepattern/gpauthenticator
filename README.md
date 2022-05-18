# gpauthenticator

**gpauthenticator** is an Authenticator plugin for JupyterHub. It allows users to log into the hub using their 
GenePattern credentials.

An example of how to configure this is below:

```python
# Set gpauthenticator as the authentication mechanism for the hub
c.JupyterHub.authenticator_class = 'gpauthenticator.GenePatternAuthenticator'

# If set, the authenticator will create a blank directory for the user here
c.GenePatternAuthenticator.users_dir_path = '/data/users'   

# If set, users get the files in this directory by default
c.GenePatternAuthenticator.default_nb_dir = '/data/default'  
```
