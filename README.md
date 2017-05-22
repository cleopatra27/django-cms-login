# django-cms-login
A django-cms apphook to aid with user authentication.

### Installing


```
pip install django_login
```

Add "django_login" to your INSTALLED_APPS setting like this:

```
INSTALLED_APPS = [
        ...
        'django_login',
    ]
```

Add "LOGIN_REDIRECT_URL" to your settings:
```
LOGIN_REDIRECT_URL = '/'
```

Import auth-views
```
from django.contrib.auth import views as auth_views

```

Add the follwing to your urlpatterns (after import)
```
url(r'^en/login/$', auth_views.login, {'template_name': 'registration/login.html'}),
url(r'^logout/$', auth_views.logout),
url(r'^', include('django_login.urls')),
```
## Built With

* [Django](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [codepen](http://django-cms.org/) - Template used

## USAGE
1. Create a new page

![fis](https://cloud.githubusercontent.com/assets/18359815/26309035/ff2d5c00-3eea-11e7-84e1-8219abf7b221.png)

2.Add apphook LOGIN to the page

![fif](https://cloud.githubusercontent.com/assets/18359815/26309031/fc34ea5e-3eea-11e7-8c10-218ea02a67b6.jpg)

ENJOY!!

![codepen](https://cloud.githubusercontent.com/assets/18359815/26309025/f737448e-3eea-11e7-89f2-ef4a79a21f58.jpg)
