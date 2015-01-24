====================
network-policy
====================

 Put here  description of attribute

network-policys Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   display_name " network-policy" string "No " CR " generated " N/A " The display name
   fq_name " network-policy" list(str) "Yes " CR " [] " Valid form <domain>,<project>,<name>" The full query name of this attribute  
   href " network-policy"  string "No " R " generated " N/A " The URI of this attribute
   id_perms " network-policy" N/A "No " CR "generated " N/A " The root of this attribute
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute
   description " id_perms" string "No " CRU " null " N/A " The description of this attribute
   enable " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is enable or not
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " 0-7 " The access type of group
   other_access " permissions" int "No " CRU " generated " 0-7 " The access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " 0-7 " Access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is visible by user or not
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use
   name " network-policy" string "No " CRU " generated " N/A " The name of thie attribute
   network_policy_entries " network-policy" N/A "No " CR " N/A " N/A " The root of this attribute
   policy_rule " network_policy_entries" list(str) "No " CRUD " N/A " N/A " The network policy rule
   action_list " policy_rule" list(dict) "No " CRU " N/A " N/A " The policy action list
   apply_service " action_list" string "No " CRU " null " Valid ervice name" The apply service
   gateway_name " action_list" string "No " CRU " null " Valid gateway name " The gateway name
   mirror_to " action_list" string "No " CRU " null " Valid analyzer name" The Analyzer name
   simple_action " action_list" string "No " CRU " N/A " {alert|drop|deny|log|pass|reject} " The simple action type
   application " policy_rule" list(str) "No " CRU " [] " Valid application list " The application name
   direction " policy_rule" string "Yes " CRU " N/A " {>|<>} " The direction of traffic
   dst_addresses " policy_rule" list(str) "No " CRUD " N/A " N/A " The root od this attribute
   network_policy " dst_addresses" string "No " CRU " null " Valid network policy name" The network policy
   security_group " dst_addresses" string "No " CRU " null " Valid security group name" The security group
   subnet " dst_addresses" Type "Requ " CRU " N/A " N/A " The root of this attribute
   ip_prefix " subnet" string "No " CRUD " null " Valid network address " The network address of the subnet
   ip_prefix_len " subnet" int "No " CRUD " null " Valid IP prefix " The prefix of the subnet
   virtual_network " dst_addresses" string "No " CRU " null " Valid virtual network " The virtual network name
   dst_ports " policy_rule" list(dict) "No " CRU " N/A " N/A " The destination port range
   end_port " dst_ports" integer "No " CRU " null " -1-65535 " The end port of range
   start_port " dst_ports" integer "No " CRU " null " -1-65535 " The start port of range
   protocol " policy_rule" string "No " CRU " any " {tcp|udp|icmp|any} " The protocol name
   rule_sequence " policy_rule" list(dict) "No " CRU " N/A " N/A " The root of this attribute
   major " rule_sequence" integer "No " CRU " -1 " N/A " The major rule sequence
   minor " rule_sequence" integer "No " CRU " -1 " N/A " The minor rule sequence
   rule_uuid " policy_rule" uuid-str "No " CR " generated " N/A " The UUID of this attribute
   src_addresses " policy_rule" list(str) "No " CRUD " N/A " N/A " The root od this attribute
   network_policy " src_addresses" string "No " CRU " null " Valid network policy name" The network policy
   security_group " src_addresses" string "No " CRU " null " Valid security group name" The security group
   subnet " src_addresses" Type "Requ " CRU " N/A " N/A " The root of this attribute
   virtual_network " src_addresses" string "No " CRU " null " Valid virtual network " The virtual network name
   src_ports " policy_rule" list(dict) "No " CRU " N/A " N/A " The destination port range
   end_port " src_ports" integer "No " CRU " null " -1-65535 " The end port of range
   start_port " src_ports" integer "No " CRU " null " -1-65535 " The start port of range
   parent_href " network-policy" string "No " R " generated " N/A " The URI of this attribute
   parent_type " network-policy" string "Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " network-policy" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid " network-policy" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_network_back_refs " network-policy" list(str) "No " R " generated " N/A " The root of this attribute
   attr " virtual_network_back_refs" list(dict) "No " R " generated " N/A " The root of this attribute
   sequence " attr" Type "list(dict) " R " generated " N/A " The root of this attribute
   major " sequence" integer "No " R " generated " N/A " The major rule sequence
   minor " sequence" integer "No " R " generated " N/A " The minor rule sequence
   timer " attr" string "No " R " generated " N/A " The time of this attribute
   href " virtual_network_back_refs" string "No " R " generated " N/A " The URI of this attribute
   to " virtual_network_back_refs" list(str) "No " CR " [] " Valid form <domain>,<project>,<network> " The list of this attribute
   uuid " virtual_network_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute

network-policys JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "network-policy": {
           "display_name": "<NAME>",
           "fq_name": [
               "<DOMAIN>",
               "<PROJECT>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/network-policy/<UUID>",
           "id_perms": {
               "created": "<DATE>",
               "description": null,
               "enable": true,
               "last_modified": "<DATE>",
               "permissions": {
                   "group": "<GROUP>",
                   "group_access": 7,
                   "other_access": 7,
                   "owner": "<ADMIN>",
                   "owner_access": 7
               },
               "user_visible": true,
               "uuid": {
                   "uuid_lslong": 13137042031121705301,
                   "uuid_mslong": 6202226196110723417
               }
           },
           "name": "<NAME>",
           "network_policy_entries": {
               "policy_rule": [
                   {
                       "action_list": {
                           "apply_service": null,
                           "gateway_name": null,
                           "mirror_to": null,
                           "simple_action": "pass"
                       },
                       "application": [],
                       "direction": "<>",
                       "dst_addresses": [
                           {
                               "network_policy": null,
                               "security_group": null,
                               "subnet": null,
                               "virtual_network": "<DOMAIN>:<PROJECT>:<NETWORK>"
                           }
                       ],
                       "dst_ports": [
                           {
                               "end_port": <PORT>,
                               "start_port": <PORT>
                           }
                       ],
                       "protocol": "<PROTOCOL>",
                       "rule_sequence": {
                           "major": -1,
                           "minor": -1
                       },
                       "rule_uuid": "<UUID>",
                       "src_addresses": [
                           {
                               "network_policy": null,
                               "security_group": null,
                               "subnet": null,
                               "virtual_network": "<DOMAIN>:<PROJECT>:<NETWORK>"
                           }
                       ],
                       "src_ports": [
                           {
                               "end_port": <PORT>,
                               "start_port": <PORT>
                           }
                       ]
                   }
               ]
           },
           "parent_href": "http://<API-SERVER>/project/<UUID>",
           "parent_type": "project",
           "parent_uuid": "<UUID>",
           "uuid": "<UUID>",
           "virtual_network_back_refs": [
               {
                   "attr": {
                       "sequence": {
                           "major": 0,
                           "minor": 0
                       },
                       "timer": null
                   },
                   "href": "http://<API-SERVER>/virtual-network/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<NETWORK>"
                   ],
                   "uuid": "<UUID>"
               }
           ]
       }
   }

