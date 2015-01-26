====================
domain
====================

 domain includes namespaces,projects,service templates.

domains Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   fq_name " domain " list(str) " Yes " CR " N/A " Valid from <domain> " The full query name of this attribute
   href " domain " string " No " R " generated " N/A " The URI of this attribute
   id_perms " domain " N/A " No " CR " generated " N/A " The root of this attribute
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
   name " domain " string " No " CRU " generated " N/A " The name of this attribute
   namespaces " domain " list(dict) " No " CRU " [] " N/A " The root of this attribute
   href " namespaces " str " No " R " generated " N/A " The URI of this attribute
   to " namespaces " list(str) " No " CRU " [] " Valid domain form <domain>,<namespace> " The list of this attribute
   uuid " namespaces " uuid-str " No " R " generated " N/A " The uuid of this attribute
   projects " domain " list(dict) " No " CRU " [] " N/A " The root of this attribute
   href " projects " str " No " R " generated " N/A " The URI of this attribute
   to " projects " list(str) " No " CRU " [] " Valid domain form <domain>,<project> " The list of this attribute
   uuid " projects " uuid-str " No " R " generated " N/A " The uuid of this attribut
   service_templates " domain " list(dict) " No " CRU " [] " N/A " The root of this attribute
   href " service_templates " str " No " R " generated " N/A " The URI of this attribute
   to " service_templates " list(str) " No " CRU " [] " Valid domain form <domain>,<service_templates> " The list of this attribute
   uuid " service_templates " uuid-str " No " R " generated " N/A " The uuid of this attribut
   uuid " domain " uuid-str " No " R " generated " N/A " The uuid of this attribut
   virtual_DNSs " domain " list(dict) " No " CRU " [] " N/A " The root of this attribute
   href " virtual_DNSs " str " No " R " generated " N/A " The URI of this attribute
   to " virtual_DNSs " list(str) " No " CRU " [] " Valid domain form <domain>,<dns> " The list of this attribute
   uuid " virtual_DNSs " uuid-str " No " R " generated " N/A " The uuid of this attribut

domains JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "domain": {
           "fq_name": [
               "<DOMAIN>"
           ],
           "href": "http://<API-SERVER>/domain/<UUID>",
           "id_perms": {
               "created":: "<DATE>",
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
                   "uuid_lslong": 9771981931291160937,
                   "uuid_mslong": 1288797455661024092
               }
           },
           "name": "<DOMAIN>",
           "namespaces": [
               {
                   "href": "http://<API-SERVER>/namespace/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "projects": [
               {
                   "href": "http://<API-SERVER>/project/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }, :
           ],
           "service_templates": [
               {
                   "href": "http://<API-SERVER>/service-template/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               },
           ],
           "uuid": "<UUID>",
           "virtual_DNSs": [
               {
                   "href": "http://<API-SERVER>/virtual-DNS/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               },
           ]
       }
   }
