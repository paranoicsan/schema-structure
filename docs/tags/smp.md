# Smp

**Belongs to:** [Activity](../activity.md)  
**Type:** [Conversation](http://schema.org/Conversation)  
**Tag:** SmpTag
 
### Custom properties:

|name|type|description|
|----|----|-----------|
|content|[Text](http://schema.org/Text)|internal content of an object 
|values|[ItemList](http://schema.org/ItemList)|The set of [ListItems](http://schema.org/ListItem)|
|type|[Text](http://schema.org/Text)|value: _Smp_|

### Example

_Smp_ wraps [Dialogue](./dialogue.md):

```html
<div itemscope="" itemtype="http://schema.org/CreativeWork">
    <meta itemprop="type" content="SMP">
    <ul itemprop="values" itemscope="" itemtype="http://schema.org/ItemList">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">MP.6</span>
        </li>
    </ul>
    <div itemprop="content">
        <div itemscope="" itemtype="http://schema.org/Conversation">
            <div itemprop="phrases" itemscope="" itemtype="http://schema.org/ItemList">
                <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
                    <div itemprop="text">
                        <p>
                            <span><strong>Teacher:</strong> Today we’re going to practice unit form counting. This time we’ll include hundreds! The unit form way to say 324 is 3 hundreds 2 tens 4 ones. (Pull the cards apart to show the 300, 20, and 4.) </span>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```
