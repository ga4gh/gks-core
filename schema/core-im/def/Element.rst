
.. note:: This data class is at a **trial use** maturity level and may change
    in future releases. Maturity levels are described in the :ref:`maturity-model`.
                      
                    
**Computational Definition**

The base definition for all identifiable data objects.

**Information Model**


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
