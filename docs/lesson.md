# Lesson

The markup which is placed right before any parsed tag. Contains the data from document-metadata tables.

**Type:** [CreativeWork](http://schema.org/CreativeWork)  
**Contains:**
- [Sections](./section.md)
- Standalone tags
 
### Properties:

|name|type|description|
|----|----|-----------|
|description|[Text](http://schema.org/Text)|linked to description field|
|licence|[Text](http://schema.org/Text)|linked to cc-attribution field|
|name|[Text](http://schema.org/Text)|linked to title field|

### Custom properties:

|name|type|description|
|----|----|-----------|
|grade|[Text](http://schema.org/Text)|linked to grade field|
|lesson|[Text](http://schema.org/Text)|linked to lesson field|
|lessonMathematicalPractice|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.org/AlignmentObject)'s targetName contains the data|
|lessonObjective|[LearningObjective](http://oerschema.org/LearningObjective)|[LearningObjective](http://oerschema.org/LearningObjective)'s targetName contains the data|
|lessonStandard|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.org/AlignmentObject)'s mainContent contains the data|
|standard|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.org/AlignmentObject)'s targetName contains the data|
|subject|[category](http://schema.org/category)||
|teaser|[Text](http://schema.org/Text)|linked to teaser field|
|topic|[Topic](http://oerschema.org/Topic)|[Topic](http://oerschema.org/Topic)'s mainContent contains the data|
|type|[LearningComponent](http://oerschema.org/LearningComponent)|[LearningComponent](http://oerschema.org/LearningComponent)'s mainContent contains the data|
|unit|[Text](http://schema.org/Text)|linked to unit field|

### Example

```html
<div itemscope="" itemtype="http://schema.org/CreativeWork"  data-scroll="ld-page" id="ld-page">
    <span itemprop="subject" itemscope="" itemtype="http://schema.org/category" >math</span>
    <meta itemprop="grade" content="4">
    <meta itemprop="unit" content="1">
    <div itemprop="topic" itemscope="" itemtype="http://oerschema.org/Topic" >
        <meta itemprop="mainContent" content="A">
    </div>
    <meta itemprop="lesson" content="4">
    <div itemprop="type" itemscope="" itemtype="http://oerschema.org/LearningComponent" >
        <meta itemprop="mainContent" content="core">
    </div>
    <div itemprop="lessonObjective" itemscope="" itemtype="http://oerschema.org/LearningObjective" >
        <meta itemprop="mainContent" content="SWBAT name numbers within 1 million by building understanding of the place value chart and placement of commas for naming base thousand units.">
    </div>
    <div itemprop="lessonStandard" itemscope="" itemtype="http://schema.org/AlignmentObject" >
        <meta itemprop="targetName" content="4.NBT.A.2">
    </div>
    <div itemprop="lessonMathematicalPractice" itemscope="" itemtype="http://schema.org/AlignmentObject" >
        <meta itemprop="targetName" content="">
    </div>
    <meta itemprop="name" content="Name numbers within 1 million by building understanding of the place value chart and placement of commas for naming base thousand units.">
    <meta itemprop="description" content="">
    <meta itemprop="license" content="This work is based on an original work of Great Minds and licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License. UnboundEd is not affiliated with the copyright holder of this work.">
</div>
```
