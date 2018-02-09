# ActivityMetadataTypeTag (MATH activity)

Type: [CreativeWork](http://schema.org/CreativeWork)
 
### Properties:

|name|type|description|
|----|----|-----------|
|learningResourceType|Text|linked to activity_type field|
|name|Text|linked to title field|
|timeRequired|Duration|linked to time field. **TODO**: need to transform the time to [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)|

### Custom properties:

|name|type|description|
|----|----|-----------|
|activityAlert|[Text](http://schema.org/Text)|linked to grade field|
|activityGuidance|[Text](http://schema.org/Text)|linked to lesson field|
|activityIsFoundational|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.\org/AlignmentObject)'s targetName contains the data|
|activityIsOptional|[LearningObjective](http://oerschema.org/LearningObjective)|[LearningObjective](http://oerschema.org/LearningObjective)'s targetName contains the data|
|activityMaterials|[ItemList](http://schema.org/ItemList)|[values](#materials)|
|activityMetacognition|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.org/AlignmentObject)'s targetName contains the data|
|activityPriorityDescription|[category](http://schema.org/category)||
|activityPriorityValue|[Text](http://schema.org/Text)|linked to teaser field|
|activityStandards|[ItemList](http://schema.org/ItemList)|[values](#standards)|
|learningResourceType|[Text](http://schema.org/Text)|linked to activity_type field|
|type|[Text](http://schema.org/Text)|value: _MathActivity_|

#### activityMaterials<a href="materials"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetName|[Text](http://schema.org/Text)|linked to material name|

#### activityStandards<a href="standards"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetDescription|[Text](http://schema.org/Text)|linked to standard description|
|targetName|[Text](http://schema.org/Text)|linked to standard name|


### Example

```html
<div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
    <meta itemprop="type" content="MathActivity">
    <meta itemprop="activityIsFoundational" content="false">
    <meta itemprop="activityIsOptional" content="false">
    <div itemprop="learningResourceType"> Fluency Practice</div>
    <h3>
        <div>
            <span itemprop="name">Skip-Count by Tens: Up and Down Crossing 100</span>
            <div>
                <meta itemprop="activityPriorityValue" content="2">
                <span></span>
            </div>
            <span itemprop="activityPriorityDescription"> This is a Priority 2 activity that can be skipped if running short on time. It is less tightly connected to the lesson objective. It might be designed as an extension or to ensure maintenance of prior skills. </span>
        </div>
        <div itemprop="timeRequired"> 2 mins</div>
    </h3>
    <div>
        <span itemprop="activityMetacognition">In this Fluency Activity, students count by 10...</span>
    </div>
    <div>
        <span itemprop="activityGuidance">While this is a good activator for the Concept Development....</span>
    </div>
    <ul itemprop="activityMaterials" itemscope="" itemtype="http://schema.org/ItemList">
        <meta itemprop="name" content="Materials">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">MATH-hide-zero-cards-template-teacher</span>
        </li>
    </ul>
    <ul itemprop="activityStandards" itemscope="" itemtype="http://schema.org/ItemList">
        <meta itemprop="name" content="Standards">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/AlignmentObject">
            <span itemprop="targetNamet">4.NBT.A.2</span>
            <span itemprop="targetDescription">Read and write multi-digit whole numbers using...</span>
        </li>
    </ul>
</div>
```
