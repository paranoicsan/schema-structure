# Def

**Belongs to:** [Activity](../activity.md)  
**Type:** [ImageObject](http://schema.org/ImageObject)  
**Tag:** DefTag
 
### Properties:

|name|type|description|
|----|----|-----------|
|caption|[Text](http://schema.org/Text)||
|url|[Text](http://schema.org/Text)||

### Custom properties:

|name|type|description|
|----|----|-----------|
|type|[Text](http://schema.org/Text)|value: _Image_|

### Example

```html
<figure itemscope="" itemtype="http://schema.org/ImageObject">
    <meta itemprop="type" content="Image">
    <img itemprop="ur]" src="https://unbounded-uploads-development.s3.amazonaws.com/ela-images/G2/1/1A-2.jpg">
    <figcaption itemprop="caption">Show image 1A-2: Fisherman with a fish on the line</figcaption>
</figure>
```
