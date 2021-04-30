# Code lists

**Purpose**: Verify that code lists extensions can be accessed.

**Prerequisites**

**Test method**

* Verify that any code list extensions are publicly accessible via HTTP, i.e. inspect extensible code list values property elements. If a reference (@xlink:href) has a value that does not start with http://inspire.ec.europa.eu/codelist/, verify that a HTTP GET request to the URI retrieves a document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following empty code lists:

* [CommodityCodeValue](#CommodityCodeValue): http://inspire.ec.europa.eu/codelist/CommodityCodeValue
* [ImportanceValue](#ImportanceValue): http://inspire.ec.europa.eu/codelist/ImportanceValue
* [MineralDepositTypeValue](#MineralDepositTypeValue): http://inspire.ec.europa.eu/codelist/MineralDepositTypeValue


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS SU](./README.md#ref_TG_DS_SU) Annex C

**Test type**: Automated

**Notes**


## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression      |Multiplicity   |Voidable
---------------------------------------------------------- | -----------------------|---------------|---------------------------------
CommodityCodeValue <a name="CommodityCodeValue"></a> | //schema-element(mr-core:Commodity)/mr-core:commodity/@xlink:href <br>//schema-element(mr-core:MineralOccurrence)/mr-core:commodityDescription/mr-core:Commodity/mr-core:commodity/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:commodityDescription/mr-core:Commodity/mr-core:commodity | 1 | No
ImportanceValue <a name="ImportanceValue"></a> | //schema-element(mr-core:Commodity)/mr-core:commodityImportance/@xlink:href <br>//schema-element(mr-core:MineralOccurrence)/mr-core:commodityDescription/mr-core:Commodity/mr-core:commodityImportance/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:commodityDescription/mr-core:Commodity/mr-core:commodityImportance  | 1 | Yes
MineralDepositTypeValue <a name="MineralDepositTypeValue"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:classification/mr-core:MineralDepositModel/mr-core:mineralDepositType/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:classification/mr-core:MineralDepositModel/mr-core:mineralDepositType/@xlink:href | 1..\* | Yes