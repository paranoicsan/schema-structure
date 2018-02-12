# Def

**Belongs to:** [Activity](../activity.md)  
**Type:** [MediaObject](http://schema.org/MediaObject)  
**Tag:** PdTag
 
### Properties:

|name|type|description|
|----|----|-----------|
|name|[Text](http://schema.org/Text)||
|url|[Text](http://schema.org/Text)||

### Custom properties:

|name|type|description|
|----|----|-----------|
|type|[Text](http://schema.org/Text)|value: _Pd_|

### Example

```html
<div itemscope="" itemtype="http://schema.org/MediaObject">
    <meta itemprop="type" content="PD">
    <div>
        <div itemprop="name">professional development</div>      
    </div>
    <a itemprop="url" href="https://unbounded-uploads.s3.amazonaws.com/PD_PDF/QRD_K-5_Vocab.pdf"
       target="_blank"></a>
    <div><p itemprop="headline">Vocabulary: Unbound A quick reference
        guide to vocabulary in complex text for K-5 ELA/Literacy educators</p>
    </div>
</div>
```
