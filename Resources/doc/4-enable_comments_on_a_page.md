Step 4: Enable comments on a page
=================================
The recommended way to include comments on a page is using the reference
javascript provided. The javascript will asynchronously load the comments after
the page load.

> **Note:**
> The implementation javascript provided with FOSCommentBundle relies on jQuery 1.7
> You will need to install this separately and make sure that it is available on the
> page you want to enable comments on.
>
> You are welcome to rewrite the reference implementation using another javascript
> framework.

And the following code at a desired place in the template to load the comments:

```
{% include 'FOSCommentBundle:Thread:async.html.twig' with {'id': 'foo'} %}
```
> **Note:**
> The id of the thread will be encoded in a url like `/../id/../`. If the id
> contains special characters you should url encode it.


That's the basic setup! For additional information and configuration check the ... section and the cookbook.

**Any problem?** Check our [FAQ](99-faq.md).
