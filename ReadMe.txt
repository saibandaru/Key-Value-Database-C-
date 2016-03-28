Project 2
=========
Assumptions:
------------
* In this project I have taken scheduler time as 1 sec and number of writes
beforing saving to database as 4.

Demonstration
-------------
Here I am taking two database to demonstrate two different types of payloads
	1. Native type so I call this database as Native database
	1. Collection type so I call this database as Collection database(Like List<string>)

XML Structure
-------------
<?xml version="1.0" encoding="utf-8" standalone="yes"?>
<NoSQLDatabase>
  <KEY_TYPE>string</KEY_TYPE>
  <PAYLOAD_TYPE>List&lt;string&gt;</PAYLOAD_TYPE>
  <KEY key="1000" name="Element_1000 List Replace" description="Element_1000 List Description Replace" timestamp="2015-10-07T14:36:25.8116323-04:00">
    <Payload>
      <value>Element_1000 Data1 Replace</value>
      <value>Element_1000 Data2 Replace</value>
      <value>Element_1000 Data3 Replace</value>
    </Payload>
    <child>List Child_1 Replace</child>
    <child>List Child_2 Replace</child>
    <child>List Child_3 Replace</child>
  </KEY>
</NoSQLDatabase>

Key/Value is saved as:
---------------------
  <KEY key="1000" name="Element_1000 List Replace" description="Element_1000 List Description Replace" timestamp="2015-10-07T14:36:25.8116323-04:00">
    <Payload>
      <value>Element_1000 Data1 Replace</value>
      <value>Element_1000 Data2 Replace</value>
      <value>Element_1000 Data3 Replace</value>
    </Payload>
    <child>List Child_1 Replace</child>
    <child>List Child_2 Replace</child>
    <child>List Child_3 Replace</child>
  </KEY>

Type of database in XML file is captured in:
<KEY_TYPE>string</KEY_TYPE>
<PAYLOAD_TYPE>List&lt;string&gt;</PAYLOAD_TYPE>