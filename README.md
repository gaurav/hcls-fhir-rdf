# hcls-fhir-rdf
This repo is maintained by the [RDF subgroup of the HL7 ITS group](https://confluence.hl7.org/pages/viewpage.action?pageId=66922543), and is mostly used for tracking FHIR RDF [issues](https://github.com/w3c/hcls-fhir-rdf/issues).

## State of affairs
RDF (Turtle) is one of three official FHIR serialization formats, along with JSON and XML.

The [FHIR publishing process on github](https://github.com/HL7/fhir) generates:
* a ShEx schema for all core FHIR resources,
* a fairly minimal FHIR ontology; and
* RDF serializations for all of the FHIR examples in the FHIR specification.   

HAPI is now used for parsing and generating FHIR RDF in the FHIR publication process.  See [RDFParser](https://github.com/hapifhir/hapi-fhir/blob/master/hapi-fhir-base/src/main/java/ca/uhn/fhir/parser/RDFParser.java)

Code for the ShEx generation can be found in [ShExGenerator.java](https://github.com/hapifhir/org.hl7.fhir.core/blob/master/org.hl7.fhir.r5/src/main/java/org/hl7/fhir/r5/conformance/ShExGenerator.java)

<span color="red">**The RDF and ShEx generation code in this repository is no longer maintained.**</span>

---------

## Directories
Still in use:
* scripts -- Convenience scripts for transforming FHIR RDF data

Obsolete:
* <del>data - the current stable FHIR specification</del>
  * <del>examples -- XML examples from specification</del>
  * <del>site -- FHIR definitions (we use the json format)</del>
  * <del>rdf -- RDF representation of examples</del>
  * <del>definitions.shex -- shex definitions of FHIR content</del>
  * <del>definitions.xml -- XML definitions used in xslt transformation</del>
  * <del>extract.log -- log of build for the data directory</del>
* <del>hcls_fhir_rdf -- python 3 modules for building data directory</del>
* <del>ontology -- early work on modeling FHIR definitions in OWL</del>
* <del>tests -- python unit tests (not a lot at the moment)</del>
* <del>xsl -- XSLT 2.0 transform for converting FHIR instances from XML to RDF</del>

