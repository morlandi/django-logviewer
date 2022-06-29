## Django LogViewer

Allows the viewing and download of specific log files in real time directly from the Django admin interface.

Inspired by [Django LogTailer](https://github.com/fireantology/django-logtailer)

### Installation

1) Install Django LogViewer:

```
pip install django-logviewer
```

2) Add it to your `INSTALLED_APPS`:


```
    INSTALLED_APPS = (
        ...
        'logviewer',
        ...
    )
```

3) Add Django LogViewer's URL patterns:


```
    urlpatterns = [
        ...
        path('logviewer/', include('logviewer.urls', namespace='logviewer')),
        ...
    ]
```

Then visit:

http://127.0.0.1:8000/logviewer/logs
