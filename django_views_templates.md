## Note: This page is in draft stage

## Django views and templates

A view is a place where we put the "logic" of our application. It will request information from the model and pass it to a template. 

```
from django.conf.urls import include, url
from django.contrib import admin


urlpatterns = [
    url(r'^admin/', admin.site.urls),
    url(r'', include('website.urls')),

]
```

```
from django.conf.urls import url
from . import views

urlpatterns = [
    url(r'^$', views.home, name='home'),
    url(r'^services/$', views.services, name='services'),
]
```
### Template path

```
os.path.join(BASE_DIR, "templates")]
```

### website views

```
from django.http import HttpResponseRedirect, HttpResponse

def home(request):
    return render(request, 'website/index.html')

```