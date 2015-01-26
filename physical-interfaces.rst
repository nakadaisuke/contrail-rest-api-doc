====================
physical-interface
====================

 physical-interface includes pyhsical interface attribute and so on

physical-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " physical-interface " string " No " CR " generated " N/A " The display name
   fq_name " physical-interface " list(str) " Yes " CR " [] " Valid form <system-config>,<physical-router>,<name> " The full query name of this attribute
   href " physical-interface " string " No " R " generated " N/A " The URI of this attribute
   id_perms " physical-interface " N/A " No " CRU " N/A " N/A " The root of this attribute
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
   logical_interfaces " physical-interface " list(str) " No " CRUD " [] " N/A " The root of this attribute
   href " logical_interfaces " tring " No " R " generated " N/A " The URI of this attribute
   to " logical_interfaces " list(str) " No " CR " [] " Valid form <system-config>,<physical-router>,<physical-port><logical-port> " The list of this attribute
   uuid " logical_interfaces " uuid-str " No " R " generated " N/A " The UUID of this attribute
   name " physical-interface " string " No " CRU " generated " N/A " The name of thie attribute
   parent_href " physical-interface " string " No " R " generated " N/A " The URI of this attribute
   parent_type " physical-interface " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " physical-interface " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid " physical-interface " uuid-str " No " R " generated " N/A " The UUID of this attribute

physical-interfaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "physical-interface": {
           "display_name": "<NAME>",
           "fq_name": [
               "<SYSTEM-CONFIG>",
               "<PHYSICAL-ROUTER>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/physical-interface/<UUID>",
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
                   "uuid_lslong": 13735952386302396629,
                   "uuid_mslong": 11915500640573540798
               }
           },
           "logical_interfaces": [
               {
                   "href": "http://<API-SERVER>/logical-interface/<UUID>",
                   "to": [
                       "<SYSTEM-CONFIG>",
                       "<PHYSICAL-ROUTER>",
                       "<PHYSICAL-INTERFACE>",
                       "<LOGICAL-INTERFACE>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "name": "<NAME>",
           "parent_href": "http://<API-SERVER>/physical-router/<UUID>",
           "parent_type": "physical-router",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>"
       }
   }
