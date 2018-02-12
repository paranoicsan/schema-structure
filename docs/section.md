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
|name|Text|linked to title field|
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

MATH activity:
