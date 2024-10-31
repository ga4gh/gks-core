
.. warning:: This data class is at a **draft** maturity level and may change
    significantly in future releases. Maturity levels are described in 
    the :ref:`maturity-model`.
                      
                    
**Computational Definition**

The abstract entity representing a possible fact that may be put forth as true, or subjected to an evidence-based assessment, by a Statement. As abstract entities, their identity and existence are independent of space and time, and whether they are ever asserted to be true by some agent. Propositions may be used in two contexts; (1) by Statements that assert them to be true or false, or describe the overall level of confidence/evidence for or against them; (2) by Evidence Lines that report the direction and strength of an evidence-based argument for the Proposition.

**Information Model**

Some Proposition attributes are inherited from :ref:`Entity`.

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
      - The 'logical' identifier of the Entity in the system of record, e.g. a UUID.  This 'id' is unique within a given system, but may or may not be globally unique outside the system. It is used within a system to reference an object from another.
   *  - label
      - string
      - 0..1
      - A primary name for the entity.
   *  - description
      - string
      - 0..1
      - A free-text description of the Entity.
   *  - alternativeLabels
      - string
      - 0..m
      - Alternative name(s) for the Entity.
   *  - extensions
      - :ref:`Extension`
      - 0..m
      - A list of extensions to the Entity, that allow for capture of information not directly supported by elements defined in the model.
   *  - type
      - string
      - 1..1
      - Must be "Proposition"
   *  - propositionText
      - string
      - 0..1
      - A natural-language expression of the Proposition's meaning. e.g. "BRCA2 c.8023A>G is pathogenic for Breast Cancer".
   *  - subject
      - object
      - 1..1
      - The Entity or concept about which the Proposition is made.
   *  - predicate
      - string
      - 1..1
      - The relationship declared to hold between the subject and the object of the Statement.
   *  - object
      - object
      - 1..1
      - An Entity or concept that is related to the subject of a Proposition via its predicate.
