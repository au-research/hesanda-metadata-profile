.. _Intro:

Introduction
============

Document history

======== ========== ==============================
Version  Date       Description
======== ========== ==============================
0.1      28/09/2022 Draft release for consultation
1.0      16/12/2022 First major release
======== ========== ==============================

This document outlines HeSANDA's information requirements and metadata profile. These requirements have been designed such that they can be fulfilled using two pre-existing metadata sources: the Australian New Zealand Clinical Trials Registry (ANZCTR) and DataCite.  

The left-hand side of the table below lists the information categories and attributes required for data discovery and the functionality of HeSANDA's Federation Service. The right-hand side of the table then indicates how each requirement can be fulfilled using metadata sourced from ANZCTR and DataCite. 

Please note: 

#. The metadata profile has been designed such that HeSANDA requires a minimum number of fields beyond what is required by ANZCTR and DataCite. These are: 

    * DataCite 6 Subject (for HeSANDA information requirement 2.3.1) 
    * DataCite 7 Contributor (for HeSANDA information requirement 4.4.2) 
    * DataCite 12 Related Identifier (for HeSANDA information requirement 2.1) 
    * DataCite 17 Description (for HeSANDA information requirement 1.10 and 3.2) 

#. The following HeSANDA information requirements can be fulfilled using both ANZCTR and DataCite metadata:

    * 2.1 Study identifier
    * 2.4 Funding sources
    * 2.7 Study protocol
    * 2.7a Data dictionary
    * 4.1 Permitted uses

ANZCTR metadata is required in all cases. With the exception of requirement 2.1 (Study identifier), DataCite metadata is optional. For further information, refer to the description section in the table below.

#. A DataCite field may have one or more subfields, which may or may not be required. The Occurrences column indicates whether a subfield is required, optional, and even repeatable.

    * 0-1 - Optional but not repeatable
    * 0-n - Optional and repeatable
    * 1 - Required but not repeatable
    * 1-n - Required and repeatable

#. This document refers to Version 4.4 of the DataCite Schema.

#. Each dataset will require a landing page. DataCite provides guidance on best practices for landing pages. Please contact ARDC if you need support implementing these requirements.

Please contact ARDC to discuss any issues fulfilling these requirements via ANZCTR and DataCite. 

Related information:

* The `DataCite support site <https://support.datacite.org/>`_ is an excellent source of information on how to work with DataCite systems.