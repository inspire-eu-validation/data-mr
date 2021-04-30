# Feature references

**Purpose**: Verify that referenced features can be retrieved.

**Prerequisites**

**Test method**

* Verify that any feature reference in an association role is publicly accessible via HTTP, i.e. inspect all relevant properties. If a reference (@xlink:href) has a value that starts with "#", verify that an element with a `gml:id` attribute with the referenced identifier exists in the same document. If the reference starts with "http", verify that a HTTP GET request to the URI retrieves an XML document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following association role:

* [EarthResource.explorationHistory](#explorationHistory): ExplorationActivity
* [EarthResource.classification](#classification): MineralDepositModel
* [EarthResource.resourceExtraction](#resourceExtraction): MiningActivity
* [EarthResource.commodityDescription](#commodityDescription): Commodity
* [Commodity.source](#source): EarthResource
* [MiningFeatureOccurrence.specification](#specificationMFO): MiningFeature (Mine or MiningActivity)
* [Mine.relatedMine](#relatedMine): Mine
* [Mine.relatedActivity](#relatedActivity): MiningActivity
* [MiningActivity.associatedMine](#associatedMine): Mine
* [MiningActivity.deposit](#deposit): EarthResource
* [CommodityMeasure.commodityOfInterest](#commodityOfInterest): Commodity


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)

**Test type**: Automated

**Notes**

ProfileElement and Mineral ResourcesProfile are abstract.

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                         |  XPath expression    | Multiplicity    | Voidable
------------------------------------ | ---------------------|-----------------|------------
explorationHistory <a name="explorationHistory"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:explorationHistory/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:explorationHistory/@xlink:href | 1..\* | Yes
classification <a name="classification"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:classification/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:classification/@xlink:href | 1 | Yes
resourceExtraction <a name="resourceExtraction"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:resourceExtraction/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:resourceExtraction/@xlink:href | 0..\* | Yes
commodityDescription <a name="commodityDescription"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:commodityDescription/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:commodityDescription/@xlink:href | 1..\* | Yes
source <a name="source"></a> |  //schema-element(mr-core:Commodity)/mr-core:source/@xlink:href | 1 | No
specification <a name="specificationMFO"></a> |  //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/@xlink:href | 1 | No
relatedMine <a name="relatedMine"></a> |  //schema-element(mr-core:Mine)/mr-core:relatedMine/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:Mine/mr-core:relatedMine/@xlink:href | 1..\* | Yes
relatedActivity <a name="relatedActivity"></a> |  //schema-element(mr-core:Mine)/mr-core:relatedActivity/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:Mine/mr-core:relatedActivity/@xlink:href | 1..\* | No
associatedMine <a name="associatedMine"></a> |  //schema-element(mr-core:MiningActivity)/mr-core:associatedMine/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:MiningActivity/mr-core:associatedMine/@xlink:href | 1 | No
deposit <a name="deposit"></a> |  //schema-element(mr-core:MiningActivity)/mr-core:deposit/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:MiningActivity/mr-core:deposit/@xlink:href | 1 | No
commodityOfInterest <a name="commodityOfInterest"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Endowment/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Reserve/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Resource/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Endowment/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Reserve/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Resource/mr-core:measureDetails/mr-core:CommodityMeasure/mr-core:commodityOfInterest/@xlink:href | 1..\* | No