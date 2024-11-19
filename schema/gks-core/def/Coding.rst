.. warning:: This data class is at a **draft** maturity level and may \
    change significantly in future releases. Maturity \
    levels are described in the :ref:`maturity-model`.

**Computational Definition**

A structured representation of a code for a defined concept in a terminology or code system.

**Information Model**

Some Coding attributes are inherited from :ref:`Element`.

.. list-table::
   :class: clean-wrap
   :header-rows: 1
   :align: left
   :widths: auto

   *  - Field
      - Flags
      - Type
      - Limits
      - Description
   *  - id
      - 
      - string
      - 0..1
      - The 'logical' identifier of the data element in the system of record, e.g. a UUID.  This 'id' is unique within a given system, but may or may not be globally unique outside the system. It is used within a system to reference an object from another.
   *  - extensions
      - 
                        .. raw:: html

                            <span style="background-color: #B2DFEE; color: black; padding: 2px 6px; border: 1px solid black; border-radius: 3px; font-weight: bold; display: inline-block; margin-bottom: 5px;" title="Unordered">&#8942;</span>
      - :ref:`Extension`
      - 0..m
      - A list of extensions to the Entity, that allow for capture of information not directly supported by elements defined in the model.
   *  - label
      - 
      - string
      - 0..1
      - The human-readable name for the coded concept, as defined by the code system.
   *  - system
      - 
      - string
      - 1..1
      - The terminology/code system that defined the code. May be reported as a free-text name (e.g. 'Sequence Ontology'), but it is preferable to provide a uri/url for the system. When the 'code' is reported as a CURIE, the 'system' should be reported as the uri that the CURIE's prefix expands to (e.g. 'http://purl.obofoundry.org/so.owl/' for the Sequence Ontology).
   *  - systemVersion
      - 
      - string
      - 0..1
      - Version of the terminology or code system that provided the code.
   *  - code
      - 
      - :ref:`code`
      - 1..1
      - A symbol uniquely identifying the concept, as in a syntax defined by the code system. CURIE format is preferred where possible (e.g. 'SO:0000704' is the CURIE form of the Sequence Ontology code for 'gene').
