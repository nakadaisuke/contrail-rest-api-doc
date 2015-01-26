====================
security-group
====================

 security-group includes virtual network,security parameters and so on

security-groups Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: "

   access_control_lists " security-group " list(str) " No " CRUD " [] " N/A " The root of this attribute
   href " access_control_lists " string " No " R " generated " N/A " The URI of this attribute
   to " access_control_lists " list(str) " No " CR " [] " Valid form <domain>,<project>,<network>,<name> " The list of this attribute
   uuid " access_control_lists " uuid-str " No " R " generated " N/A " The UUID of this attribute
   display_name " security-group " string " No " CR " generated " N/A " The display name
   fq_name " security-group " list(str) " Yes " CR " [] " Valid form <domain>,<project>,<network>,<name> " The full query name of this attribute
   href " access_control_lists " string " No " R " generated " N/A " The URI of this attribute
   id_perms " access_control_lists " N/A " No " CRU " N/A " N/A " The root of this attribute
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
   name " security-group " string " No " CRU " generated " N/A " The name of thie attribute
   parent_href " security-group " string " No " R " generated " N/A " The URI of this attribute
   parent_type " security-group " string " Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " security-group " uuid-str " No " R " generated " N/A " The UUID of this attribute
   security_group_entries " security-group " N/A " No " CR " N/A " The root of this attribute
   policy_rule " security_group_entries " list(str) " No " CRUD " N/A " N/A " The network policy rule
   action_list " policy_rule " list(dict) " No " CRU " N/A " N/A " The policy action list
   apply_service " action_list " string " No " CRU " null " Valid ervice name " The apply service
   direction " policy_rule " string " Yes " CRU " N/A " Valid form {>|<>} " The direction of traffic
   dst_addresses " policy_rule " list(str) " No " CRUD " N/A " N/A " The root od this attribute
   network_policy " dst_addresses " string " No " CRU " null " Valid network policy name " The network policy
   security_group " dst_addresses " string " No " CRU " null " Valid security group name " The security group
   subnet " dst_addresses " Type " Requ " CRU " N/A " N/A " The root of this attribute
   ip_prefix " subnet " string " No " CRUD " null " Valid network address " The network address of the subnet
   ip_prefix_len " subnet " int " No " CRUD " null " Valid IP prefix " The prefix of the subnet
   virtual_network " dst_addresses " string " No " CRU " null " Valid virtual network " The virtual network name
   dst_ports " policy_rule " list(dict) " No " CRU " N/A " N/A " The destination port range
   end_port " dst_ports " integer " No " CRU " null " -1-65535 " The end port of range
   start_port " dst_ports " integer " No " CRU " null " -1-65535 " The start port of range
   protocol " policy_rule " string " No " CRU " any " Valid form {tcp|udp|icmp|any} " The protocol name
   rule_sequence " policy_rule " list(dict) " No " CRU " null " N/A " The root of this attribute
   major " rule_sequence " integer " No " CRU " -1 " N/A " The major rule sequence
   minor " rule_sequence " integer " No " CRU " -1 " N/A " The minor rule sequence
   rule_uuid " policy_rule " uuid-str " No " CR " generated " N/A " The UUID of this attribute
   src_addresses " policy_rule " list(str) " No " CRUD " N/A " N/A " The root od this attribute
   network_policy " src_addresses " string " No " CRU " null " Valid network policy name " The network policy
   security_group " src_addresses " string " No " CRU " null " Valid security group name " The security group
   subnet " src_addresses " Type " Requ " CRU " N/A " N/A " The root of this attribute
   virtual_network " src_addresses " string " No " CRU " null " Valid virtual network " The virtual network name
   src_ports " policy_rule " list(dict) " No " CRU " N/A " N/A " The destination port range
   end_port " src_ports " integer " No " CRU " null " -1-65535 " The end port of range
   start_port " src_ports " integer " No " CRU " null " -1-65535 " The start port of range
   security_group_id " security-group " string " Yes " CR " null " N/A " The security group ID
   uuid " security-group " uuid-str " No " R " generated " N/A " The UUID of this attribute
   virtual_machine_interface_back_refs " security-group " list(str) " No " R " generated " N/A " The root of this attribute
   to " virtual_machine_interface_back_refs " list(str) " No " CR " [] " Valid form <domain>,<project>,<network> " The list of this attribute
   href " virtual_machine_interface_back_refs " string " No " R " generated " N/A " The URI of this attribute
   attr " virtual_machine_interface_back_refs " list(dict) " No " R " generated " N/A " The root of this attribute
   uuid " virtual_machine_interface_back_refs " uuid-str " No " R " generated " N/A " The UUID of this attribute

security-groups JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "security-group": {
           "access_control_lists": [
               {
                   "href": "http://<API-SERVER>/access-control-list/<UUID>",
                   "to": [
                       "<DOMAIN>",
                       "<PROJECT>",
                       "<NAME>",
                       "<ACL_NAME>"
                   ],
                   "uuid": "<UUID>"
               }
           ],
           "display_name": "<NAME>",
           "fq_name": [
               "<DOMAIN>",
               "<PROJECT>",
               "<NAME>"
           ],
           "href": "http://<API-SERVER>/security-group/<UUID>",
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
                   "uuid_lslong": 10165588832123798848,
                   "uuid_mslong": 4042981921413877472
               }
           },
           "name": "<NAME>",
           "parent_href": "http://<API-SERVER>/project/<UUID>",
           "parent_type": "project",
           "parent_uuid": "<UUID>",
           "security_group_entries": {
               "policy_rule": [
                   {
                       "action_list": null,
                       "application": [],
                       "direction": ">",
                       "dst_addresses": [
                           {
                               "network_policy": null,
                               "security_group": null,
                               "subnet": {
                                   "ip_prefix": "<IP_ADDRESS>",
                                   "ip_prefix_len": <PREFIX>
                               },
                               "virtual_network": null
                           }
                       ],
                       "dst_ports": [
                           {
                               "end_port": <PORT>,
                               "start_port": <PORT>
                           }
                       ],
                       "protocol": "icmp",
                       "rule_sequence": null,
                       "rule_uuid": "<UUID>",
                       "src_addresses": [
                           {
                               "network_policy": null,
                               "security_group": "local",
                               "subnet": {
                                   "ip_prefix": "<IP_ADDRESS>",
                                   "ip_prefix_len": <PREFIX>
                               },
                               "virtual_network": null
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
           "security_group_id": 1,
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
