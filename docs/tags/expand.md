# Expand

**Belongs to:** [Activity](../activity.md)  
**Type:** [Article](http://schema.org/Article)  
**Tag:** ExpandTag
 
### Custom properties:

|name|type|description|
|----|----|-----------|
|additionalContent|[Text](http://schema.org/Text)|initially hidden content|
|content|[Text](http://schema.org/Text)|internal content of an object|
|type|[Text](http://schema.org/Text)|value: _Expand_|

### Example

```html
<div itemscope="" itemtype="http://schema.org/Article">
    <meta itemprop="type" content="Expand">
    <div itemprop="content">
        <p><span style="font-weight:700;">NOTES ON MULTIPLE MEANS OF ENGAGEMENT</span></p>
        <p><span>As often as possible, create opportunities for every student to respond every time. ...</span></p>
    </div>
    <div itemprop="additionalContent">
        Including choral response, partner talk, personal white boards, and individual tools...
    </div>
</div>
```
