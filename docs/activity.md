# Activity

**Belongs to:** [Section](./section.md)  
**Type:** [CreativeWork](http://schema.org/CreativeWork)
**Contains:**
- [Callout](./tags/callout.md)  
- [Core Content Objectives](./tags/core-content-objectives.md)  
- [Def](./tags/def.md)  
- [Dialogue](./tags/dialogue.md)  
- [Expand](./tags/expand.md)
- [Gls](./tags/gls.md)
- Heading tags:   
  - [Et](./tags/et.md)
  - [Sh](./tags/sh.md)
  - [Th](./tags/th.md)
  - [Key](./tags/key.md)  
- [Image](./tags/image.md)  
- [Image Student Worksheet](./tags/image-student-worksheet.md)  
- [Language Arts Objectives](./tags/language-arts-objectives.md)
- Link tags:
  - [Qrd](./tags/qrd.md)
  - [Pos](./tags/pos.md) 
- [Optional Break](./tags/opt-break.md)  
- [Pd](./tags/pd.md)  
- [Smp](./tags/smp.md)
- [Standard](./tags/standard.md)
- [Vocab](./tags/vocab.md)
  
**Math:** ActivityMetadataTypeTag  
**ELA:** SectionTag
 
### Properties:

|name|type|description|
|----|----|-----------|
|learningResourceType|[Text](http://schema.org/Text)|linked to activity_type field|
|name|[Text](http://schema.org/Text)|linked to title field|
|timeRequired|[Duration](http://schema.org/Duration)|linked to time field. **TODO**: need to transform the time to [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)|

### Custom properties:

|name|type|description|
|----|----|-----------|
|activityAlert|[Text](http://schema.org/Text)|linked to grade field|
|activityCcssStrand|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.\org/AlignmentObject)'s targetName contains the data|
|activityCcssSubstrand|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.\org/AlignmentObject)'s targetName contains the data|
|activityGroupSize|[Text](http://schema.org/Text)|linked to group_size field|
|activityGuidance|[Text](http://schema.org/Text)|linked to lesson field|
|activityIsFoundational|[Text](http://schema.org/Text)|linked to is_foundational field|
|activityIsOptional|[Text](http://schema.org/Text)|linked to is_optional field|
|activityMaterials|[ItemList](http://schema.org/ItemList)|[values](#materials)|
|activityMetacognition|[Text](http://schema.org/Text)|linked to metacognition field|
|activityPriorityDescription|[category](http://schema.org/category)|linked to priority_description field|
|activityPriorityValue|[Text](http://schema.org/Text)|linked to teaser field|
|activityStandards|[ItemList](http://schema.org/ItemList)|[values](#standards)|
|learningResourceType|[Text](http://schema.org/Text)|linked to activity_type field|
|type|[Text](http://schema.org/Text)|value: _MathActivity_ or _ELASection_|

#### activityMaterials<a name="materials"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetName|[Text](http://schema.org/Text)|linked to material name|

#### activityStandards<a name="standards"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetDescription|[Text](http://schema.org/Text)|linked to standard description|
|targetName|[Text](http://schema.org/Text)|linked to standard name|


### Example

MATH activity:

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

ELA activity:

```html
<div itemscope="" itemtype="http://schema.org/CreativeWork">
    <meta itemprop="activityIsOptional" content="false">
    <meta itemprop="activityGroupSize" content="Whole, Small">
    <meta itemprop="type" content="ELASection">
    <div itemprop="activityCcssStrand" itemscope="" itemtype="http://schema.org/AlignmentObject">
        <meta itemprop="targetName" content="Strand here">
    </div>
    <div itemprop="activityCcssSubstrand" itemscope="" itemtype="http://schema.org/AlignmentObject">
        <meta itemprop="targetName" content="Substrand here">
    </div>
    <ul itemprop="activityMaterials" itemscope="" itemtype="http://schema.org/ItemList">
        <meta itemprop="name" content="Materials">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">ELA-G2-M1-U1-SW-Story Map</span>
        </li>
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">chart paper</span>
        </li>
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">chalkboard</span>
        </li>
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
            <span itemprop="name">or whiteboard</span>
        </li>
    </ul>
    <ul itemprop="activityStandards" itemscope="" itemtype="http://schema.org/ItemList">
        <meta itemprop="name" content="Standards">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/AlignmentObject">
            <span itemprop="targetNamet">ELA.SL.2.2</span>
            <span itemprop="targetDescription">Recount or describe key ideas or details from a text read...</span>
        </li>
    </ul>
    <hr>
    <div>
        <h3>
            <div>
                <span itemprop="name">Retelling the Read-Aloud</span>
            </div>
            <div itemprop="timeRequired"> 20 mins</div>
        </h3>
        <div itemprop="activityMetacognition"> Conduct an application activity...</div>
    </div>
</div>
```
