# API Deployment

## Configuring Django Settings: Best Practices

## Managing Django Settings: Issues

1. Different environments :

 Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

2. Sensitive data :

 You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

3. Sharing settings between team members :
 
  This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.

4. Django settings are a Python code :
 
  This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


## Setting Django Configurations: Different Approaches
 
 There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best. Let’s take a brief look at the most popular ones to examine their weaknesses and strengths.

## Django Settings: Best practices
 
 1. Keep settings in environment variables.
 2. Write default values for production configuration (excluding secret keys and tokens).
 3. Don’t hardcode sensitive settings, and don’t put them in VCS.
 4. Split settings into groups: Django, third-party, project.
 5. Follow naming conventions for custom (project) settings.

# What Is SSH?
 SSH, or Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet.

## main encryption technologies :
 1. Symmetrical Encryption
 2. Asymmetrical Encryption
 3. Hashing

## How Does SSH Work
 SSH works by using the client-server model to allow for authentication between two remote systems and encrypt the data passed between them.