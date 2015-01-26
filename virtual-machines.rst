====================
virtual-machine
====================

 virtual-machine includes virtual machine interface and so on

virtual-machines Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " virtual-machine " string " No " CR " generated " N/A " The display name
   fq_name " virtual-machine " list(str) " Yes " CR " [] " Valid form <name> " The full query name of this attribute
   href " virtual-machine " string " No " R " generated " N/A " The URI of the interface
   id_perms " virtual-machine " N/A " No " CRU " N/A " N/A " The root of this attribute
   created " id_perms " datetime " No " R " generated " N/A " The date time of created date of this attribute
   description " id_perms " string " No " CRU " null " N/A " The description of this attribute
   enable " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is enable or not
   last_modified " id_perms " datetime " No " R " generated " N/A " The date time of modified date of this attribute
   permissions " id_perms " list(dict) " No " CRU " generated " N/A " The owner and access level
   group " permissions " string " No " CRU " generated " N/A " The group of this attribute
   group_access " permissions " int " No " CRU " generated " 0-7 " The access type of group
   other_access " permissions " int " No " CRU " generated " 0-7 " The access type of others
   owner " permissions " string " No " CRU " generated " N/A " The name of the ownter of this attribute
   owner_access " permissions " int " No " CRU " generated " 0-7 " The access type of the ownter
   user_visible " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is visible by user or not
   uuid " id_perms " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid " int " No " R " generated " N/A " For internal use
   uuid_mslong " uuid " int " No " R " generated " N/A " For internal use
   name " virtual-machine " string " No " CRU " generated " N/A " The name of thie attribute
   uuid " virtual-machine " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_back_refs " virtual-machine " list(str) " No " R " generated " N/A " The root of this attribute
   attr " virtual_machine_interface_back_refs " N/A " No " R " generated " N/A " The root of this attribute
   href " virtual_machine_interface_back_refs " string " No " R " generated " N/A " The URI of the interface
   to " virtual_machine_interface_back_refs " list(str) " Yes " CRD " [] " Valid IPAM form <domain>,<project>,<network>,<name> " The list of this attribute
   uuid " virtual_machine_interface_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute

virtual-machines JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-machine": {
           "display_name": "<NAME>",
           "fq_name": [
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/virtual-machine/<UUID>",
           "id_perms": {
               "created": "<DATE>",
               "description": null,
               "enable": true,
               "last_modified": "<DATE>",
               "permissions": {
                   "group": "<GROUP>",
                   "group_access": 7,
                   "other_access": 7,
                   "owner": "<OWNER>",
                   "owner_access": 7
               },
               "user_visible": true,
               "uuid": {
                   "uuid_lslong": 11207594496087950160,
                   "uuid_mslong": 8807160146013473852
               }
           },
           "name": "<NAME>",
           "uuid": "<UUID>",
           "virtual_machine_interface_back_refs": [
               {
                   "attr": null,
                   "href": "http://<API-SERVER>/virtual-machine-interface/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<NETWORK>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ]
       }
   }

