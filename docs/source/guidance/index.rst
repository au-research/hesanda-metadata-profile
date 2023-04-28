.. _guidance:

Guidance
============

This page contains general guidance about minting DOIs that is not directly relevant to any particular metadata field.

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

Metadata format - XML or JSON
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DataCite metadata can be fully expressed in either XML or JSON formats. There is no advantage to one over the other
beyond the technical requirements of your systems and workflows.

The metadata must conform to both the DataCite metadata standard 4.4 as well as this HeSANDA metadata profile.

`DataCite's Fabrica service can be used to validate metadata <https://support.datacite.org/docs/how-do-i-validate-doi-metadata>`_ against the DataCite metadata schema.