<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-moderator-required.svg?maxAge=3600)](https://pypi.org/project/django-moderator-required/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-moderator-required.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-moderator-required.py/actions)

### Installation
```bash
$ [sudo] pip install django-moderator-required
```

##### `models.py`
```python
class User(AbstractBaseUser):
    is_moderator = models.BooleanField(default=False)
```

##### `views.py`
```python
from django_moderator_required.views import ModeratorRequiredMixin

class MyView(ModeratorRequiredMixin,...):
    ...
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>