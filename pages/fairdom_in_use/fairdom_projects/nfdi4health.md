---
title: NFDI4Health
description: The main local component and connector of the federated distributed services of NFDI4Health, Germany.
toc: false
page_img: fairdom_in_use/nfdi4health-logo.svg
type: project
---

## The Local Data Hubs (LDH)

The Local Data Hub (LDH) is the main local component and connector of the federated distributed services of NFDI4Health (see [Meineke F., Golebiewski M., Hu X. et al.](https://doi.org/10.3233/SHTI240845)). It enables local (meta-)data structuring, bundling, and sharing within Data Holding Organizations (DHOs) and beyond. Its software operationalizes NFDI4Health standards, including a tailored metadata schema (MDS) for health studies, facilitating communication with the German Central Health Study Hub. Integration into DHO processes and workflows is imperative. These LDHs target (bio)medicine, epidemiology, biostatistics, modelling, and bio- and medical informatics researchers, providing standardized platforms for collaborative sharing of various data elements such as projects, studies, publications, and software tools.

Adhering to the fundamental FAIR principles (Findable, Accessible, Interoperable, Reusable), the LDH ensures that stored information is easily discoverable, accessible to authorized users, interoperable across various systems, and available for reuse in subsequent research endeavours. 


{% include image.html file="fairdom_in_use/nfdi4health1.png" alt="NFDI4Health system" click=true class='screenshot' caption="The NFDI4Health system features Local Data Hubs (LDH), built with FAIRDOM-SEEK." %}

The Local Data Hub within the NFDI4Health ecosystem offers a comprehensive suite of features to enhance research collaboration and data management. It systematically organizes information related to local research, ensuring easy navigation and accessibility. The hub creates meaningful links between domain-specific metadata and data from local studies, facilitating a cohesive research environment. With fine-grained access rights management, it allows precise control over data access. The Local Data Hub supports programmatic access (API), promoting interoperability and data exchange with analytical tools like DataSHIELD or Personal Health Train. Additionally, it facilitates the sharing of public metadata by submitting data to the German Health Study Hub, another core service of NFDI4Health.

Due to its inherent FAIR principles, FAIRDOM-SEEK emerged as the chosen platform for the Local Data Hub (LDH) in the NFDI4Health project for various compelling reasons. The platform's well-established user community, spanning diverse life sciences research areas. FAIRDOM-SEEK’s out-of-the-box compatibility with NFDI4Health's requirements simplifies implementation, ensuring a smooth and efficient integration process. The decision is reinforced by a proven track record in data management, as evidenced by the success of projects such as the "Leipzig Health Atlas," FAIRDOMHub, and LiSyM SEEK. Furthermore, the development expertise at HITS, including their role in co-founding the FAIRDOM initiative, underscores a deep understanding of FAIRDOM-SEEK's capabilities, thereby enhancing its effective utilization for the LDH. The LDH software platform has already been implemented at 3 different DHOs in Germany, including one clinical study centre, which demonstrates the usefulness of our development for users.


## Extended metadata feature

In response to the intricate nature of Metadata Schemas (MDS), FAIRDOM-SEEK incorporates an "extended metadata" feature, allowing flexible user-defined metadata extensions tailored to meet NFDI4Health's specific requirements. This feature also applies across the entire FAIRDOM Community, facilitating the description of complex metadata structures. 

The SEEK-based Local Data Hub now fully represents the comprehensive NFDI4Health metadata schema, thanks to the implementation of this refined extended metadata functionality.

Extended Metadata supports the definition of additional metadata attributes for a particular type, enabling adherence to specific standards (e.g., NFDI4Health MDS). While not directly visible to users, these attributes are associated with a particular attribute type, marked as optional or mandatory, and validated against. Extended Metadata works similarly to Samples, sharing code and defining attributes with names linked to a SampleAttributeType.


{% include image.html file="fairdom_in_use/nfdi4health2-crop.png" alt="screenshot of the architecture of Extended Metadata" class="screenshot" caption="Extended Metadata specific to NFDI4Health is integrated into FAIRDOM-SEEK." click=true %}


Extended Metadata types are linked to specific resource types in FAIRDOM-SEEK, including Collection, DataFile, Document, Event, Model, Presentation, SOP, and Project.  

Extended Metadata can only be currently defined directly in the database, typically through a seed file like the [NFDI4Health MDS Extended Metadata Seed](https://github.com/nfdi4health/ldh/blob/main/db/seeds/018_MDS_3_3_Project_gen.seeds.rb).

Future plans include making it easier for administrators to define Extended Metadata through JSON, an Excel template, or a user interface. 

## Define your own extended metadata type

If users are managing their own FAIRDOM-SEEK instance, they possess the flexibility to tailor Extended Metadata types to align with their project's specific needs by employing a seed file to populate the database.

In addition to defining fundamental attribute types such as string, text, date, date-time, integer, real number, and Boolean, FAIRDOM-SEEK offers the capability to establish more sophisticated types like controller vocabularies and controlled vocabulary lists. 

Controlled vocabularies restrict attributes to a predefined set, presented as a single-select dropdown, while controlled vocabulary lists offer more flexibility, allowing users to make multiple selections from a predetermined  value set for a given attribute.

Moreover, users can define Nested Extended Metadata, introducing a hierarchical structure where one Extended Metadata type can reference another. This results in the nesting of these types within a single form. This feature is particularly powerful, providing a means to model complex relationships and dependencies within users' data. It enhances the overall structure and organisation of metadata, making it a valuable tool for handling intricate data scenarios in a seamless manner, such as NFDI4health MDS. 

It is worth mentioning that users can easily access extended metadata through the user interface or the API. The API extends possibilities, enabling interaction with remote platforms like the German Health Study Hub.


{% include image.html file="fairdom_in_use/nfdi4health3.png" alt="Metadata schemas implementation using extended metadata function" class="screenshot" caption="Metadata schemas are implementated using the extended metadata function of FAIRDOM-SEEK." click=true %}


