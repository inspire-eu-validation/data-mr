# Statistical Units theme-specific requirements

**Purpose**: Verification whether the MappedFeature type specified in Section 4.2.1.10 of Annex III ([IR-ISDSS](./README.md#ref_IR-ISDSS)) is used to describe the geometric properties of MineralOccurrence spatial object type.


**Prerequisites**

**Test method**

Check whether all instances of MineralOccurrence spatial object type use for providing geometric properties the attribute [Shape](#shape) (GM_Object) defined by MappedFeature spatial object type (in Geology Data Specification).


**Reference(s)**: 

* [TG DS_MR](./README.md#ref_TG_DS_MR) Annex A - Part 1 - A.1.8
* [IR-ISDSS](./README.md#ref_IR-ISDSS) Annex IV, Section 20.4

**Test type**: Automatic

**Notes** 

Two different encodings are possible for providing MineralOccurrence spatial object and the related MappedFeature spatial object:

 * MineralOccurrence spatial object and the related MappedFeature spatial object are provided separately: In this case the element "[specification](#specification1)" of the MappedFeature spatial object shall provide the link to the related MineralOccurrence spatial object through the xlink:href atttribute.
 * MineralOccurrence spatial object and the related MappedFeature spatial object are provided embedded: In this case the specific requirement is self verified because the element "[specification](#specification2)" of the MappedFeature spatial object contains the MineralOccurrence spatial object.


## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                   |  XPath expression                 |Multiplicity       |Voidable
------------------------------ | --------------------------------- | ------------------|----------
shape <a name="shape"></a> | //schema-element(ge:MappedFeature)/ge:shape | 1 | No
specification (reference to MineralOccurrence) <a name="specification1"></a> | //schema-element(ge:MappedFeature)/ge:specification/@xlink:href | 1 | No
specification (embedded encoding of MineralOccurrence) <a name="specification2"></a> | //schema-element(ge:MappedFeature)/ge:specification/mr-core:MineralOccurrence | 1 | No
