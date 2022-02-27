**Computational Definition**

This descriptor is intended to reference VRS Gene value objects. In addition to the attributes inherited from its `Value Object Descriptor`_ parent class, the Gene Descriptor has the following attributes:

**Information Model**

Some GeneDescriptor attributes are inherited from :ref:`ValueObjectDescriptor`.

.. list-table::
   :class: clean-wrap
   :header-rows: 1
   :align: left
   :widths: auto
   
   *  - Field
      - Type
      - Limits
      - Description
   *  - id
      - `CURIE <https://raw.githubusercontent.com/ga4gh/vrs/1.2.1/schema/vrs.json#/definitions/CURIE>`_
      - 1..1
      - Descriptor ID; MUST be unique within document.
   *  - type
      - string
      - 1..1
      - MUST be "GeneDescriptor".
   *  - label
      - string
      - 0..1
      - A primary label for the value object.
   *  - description
      - string
      - 0..1
      - A free-text description of the value object.
   *  - xrefs
      - `CURIE <https://raw.githubusercontent.com/ga4gh/vrs/1.2.1/schema/vrs.json#/definitions/CURIE>`_
      - 0..m
      - List of CURIEs representing associated concepts.
   *  - alternate_labels
      - string
      - 0..m
      - List of strings representing alternate labels for the value object.
   *  - extensions
      - :ref:`Extension`
      - 0..m
      - List of resource-specific :ref:`Extensions <Extension>` needed to describe the value object.
   *  - gene_id
      - `CURIE <https://raw.githubusercontent.com/ga4gh/vrs/1.2.1/schema/vrs.json#/definitions/CURIE>`_
      - 0..1
      - This SHOULD be provided if variation_id is omitted.
   *  - gene
      - `Gene <https://raw.githubusercontent.com/ga4gh/vrs/1.2.1/schema/vrs.json#/definitions/Gene>`_
      - 0..1
      - This MUST be provided if gene_id is omitted.
