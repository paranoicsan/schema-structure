# Callout

**Belongs to:** [Activity](../activity.md)  
**Type:** [Article](http://schema.org/Article)  
**Tag:** CalloutTag
 
### Properties:

|name|type|description|
|----|----|-----------|
|headline|[Text](http://schema.org/Text)||
|text|[Text](http://schema.org/Text)||

### Custom properties:

|name|type|description|
|----|----|-----------|
|type|[Text](http://schema.org/Text)|value: _Callout_|

### Example

```html
<div itemscope="" itemtype="http://schema.org/Article">
    <meta itemprop="type" content="Callout">
    <h4 itemprop="headline">This is a Callout Header</h4>
    <div itemprop="text">
        <p><span>If students have difficulty responding to questions, reread pertinent...</span></p>
    </div>
</div>
```
