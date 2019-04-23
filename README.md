# Wagtail Quick Create

### Wagtail Quick Create offers shortcut links to create objects from models specified in your settings file.

A panel is added to the admin home, offering a type:

![Quick Create Panel example](https://i.imgur.com/DjgQB1R.png)

Clicking a create link will offer a parent selection for the new item

![Parent selection example](https://i.imgur.com/TLlJA9P.png)

### Configuration

Install using pip:

```[bash]
pip install wagtail-quick-create
```

After installing the module, add `wagtailquickcreate` to your installed apps in your settings file:

```[python]
INSTALLED_APPS = [
    ...
    'wagtailquickcreate',
]
```

Also add the following to your settings file:

```
WAGTAIL_QUICK_CREATE_PAGE_TYPES = ['news.NewsPage', 'events.EventPage']
WAGTAIL_QUICK_CREATE_IMAGES = True
WAGTAIL_QUICK_CREATE_DOCUMENTS = True
WAGTAIL_QUICK_CREATE_REPLACE_SUMMARY_PANEL = False
```

