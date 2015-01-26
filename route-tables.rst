====================
route-table
====================

 route-table includes routes, next hop, virtual network and so on 

route-tables Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " route-table " string " No " CR " generated " N/A " The display name
   fq_name " route-table " list(str) " Yes " CR " [] " Valid form <domain>,<project>,<name> " The full query name of this attribute
   href " route-table " string " No " R " generated " N/A " The URI of this attribute
   id_perms " route-table " N/A " No " CRU " N/A " N/A " The root of this attribute
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
   name " route-table " string " No " CRU " generated " N/A " The name of thie attribute
   parent_href " route-table " string " No " R " generated " N/A " The URI of this attribute
   parent_type " route-table " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " route-table " uuid-str " No " R " generated " N/A " The UUID of this attribute
   routes " route-table " N/A " No " CRD " N/A " N/A " The root of this attribute
   route " routes " list(dict) " No " CR " N/A " N/A " The root of this attribute
   next_hop " route " string " No " CRU " null " N/A " The next hop interface
   next_hop_type " route " string " No " CRU " null " N/A " The next hop type
   prefix " route " string " No " CRU " null " N/A " The IP address with prefix
   uuid " route-table " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_network_back_refs " route-table " list(str) " No " R " generated " N/A " The root of this attribute
   attr " virtual_network_back_refs " string " No " R " generated " N/A " The list of this attribute
   href " virtual_network_back_refs " string " No " R " generated " N/A " The URI of the interface
   to " virtual_network_back_refs " list(str) " No " R " generated " N/A " The list of this attribute
   uuid " virtual_network_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute

route-tables JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "route-table": {
           "display_name": "<NAME>",
           "fq_name": [
               "<DOMAIN>",
               "<PROJECT>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/route-table/<UUID>",
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
                   "uuid_lslong": 11685813492722890621,
                   "uuid_mslong": 180340793313414858
               }
           },
           "name": "<NAME>",
           "parent_href": "http://<API-SERVER>/project/<UUID>",
           "parent_type": "project",
           "parent_uuid": "<UUID>",
           "routes": {
               "route": [
                   {
                       "next_hop": "<NEXT-HOP>",
                       "next_hop_type": null,
                       "prefix": "<PREFIX>"
                   }
               ]
           },
           "uuid": "<UUID>",
           "virtual_network_back_refs": [
               {
                   "attr": null,
                   "href": "http://<API-SERVER>/virtual-network/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ]
       }
   }
