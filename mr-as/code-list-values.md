# Code list values

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

When an attribute has a code list as its type, verify that the values comply with the definitions and include the values set out in Annex II, III and IV of the Implementing Rule. To pass this test verify that any instance of an attribute:

* takes only values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'none'.
* takes only a value explicitly specified in the INSPIRE code list register or shall take a value that is narrower (i.e. more specific) than those explicitly specified in the application schema when the code list‘s extensibility is 'narrower'.
* takes values explicitly specified in the INSPIRE code list register when the code list‘s extensibility is 'open' or if a value is not one of the values listed in the code list register check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements (This last check is a manual test).


The following checks are performed for every feature in the dataset, for the 'open' codelist:

* Check that all the [classificationMethodUsed](#classificationMethodUsed) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue1). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue1"></a> Pre-defined values for xlink:href attribute of [classificationMethodUsed](#classificationMethodUsed) element are available in the INSPIRE Registry | 
| ---- | 
| ClassificationMethodUsedValue: http://inspire.ec.europa.eu/codelist/ClassificationMethodUsedValue |

* Check that all the [endusePotential](#endusePotential) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue2). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue2"></a> Pre-defined values for xlink:href attribute of [endusePotential](#endusePotential) element are available in the INSPIRE Registry | 
| ---- | 
| EndusePotentialValue: http://inspire.ec.europa.eu/codelist/EndusePotentialValue |

* Check that all the [activityType](#activityTypeEA) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue3). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue3"></a> Pre-defined values for xlink:href attribute of [activityType](#activityTypeEA) element are available in the INSPIRE Registry | 
| ---- | 
| ExplorationActivityTypeValue: http://inspire.ec.europa.eu/codelist/ExplorationActivityTypeValue |

* Check that all the [explorationResult](#explorationResult) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue4). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue4"></a> Pre-defined values for xlink:href attribute of [explorationResult](#explorationResult) element are available in the INSPIRE Registry | 
| ---- | 
| ExplorationResultValue: http://inspire.ec.europa.eu/codelist/ExplorationResultValue |

* Check that all the [status](#status) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue5). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue5"></a> Pre-defined values for xlink:href attribute of [status](#status) element are available in the INSPIRE Registry | 
| ---- | 
| MineStatusValue: http://inspire.ec.europa.eu/codelist/MineStatusValue |

* Check that all the [mineralDepositGroup](#mineralDepositGroup) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue6). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue6"></a> Pre-defined values for xlink:href attribute of [mineralDepositGroup](#mineralDepositGroup) element are available in the INSPIRE Registry | 
| ---- | 
| MineralDepositGroupValue: http://inspire.ec.europa.eu/codelist/MineralDepositGroupValue |

* Check that all the [type](#type) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue7). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue7"></a> Pre-defined values for xlink:href attribute of [type](#type) element are available in the INSPIRE Registry | 
| ---- | 
| MineralOccurrenceTypeValue: http://inspire.ec.europa.eu/codelist/MineralOccurrenceTypeValue |

* Check that all the [activityType](#activityTypeMA) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue8). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue8"></a> Pre-defined values for xlink:href attribute of [activityType](#activityTypeMA) element are available in the INSPIRE Registry | 
| ---- | 
| MiningActivityTypeValue: http://inspire.ec.europa.eu/codelist/MiningActivityTypeValue |

* Check that all the [processingType](#processingType) elements have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue9). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue9"></a> Pre-defined values for xlink:href attribute of [processingType](#processingType) element are available in the INSPIRE Registry | 
| ---- | 
| ProcessingActivityTypeValue: http://inspire.ec.europa.eu/codelist/ProcessingActivityTypeValue |

* Check that all the [category](#categoryRsv) elements, of the Reserve data type, have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue10). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue10"></a> Pre-defined values for xlink:href attribute of [category](#categoryRsv) element are available in the INSPIRE Registry | 
| ---- | 
| ReserveCategoryValue: http://inspire.ec.europa.eu/codelist/ReserveCategoryValue |

* Check that all the [category](#categoryRsc) elements, of the Resource data type,  have a xlink:href attribute pointing to a [pre-defined value](#preDefinedValue11). If the check fails a manual check will be required asking to review the code list definition in order to verify that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule. If the check fails report [reviewCodeListValue](#reviewCodeListValue).

| <a name="preDefinedValue11"></a> Pre-defined values for xlink:href attribute of [category](#categoryRsc) element are available in the INSPIRE Registry | 
| ---- | 
| ResourceCategoryValue: http://inspire.ec.europa.eu/codelist/ResourceCategoryValue |



**Reference(s)**: 

* [TG DS AF](./README.md#ref_TG_DS_MR) 5.3.3
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated + Manual

**Notes**



## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/> | XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. Please note that the URIs of all code list values from the INSPIRE Registry shall be referenced using the http protocol.
reviewCodeListValue <a name="reviewCodeListValue"/> | XML document '{filename}', {featureType} '{gmlid}': The property '{property}' has a value '{value}' that is not one of the pre-defined values in the INSPIRE data specification. The same value is used by {count} other features in the dataset, too. Extensions to the pre-defined values are allowed, but must not overlap with one of the pre-defined values and be consistent with the specification of the property. Please review the definition of the value. Please note that the URIs of all code list values from the INSPIRE Registry shall be referenced using the http protocol.


## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression				|Multiplicity       |Voidable
---------------------------------------------------------- | -------------------------------|-------------------|---------
classificationMethodUsed <a name="classificationMethodUsed"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Endowment/mr-core:classificationMethodUsed/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Reserve/mr-core:classificationMethodUsed/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Resource/mr-core:classificationMethodUsed/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Endowment/mr-core:classificationMethodUsed/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Reserve/mr-core:classificationMethodUsed/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Resource/mr-core:classificationMethodUsed/@xlink:href | 1 | No
endusePotential <a name="endusePotential"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:endusePotential/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:endusePotential/@xlink:href | 1..\* | Yes
activityType (ExplorationActivity FT) <a name="activityTypeEA"></a> | //schema-element(mr-core:ExplorationActivity)/mr-core:activityType/@xlink:href <br>//schema-element(mr-core:MineralOccurrence)/mr-core:explorationHistory/mr-core:ExplorationActivity/mr-core:activityType/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:explorationHistory/mr-core:ExplorationActivity/mr-core:activityType/@xlink:href | 1 | No
explorationResult <a name="explorationResult"></a> | //schema-element(mr-core:ExplorationActivity)/mr-core:explorationResult/@xlink:href <br>//schema-element(mr-core:MineralOccurrence)/mr-core:explorationHistory/mr-core:ExplorationActivity/mr-core:explorationResult/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:explorationHistory/mr-core:ExplorationActivity/mr-core:explorationResult/@xlink:href | 1 | No
status <a name="status"></a> | //schema-element(mr-core:Mine)/mr-core:status/@xlink:href <br>//schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:Mine/mr-core:status/@xlink:href | 1 | No
mineralDepositGroup <a name="mineralDepositGroup"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:classification/mr-core:MineralDepositModel/mr-core:mineralDepositGroup/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:classification/mr-core:MineralDepositModel/mr-core:mineralDepositGroup/@xlink:href | 1..\* | No
type <a name="type"></a> | //schema-element(mr-core:MineralOccurrence)/mr-core:type/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:type/@xlink:href | 1 | No
activityType (MiningActivity FT) <a name="activityTypeMA"></a> | //schema-element(mr-core:MiningActivity)/mr-core:activityType/@xlink:href <br>//schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:Mine/mr-core:relatedActivity/mr-core:MiningActivity/mr-core:activityType/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:MiningActivity/mr-core:activityType/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:resourceExtraction/mr-core:MiningActivity/mr-core:activityType/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:resourceExtraction/mr-core:MiningActivity/mr-core:activityType/@xlink:href | 1 | No
processingType <a name="processingTypeMA"></a> | //schema-element(mr-core:MiningActivity)/mr-core:processingType/@xlink:href <br>//schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:Mine/mr-core:relatedActivity/mr-core:MiningActivity/mr-core:processingType/@xlink:href <br> //schema-element(mr-core:MiningFeatureOccurrence)/mr-core:specification/mr-core:MiningActivity/mr-core:processingType/@xlink:href <br> //schema-element(mr-core:MineralOccurrence)/mr-core:resourceExtraction/mr-core:MiningActivity/mr-core:processingType/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:resourceExtraction/mr-core:MiningActivity/mr-core:processingType/@xlink:href | 1 | No
category (Reserve data type) <a name="categoryRsv"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Reserve/mr-core:category/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Reserve/mr-core:category/@xlink:href | 1 | No
category (Resource data type) <a name="categoryRsc"></a> |  //schema-element(mr-core:MineralOccurrence)/mr-core:oreAmount/mr-core:Resource/mr-core:category/@xlink:href <br> //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence/mr-core:oreAmount/mr-core:Resource/mr-core:category/@xlink:href | 1 | No
