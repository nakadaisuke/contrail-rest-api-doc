====================
namespace
====================

 namespace includes name space ID and so on

namespaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   fq_name " namespace " list(str) " Yes " CR " [] " Valid form <domain>,<name> " The full query name of this attribute
   href " namespace " string " No " R " generated " N/A " The URI of this attribute
   id_perms " namespace " N/A " No " CR " generated " N/A " The root of this attribute
   created " id_perms " datetime " No " R " generated " N/A " The date time of created date of this attribute
   description " id_perms " string " No " CRU " null " N/A " Description of this attribute
   enable " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is enable or not
   last_modified " id_perms " datetime " No " R " generated " N/A " The date time of modified date of this attribute
   permissions " id_perms " list(dict) " No " CRU " generated " N/A " The owner and access level
   group " permissions " string " No " CRU " generated " N/A " The group of this attribute
   group_access " permissions " int " No " CRU " generated " 0-7 " Access type of group
   other_access " permissions " int " No " CRU " generated " 0-7 " Access type of others
   owner " permissions " string " No " CRU " generated " N/A " The name of the ownter of this attribute
   owner_access " permissions " int " No " CRU " generated " 0-7 " Access type of the ownter
   user_visible " id_perms " bool " No " CRU " true " Valid form {true|false} " Specifies whethere this attribute is visible by user or not
   uuid " id_perms " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid " int " No " R " generated " N/A " For internal use
   uuid_mslong " uuid " int " No " R " generated " N/A " For internal use
   name " namespace " string " No " CRU " generated " N/A " The name of thie attribute
   parent_href " namespace " string " No " R " generated " N/A " The URI of this attribute
   parent_type " namespace " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " namespace " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid " namespace " uuid-str " No " R " generated " N/A " The UUID of this attribute

namespaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "namespace": {
           "fq_name": [
               "<DOMAIN>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/namespace/<UUID>",
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
                   "uuid_lslong": 9227266734083715499,
                   "uuid_mslong": 18393455295341873115
               }
           },
           "name": "<NAME>",
           "parent_href": "http://<API-SERVER>/domain/<UUID>",
           "parent_type": "domain",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>"
       }
   }
