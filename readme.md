# AROSS Database Data Dictionary

A repo containing a description of the Arctic Rain on Snow Study rain on snow database

## Unorganized Notes

There does not appear to be a good definition or example of a data dictionary for Earth science data.  Here are some links that I have found.

Most link are business data science

From [Secoda](https://www.secoda.co/learn/data-dictionary-key-terms):

>A data dictionary, an essential tool in data management, typically includes key components such as term names, definitions, data types, allowable values, and the responsible party for the term. It serves as a reference that helps maintain consistency and clarity across different datasets and departments within an organization.

Furthermore, a comprehensive data dictionary might also contain information about the data source, related terms, and any calculations or transformations the data may undergo. This ensures that all stakeholders have a common understanding of the data, which is crucial for accurate analysis and decision-making.

From [atlan](https://atlan.com/what-is-a-data-dictionary/#what-is-a-data-dictionary):

>A data dictionary is a collection of metadata such as object name, data type, size, classification, and relationships with other data assets. Think of it as a list along with a description of tables, fields, and columns. The primary goal of a data dictionary is to help data teams understand data assets.

A more concise definition from atlan is:

>A data dictionary documents technical metadata for a specific database

The atlan document also includes definitions from IBM:

>a data dictionary is a “centralized repository of information about data such as meaning, relationships to other data, origin, usage, and format. It assists management, database administrators, system analysts, and application programmers in planning, controlling, and evaluating the collection, storage, and use of data.”;

and DAMA UK (Data Management Association UK):

>a data dictionary as “software in which metadata is stored, manipulated, and defined.”

The Arctic Data Center has broad requirements of metadata.  Some of which could be included in a data dictionary:

>-Full records of field and laboratory sampling times and locations, including a geographic description interpretable by a general scientific audience.  
>-Full records of taxonomic coverage within the data package (if applicable).
>-Full descriptions of field and laboratory sample collection and processing methods.
>-Full descriptions of any hardware and software used (including make, model, and version, where applicable).
>-Full attribute/variable information for all data.
>-Quality control procedures.

For the AROSS database, a data dictionary could include

- name of field
- definition of field
- data type
- valid range of values used in QC
- minimum and maximum values
- missing value
- source
- processing pipeline


There is also a need for a description of how datasets are linked

