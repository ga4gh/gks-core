
.. warning:: This data class is at a **draft** maturity level and may change
    significantly in future releases. Maturity levels are described in 
    the :ref:`maturity-model`.
                      
                    
**Computational Definition**

A mapping to a concept in a terminology or code system.

**Information Model**

Some ConceptMapping attributes are inherited from :ref:`Element`.

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
      - string
      - 0..1
      - The 'logical' identifier of the data element in the system of record, e.g. a UUID.  This 'id' is unique within a given system, but may or may not be globally unique outside the system. It is used within a system to reference an object from another.
   *  - extensions
      - :ref:`Extension`
      - 0..m
      - A list of extensions to the Entity, that allow for capture of information not directly supported by elements defined in the model.
   *  - coding
      - :ref:`Coding`
      - 1..1
      - A structured representation of a code for a defined concept in a terminology or code system.
   *  - relation
      - string
      - 1..1
      - A mapping relation between concepts as defined by the Simple Knowledge Organization System (SKOS).
