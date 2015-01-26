====================
bgp-router
====================

 bgp-router include BGP peer,attribute,Autonomus system Number and so on.

bgp-routers Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type, Required,CRUD, Default Value, Validation Constraints,	Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   bgp_router_parameters " bgp-router " N/A " Yes " CRU " N/A " N/A " The root of bgp_router_parameters
   address " bgp_router_parameters " String " Yes " CRU " null " Valid IP address " The BGP router IP address
   address_families " bgp_router_parameters " N/A " Yes " CR " N/A " N/A " The root of addres_families
   family " address_families " list(str) " No " CRUD " null " Valid form {inet-vpn|inet6-vpn|route-target|e-vpn|erm-vpn} " Set BGP address families
   autonomous_system " bgp_router_parameters " integer " Yes " CRU " null " Valid range of AS " The peer AS number
   hold_time " bgp_router_parameters " integer " No " CRU " null " N/A " The hold time of BGP
   identifier " bgp_router_parameters " string " No " CRU " null " Valid IP address " BGP router ID
   port " bgp_router_parameters " string " No " CRU " null " 1-65535 " The port of BGP
   vendor " bgp_router_parameters " string " Yes " CRU " null " N/A " The vender name
   bgp_router_refs " bgp-router " N/A " No " CRU " N/A " N/A " The root of bgp_router_refs
   attr " bgp_router_refs " N/A " No " CRU " N/A " N/A " The root of attr
   session " attr " N/A " No " CRU " N/A " N/A " The root of session
   attributes " session " N/A " No " CRU " N/A " N/A " The root of attributes
   address_families " attributes " N/A " No " CRU " N/A " N/A " The root of addres_families
   family " address_families " list(str) " No " CRUD " [] " Valid form {inet-vpn|inet6-vpn|route-target|e-vpn|erm-vpn} " Set BGP address families
   bgp_router " attributes " N/A " No " R " null " N/A " Internal use
   uuid " session " uuid-str " No " R " generated " N/A " The UUID of this attribute
   href " bgp_router_refs " string " No " R " genereted " N/A " The URI of this attribute
   to " bgp_router_refs " list(str) " No " CR " [] " Valid to form <domain><project><network><routing instance> " The list of this attribute
   uuid " bgp_router_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute
   display_name " bgp-router " tring " No " CR " generated " N/A " Display name
   fq_name " bgp-router " list(str) " Yes " CR " [] " Valid from <domain>,<tenant>,<name> " The full query name of this attribute
   href " bgp-router " string " No " R " generated " N/A " The URI of this attribute
   id_perms " virtual-network " N/A " No " CR " generated " N/A " The root of id_perms
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
   name " bgp-router " string " No " CRU " generated " N/A " The name of virtual-network
   parent_href " virtual-network " string " No " R " generated " N/A " The URI of parent attribute
   parent_type " virtual-network " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " virtual-network " uuid-str " No " R " generated " N/A " The UUID of this attribute

bgp-routers JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "bgp-router": {
           "bgp_router_parameters": {
               "address": "<IP_ADDRESS>",
               "address_families": {
                   "family": [
                       "route-target",
                       "inet-vpn",
                       "inet6-vpn",
                       "e-vpn",
                       "erm-vpn"
                   ]
               },
               "autonomous_system": <AS_NUMBER>,
               "hold_time": 90,
               "identifier": "<IP_ADDRESS>",
               "port": 179,
               "vendor": "contrail"
           },
           "bgp_router_refs": [
               {
                   "attr": {
                       "session": [
                           {
                               "attributes": [
                                   {
                                       "address_families": {
                                           "family": [
                                               "inet-vpn",
                                               "inet6-vpn",
                                               "route-target",
                                               "e-vpn"
                                           ]
                                       },
                                       "bgp_router": null
                                   }
                               ],
                               "uuid": null
                           }
                       ]
                   },
                   "href": "http://<API-SERVER>/bgp-router/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<NETWORK>",
                       "<ROUTING INSTANCE>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               },
               {
                   "attr": {
                       "session": [
                           {
                               "attributes": [
                                   {
                                       "address_families": {
                                           "family": []
                                       },
                                       "bgp_router": null
                                   }
                               ],
                               "uuid": null
                           }
                       ]
                   },
                   "href": "http://<API-SERVER>/bgp-router/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<NETWORK>",
                       "<ROUTING INSTANCE>",
                       "<NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "display_name": "<NAME>",
           "fq_name": [
               "<DOMAIN>",
               "<PROJECT>",
               "<NETWORK>",
               "<ROUTING INSTANCE>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/bgp-router/<UUID>",
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
                   "uuid_lslong": 12825287036609496247,
                   "uuid_mslong": 16195309315277015226
               }
           },
           "name": "<NAME>",
           "parent_href": "http://<API-SERVER>/routing-instance/<UUID>",
           "parent_type": "routing-instance",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>"
       }
   }

