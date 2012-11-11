jQueryAjaxSubmitter
============

This jQuery plugin will allow you to submit forms and links as AJAX requests. If you provide the proper parameters,
you can really send a request from any element. 

Settings parameters allowed:
* success (callback, called after successful response)
* fail (callback, called after failes response)
* successElements (string or array, elements to be updated after success with their respective elements in response)
* failElements (string or array, elements to be updated after fail with failMessage)
* failMessage (string, message to be displayed in failElements after failed request)
* action (string, URL of request - default: for 'a' elements, the 'href' attribute before the querystring; for 'form' elements, the action attribute)
* method (string, 'get' or 'post' - default: for 'a' elements, 'get'; for 'form' elements, the 'method' attribute or 'post' if it is not set)
* params (string, default: for 'a' elements, the querystring of the 'href' attribute'; for 'form' elements, the serialized form data)

You can also set the following data attributes in your HTML element:
* data-successElements
* data-failElements

These can be any valid CSS selectors separated by a space. This will allow you to attach the plugin to multiple
elements while having the update elements be unique without having to write a separate line of JS for each.
