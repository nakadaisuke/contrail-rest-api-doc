====================
floating-ip-pool
====================

 floating-ip-pool includes Floating IP address,belinging Network and so on

floating-ip-pools Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " floating-ip-pool " string " No " CR " generated " N/A " Display name
   floating_ips " floating-ip-pool " N/A " No " CR " N/A " N/A " The root of this attribute
   href " floating_ips " string " No " R " generated " N/A " The URI of this attribute
   to " floating_ips " list(str) " No " CR " [] " Valid form <domain>,<project>,<network>,<attribute>,<uuid> " The list of this attribute
   uuid " floating_ips " uuid-str " No " R " generated " N/A " The UUID of this attribute
   fq_name " floating-ip-pool " list(str) " Yes " CR " N/A " Valid form <domain>,<project>,<network>,<attribute> " The full query name of this attribute
   href " floating-ip-pool " string " No " R " generated " N/A " The URI of this attribute
   id_perms " floating_ips " N/A " No " CR " generated " N/A " The root of this attribute
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
   uuid_lslong " uuid " int " No " R " generated " N/A " for internal use
   uuid_mslong " uuid " int " No " R " generated " N/A " For internal use
   name " floating-ip-pool " Type " Requ " CRU " Default " Valid " ABCDE
   parent_href " floating-ip-pool " string " No " R " generated " N/A " The URI of this attribute
   parent_type " floating-ip-pool " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " floating-ip-pool " uuid-str " No " R " generated " N/A " The UUID of this attribute
   uuid " floating-ip-pool " uuid-str " No " R " generated " N/A " The UUID of this attribute

floating-ip-pools JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "floating-ip-pool": {
           "display_name": "<NAME>",
           "floating_ips": [
               {
                   "href": "http://<API-SERVER>/floating-ip/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROKECT>",
                       "<NETWORK>",
                       "<ATTRIBUTE>",
                       "<UUID>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "fq_name": [
               "<DOMAIN>",
               "<PROJECT>",
               "<NETWORK>",
               "<ATTRIBUTE>"
           ],
           "href": "http://<API-SERVER>/floating-ip-pool/<UUID>",
           "id_perms": {
               "created": "<DATE>",
               "description": null,
               "enable": true,
               "last_modified": "<DATE>",
               "permissions": {
                   "group": "admin",
                   "group_access": 7,
                   "other_access": 7,
                   "owner": "admin",
                   "owner_access": 7
               },
               "user_visible": true,
               "uuid": {
                   "uuid_lslong": 10122021800172585294,
                   "uuid_mslong": 15329672797270788202
               }
           },
           "name": "default",
           "parent_href": "http://<API-SERVER>/virtual-network/<UUID>",
           "parent_type": "virtual-network",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>"
       }
   }
