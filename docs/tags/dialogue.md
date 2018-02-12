# Dialogue

**Belongs to:** [Activity](../activity.md)  
**Type:** [Conversation](http://schema.org/Conversation)  
**Tag:** DialogueTag
 
### Custom properties:

|name|type|description|
|----|----|-----------|
|phrases|[ItemList](http://schema.org/ItemList)|The set of [ListItems](http://schema.org/ListItem)|
|type|[Text](http://schema.org/Text)|value: _Dialogue_|

### Example

```html
<div itemscope="" itemtype="http://schema.org/Conversation">
    <meta itemprop="type" content="Dialogue">
    <div itemprop="phrases" itemscope="" itemtype="http://schema.org/ItemList">
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>Teacher:</strong> Remind students that fairy tales</span></p></div>
        </div>
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>Student:</strong> Explain that many things that happen</span></p></div>
        </div>
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>T:</strong> Remind students that fairy tales</span></p></div>
        </div>
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>S:</strong> Explain that many things that happen</span></p></div>
        </div>
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>T:</strong> Remind students that fairy tales</span></p></div>
        </div>
        <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <div itemprop="text"><p><span><strong>S:</strong> Explain that many things that happen</span></p></div>
        </div>
    </div>
</div>
```
