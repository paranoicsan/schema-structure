# Section 

**Belongs to:** [Lesson](./lesson.md)  
**Type:** [CreativeWork](http://schema.org/CreativeWork)  
**Contains:**
- [Activites](./activity.md)
  
**Math:** ActivityMetadataSectionTag  
**ELA:** GroupTag

### Properties:

|name|type|description|
|----|----|-----------|
|name|[Text](http://schema.org/Text)|linked to title field|
|timeRequired|Duration|linked to time field. **TODO**: need to transform the time to [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)|

### Custom properties:

|name|type|description|
|----|----|-----------|
|sectionCcssStrand|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.\org/AlignmentObject)'s targetName contains the data|
|sectionCcssSubstrand|[AlignmentObject](http://schema.org/AlignmentObject)|[AlignmentObject](http://schema.\org/AlignmentObject)'s targetName contains the data|
|groupSize|[Text](http://schema.org/Text)|linked to group_size field|
|sectionMaterials|[ItemList](http://schema.org/ItemList)|[values](#materials)|
|sectionStandards|[ItemList](http://schema.org/ItemList)|[values](#standards)|
|type|[Text](http://schema.org/Text)|value: _MathSection_ or _ELAGroup_|

#### sectionMaterials<a name="materials"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetName|[Text](http://schema.org/Text)|linked to material name|

#### sectionStandards<a name="standards"></a>

Type: [ItemList](http://schema.org/ItemList)

Contains multiple properties _itemListElement_ of type [AlignmentObject](http://schema.org/AlignmentObject) with
properties:

|name|type|description|
|----|----|-----------|
|targetDescription|[Text](http://schema.org/Text)|linked to standard description|
|targetName|[Text](http://schema.org/Text)|linked to standard name|


### Example

MATH:

```html
<div itemscope="" itemtype="http://schema.org/CreativeWork">
  <meta itemprop="type" content="MathSection">
  <h2>
    <div itemprop="name">Opening</div>
    <div itemprop="timeRequired"> 5 mins</div>
  </h2>
  <ul itemprop="sectionMaterials" itemscope="" itemtype="http://schema.org/ItemList">
    <meta itemprop="name" content="Materials">
    <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
      <span itemprop="name">Pencil</span>
    </li>
    <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
      <span itemprop="name">map and globe</span>
    </li>
  </ul>
  <div itemprop="activities" itemscope="" itemtype="http://schema.org/ItemList">
    <meta itemprop="name" content="activities">
    <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
      <meta itemprop="activityIsFoundational" content="false">
      <meta itemprop="activityIsOptional" content="false">
      <div itemprop="learningResourceType">Fluency Practice</div>
      <div>
        <span itemprop="name">Skip-Count by Tens: Up and Down Crossing 100</span>
        <div>
          <meta itemprop="activityPriorityValue" content="2">
          <span>1</span>
        </div>
        <span itemprop="activityPriorityDescription">This is a Priority 2 activity that can be skipped...</span>
      </div>
      <div itemprop="timeRequired"> 2 mins</div>
      <div>
         <span itemprop="activityMetacognition">In this Fluency Activity, students count by 10 to get them thinking about units of 10.</span>
      </div>
      <div>
         <span itemprop="activityGuidance">While this is a good activator for the Concept Development...</span>
      </div>
      <ul itemprop="sectionStandards" itemscope="" itemtype="http://schema.org/ItemList">
        <meta itemprop="name" content="Standards">
        <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/AlignmentObject">
          <span itemprop="targetNamet">4.NBT.A.2</span>
          <span itemprop="targetDescription">Read and write multi-digit whole numbers using...</span>
      </li>
      </ul>
    </div>
    <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
      <meta itemprop="activityIsFoundational" content="false">
      <meta itemprop="activityIsOptional" content="false">
      <div id="2-core-l2-unit-form-counting-from-398-to-405">
        <div>
          <div itemprop="learningResourceType"> Fluency Practice</div>
          <span itemprop="name">Unit Form Counting from 398 to 405</span>
          <meta itemprop="activityPriorityValue" content="1">
          <span itemprop="activityPriorityDescription"> This is a Priority 1 activity that ...</span>
          <div itemprop="timeRequired"> 3 mins</div>
          <div>
            <span itemprop="activityMetacognition">In this preparatory Fluency Activity, students...</span>
          </div>
          <ul itemprop="activityStandards" itemscope="" itemtype="http://schema.org/ItemList">
            <meta itemprop="name" content="Standards">
            <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem"><span itemprop="name">2.NBT.A.3</span>
              <span itemprop="description">Read and write numbers to 1000 using base-ten numerals, number names, and expanded form.</span>
            </li>
            <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem"><span
              itemprop="name">MP.6</span> <span itemprop="description">Attend to precision.</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
```

ELA:

```html
<div itemscope="" itemtype="http://schema.org/CreativeWork">
   <meta itemprop="type" content="ELAGroup">
   <meta itemprop="groupGroupSize" content="12">
   <div itemprop="groupCcssStrand" itemscope="" itemtype="http://schema.org/AlignmentObject">
      <meta itemprop="targetName" content="Strand here">
   </div>
   <div itemprop="groupCcssSubstrand" itemscope="" itemtype="http://schema.org/AlignmentObject">
      <meta itemprop="targetName" content="Substrand here">
   </div>
   <ul itemprop="groupStandards" itemscope="" itemtype="http://schema.org/ItemList">
      <meta itemprop="name" content="Standards">
      <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/AlignmentObject">
         <span itemprop="targetName">ELA.RL.2.2</span>
         <span itemprop="targetDescription">Recount stories, including fables and folktales from diverse cultures, and determine their central message, lesson, or moral.</span>
      </li>
   </ul>
   <ul itemprop="groupMaterials" itemscope="" itemtype="http://schema.org/ItemList">
      <meta itemprop="name" content="Materials">
      <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
         <span itemprop="name">world map or globe</span>
      </li>
   </ul>
   <div itemprop="name">Introducing the Read-Aloud</div>
   <div itemprop="timeRequired"> 10 mins</div>
   <div itemprop="activities" itemscope="" itemtype="http://schema.org/ItemList">
      <meta itemprop="name" content="Activities">
      <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
         <meta itemprop="activityIsOptional" content="false">
         <meta itemprop="activityGroupSize" content="Whole">
         <meta itemprop="activityCcssStrand" content="">
         <meta itemprop="activityCcssSubstrand" content="">
         <ul itemprop="activityStandards" itemscope="" itemtype="http://schema.org/ItemList">
            <meta itemprop="name" content="Standards">
            <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
               <span itemprop="name">RL.2.5</span>
               <span itemprop="description">Describe the overall structure of a story, including describing how the beginning introduces the story and the ending concludes the action.</span>
            </li>
         </ul>
         <div>
            <h3>
               <div><span itemprop="name">Domain Introduction</span></div>
               <div itemprop="timeRequired"> 3 mins</div>
            </h3>
            <div itemprop="activityMetacognition"> Discuss fairy tales that...</div>
         </div>
      </div>
      <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
         <meta itemprop="activityIsOptional" content="false">
         <meta itemprop="activityGroupSize" content="Whole">
         <meta itemprop="activityCcssStrand" content="">
         <meta itemprop="activityCcssSubstrand" content="">
         <ul itemprop="activityMaterials" itemscope="" itemtype="http://schema.org/ItemList">
            <meta itemprop="name" content="Materials">
            <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
               <span itemprop="name">world map or globe</span>
            </li>
         </ul>
         <ul itemprop="activityStandards" itemscope="" itemtype="http://schema.org/ItemList">
            <meta itemprop="name" content="Standards">
            <li itemprop="itemListElement" itemscope="" itemtype="http://schema.org/ListItem">
               <span itemprop="name">L.2.6</span>
               <span itemprop="description">Produce complete sentences when appropriate to task and situation in order to provide requested detail or clarification.</span>
            </li>
         </ul>
         <div>
            <div>
               <span itemprop="name">Essential Background Information or Terms</span>
            </div>
            <div itemprop="timeRequired"> 5 mins</div>
            <div itemprop="activityMetacognition"> Enchanted characters are...</div>
         </div>
      </div>
      <div itemprop="itemListElement" itemscope="" itemtype="http://schema.org/CreativeWork">
         <meta itemprop="activityIsOptional" content="false">
         <meta itemprop="activityGroupSize" content="Whole">
         <meta itemprop="activityCcssStrand" content="">
         <meta itemprop="activityCcssSubstrand" content="">
         <div>
            <div><span itemprop="name">Purpose for Listening</span></div>
            <div itemprop="timeRequired"> 2 mins</div>
            <div itemprop="activityMetacognition"> Set a purpose for listening to...</div>
         </div>
      </div>
   </div>
</div>
```
