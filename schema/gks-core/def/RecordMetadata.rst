**Computational Definition**

A reusable structure that encapsulates provenance metadata about a serialized data record or object in a particular dataset (as opposed to provenance about the real world entity this record or object represents).

**Information Model**

Some RecordMetadata attributes are inherited from :ref:`Element`.

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
   *  - recordIdentifier
      - string
      - 0..1
      - The identifier of the data record or object described in this RecordMetadata object.
   *  - recordVersion
      - string
      - 0..1
      - The version number of the record-level artifact the object describes.
   *  - derivedFrom
      - string
      - 0..1
      - Another data record from which the record described here was derived, through a data ingest and/or transformation process. Value should be a string representing the identifier of the source record.
   *  - dateRecordCreated
      - string
      - 0..1
      - The date the record was initially created.
   *  - contributions
      - :ref:`Contribution`
      - 0..m
      - Describes specific contributions made by an human or software agent to the creation, modification, or administrative management of a data record or object.
