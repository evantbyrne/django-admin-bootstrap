Django's admin interface styled with Twitter Bootstrap. [Github page](https://github.com/evantbyrne/django-admin-bootstrap).

![Django Admin Bootstrap](http://i.imgur.com/4WS6b.png)

**Setup:** Configure _MEDIA\_URL_ and _MEDIA\_ROOT_ in _settings.py_. Then add the following to your _urls.py_:

	from django.conf import settings
	from django.conf.urls.static import static

	urlpatterns = patterns('',
	    # ... the rest of your URLconf goes here ...
	) + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)

---
**Credit:** Adapted from: https://github.com/aobo711/bootstrap-django-admin