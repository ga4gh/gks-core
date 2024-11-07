.. note:: This data class is at a **trial use** maturity level and may change
     in future releases. Maturity levels are described in
    the :ref:`maturity-model`.

**Computational Definition**

A concept label that may be mapped to one or more :ref:`Codings <Coding>`.

**Information Model**

Some MappableConcept attributes are inherited from :ref:`Element`.

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
   *  - conceptType
      - 
      - string
      - 0..1
      - A term indicating the type of concept being represented by the MappableConcept.
   *  - label
      - 
      - string
      - 1..1
      - A primary name for the concept.
   *  - mappings
      - 
                        .. raw:: html

                            <span style="background-color: #B2DFEE; color: black; padding: 2px 6px; border: 1px solid black; border-radius: 3px; font-weight: bold; display: inline-block; margin-bottom: 5px;" title="Unordered">&#8942;</span>
      - :ref:`ConceptMapping`
      - 0..m
      - A list of mappings to concepts in terminologies or code systems. Each mapping should include a coding and a relation.
