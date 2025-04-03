.. _guidance:

Guidance
============

This page contains general guidance about minting DOIs that is not directly relevant to any particular metadata field.

Datasets that will be available in the future
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If a dataset is not yet available for sharing but will be in the future, we term this ‘under embargo’. These datasets can still be included in the Health Data Australia's catalogue. 

The dataset-availability enhancements to Health Data Australia will be driven by the metadata use recommended by the DataCite Metadata Schema for indicating embargo (the relevant areas persist from version 4.4 though version 4.6). ARDC will not be recommending any additional or different metadata use.

**Is my dataset 'under embargo'?**

A dataset is considered ‘under embargo’ when it is not available to third parties outside of its research study. 

If the intent of the embargo is to prevent third party access permanently, then the dataset is inappropriate for inclusion in Health Data Australia. Only datasets that are currently available or are under a temporary embargo are appropriate for inclusion in Health Data Australia.

**How do I provide datasets that are under embargo to Health Data Australia?**

If your dataset is under embargo, it is important to advise prospective data requesters of the extent and nature of the embargo, as it may affect their decision to submit a data request.

Guidance is provided in DataCite’s Metadata Schema 4.4 on how to include embargoed datasets in the source metadata of the DataCite DOI. From this schema, the following information must be provided to indicate your dataset will be available in the future in HDA:

1. In `DataCite (8.) Date <https://datacite-metadata-schema.readthedocs.io/en/4.6/properties/date/#date>`_ , please include both:

  (a.) The value for “Available” for the associated field DataCite (8.a) dateType.

  (b.) The dates the dataset will be available from, and optionally to.

      (i.) Accepted date formats are “(YYYY, YYYY-MM-DD, YYYYMM-DDThh:mm:ssTZD or any other format as per DataCite guidelines”). 

      (ii.) Use a single date to indicate the date from when a dataset is available. 

      (iii.) If availability is expected to expire, use two dates for availability - the first to indicate the date from when a dataset is available and then a second date to indicate to (until) when the dataset is available.  “Use RKMS-ISO8601 standard for depicting date ranges.”  


1.a. Additional advice on DataCite (8.) Date:

* We encourage providing as specific a date as possible (i.e. to the day).  Where day is not provided, HDA will presume the first day of the month for from date and - where a range is provided - the last day of the month for to date.  Where month is not provided, HDA will presume the first month of the year for from date and - where a range is provided - the last month of the year for to date.  
* You are encouraged to follow all DataCite Metadata Schema advice relevant to embargo datasets.  For example, the use of Date/s of type “Submitted” and or “Accepted”, where relevant.  HDA will display these dates, but no behaviour beyond display will be driven by any metadata other than Date of type “Available”. 

2. In `DataCite 16 Rights <https://datacite-metadata-schema.readthedocs.io/en/4.6/properties/rights/>`_ , provide a free-text explanation as to why the dataset is under embargo, whether pre-embargo sharing might be considered, and under what circumstances. Please see the table below for guidance.

**Strongly recommended**

* In the ANZCTR Data Sharing Statement, include the date that the dataset will be available for sharing as part of your response to the questions “When will data be available (start and end dates)?”. An approximate date (e.g. July 2025) is acceptable.

**Note:** The ARDC acknowledges that DataCite 5 Publication Year is advised to be used to indicate an embargo date in DataCite Schema 4.4. Please be aware that the dataset-availability enhancements to HDA will be is driven by the DataCite 8 Date = dateType “Available” only - not Publication Year. Therefore, this field must be included in order for the enhanced functionality to occur.

**IMPORTANT!** Please check that the future date provided matches for each metadata field, so that the embargo expiration date is consistent.

**Dataset-Availability Enhancement in HDA**

HDA will be enhanced to include the following functionality around dataset availability:

* Datacite Date values will be visible in HDA view, along with their respective type.

* Message displayed to user where request is made for dataset currently under embargo. User will have option to proceed with request, or save.  

* Message displayed to user where request is made for dataset no longer available (available to date has passed).  User will not have the option to proceed with request.  User is encouraged to see DOI landing page for more information.  

DOI state and workflow
~~~~~~~~~~~~~~~~~~~~~~

The "state" of a DOI refers to the stage of the minting workflow it is in

**Draft:** The unique DOI has been reserved but not registered in the DOI system. Draft DOIs can be deleted.
**Registered:** The unique DOI has been registered in the DOI system, but hidden in search results. The DOI can no longer be deleted.
**Findable:** The unique DOI can now be found in searches. It cannot be deleted, but it can be hidden from searches by being reverted back to the Registered state.

DOIs can be freely swapped between Registered and Findable. Once a DOI leaves Draft state, it can never revert to Draft state.

Landing pages
~~~~~~~~~~~~~

A landing page is a human-readable web page that describes the object that you are minting a DOI for. For example, a dataset's
landing page will provide the "who what when where why how" such as who created it, what it covers, when and where it was created,
and so on. DataCite provides `information on best practice for landing pages <https://support.datacite.org/docs/landing-pages>`_.
A landing page should be hosted on your own systems, such as in a data repository or on a website.

For each landing page link, a full stop (.) will need to be included in the url, or www.
For example, the link to the landing page cannot be https://trog.com.au//landingpage .
Instead, it must to be https://www.trog.com.au/landingpage

Metadata format - XML or JSON
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DataCite metadata can be fully expressed in either XML or JSON formats. There is no advantage to one over the other
beyond the technical requirements of your systems and workflows.

The metadata must conform to both the DataCite metadata standard 4.4 as well as this HeSANDA metadata profile.

`DataCite's Fabrica service can be used to validate metadata <https://support.datacite.org/docs/how-do-i-validate-doi-metadata>`_ against the DataCite metadata schema.

What needs to have a DOI?
~~~~~~~~~~~~~~~~~~~~~~~~~

The most important thing in HeSANDA is the Individual Participant Data (IPD) - the DOI created for this artifact is essential for having a dataset appear in the
HeSANDA catalogue.

Other artifacts of the study, such as a data dictionary or study protocol, can also have DOIs minted for them, with fewer required metadata fields than for the IPD:

* Landing page URL
* Creator
* Title
* Publisher
* Publication year
* Resource type general - "Text" for a data dictionary, "Workflow" for a study protocol
