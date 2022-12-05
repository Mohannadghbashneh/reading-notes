# Django Custom User

## Reading:
#### Django Best Practices: Custom User Model
- Django ships with a built-in User model for authentication.
- However, for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

## django.contrib.auth
#### Fields:
- username
- first_name
- last_name
- email
- password
- groups
- user_permissions

#### Attributes:
- is_authenticated
- is_anonymous



#### AbstractUser vs AbstractBaseUser
- There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing. 

#### Create a Custom User Model
- update django_project/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin

#### Substituting a custom User model
- Some kinds of projects may have authentication requirements for which Django’s built-in User model is not always appropriate. For instance, on some sites it makes more sense to use an email address as your identification token instead of a username.

#### Changing to a custom user model mid-project¶
- Changing AUTH_USER_MODEL after you’ve created database tables is significantly more difficult since it affects foreign keys and many-to-many relationships, for example.
- This change can’t be done automatically and requires manually fixing your schema, moving your data from the old user table, and possibly manually reapplying some migrations.
- Due to limitations of Django’s dynamic dependency feature for swappable models, the model referenced by AUTH_USER_MODEL must be created in the first migration of its app (usually called 0001_initial); otherwise, you’ll have dependency issues.