====================
access-control-list
====================

 Put here  description of attribute 

access-control-lists Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Noired,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   access_control_list_entries " access-control-list" N/A "N/A " CR " generated " N/A " The root of access-control_list_entries
   acl_rule " access_control_list_entries" N/A "N/A " CR " generated " N/A " The root of acl_rule
   action_list " acl_rule" N/A "N/A " CR " generated " N/A " The root of action_list
   apply_service " action_list" list(str) "No " CRUD " [] " Valid string " The Service instance list
   assign_routing_instance " action_list" string "No  " CRUD "null " Valid routing instance " Next hop Routing instance
   gateway_name " action_list" string "No " CRUD " null " Valid Gateway name " Next hop IP address
   mirror_to " action_list" list[str] "No " CRUD " null " Valid list [analyzer-name,encapsulation,analyzer-ip-address,routing-instance,udp-port] "The packet mirroring data
   simple_action " action_list" String "No " CRU " pass " {alert|drop|deny|log|pass|reject} " Specifies action for the packet
   match_condition " acl_rule" N/A "No " CR " N/A " N/A " The root of match_condition
   dst_address " match_condition" string "No " CRU " null " Valid IP address " The destination address for ACL
   network_policy " dst_address" string "No " CRU " null " {sequence|timer} " The network policy time
   security_group " dst_address" integer "No " CRU " null " Valid security group ID " The security group ID
   subnet " dst_address" list(dict) "No " CRUD " null " N/A " The root of subnet
   ip_prefix " subnet" string "No " CRUD " null " Valid IP address " The IP address of subnet
   ip_prefix_len " subnet" integer "No " CRUD " null " Valid prefix rength " The prefix of IP address
   virtual_network " dst_address" string  "No " CRUD " null "Valid virtual network name " The virtual network attaching to ACL
   dst_port " match_condition" list(dict) "No " CRUD " null " N/A " The destination port range
   end_port " dst_port" integer "No " CRU " null " -1-65535 " The end port of range
   start_port " dst_port" integer "No " CRU " null " -1-65535 " The start port of range
   protocol " match_condition" string "No " CRU " any " {tcp|udp|icmp|any} " The protocol name
   src_address " match_condition" string "No " CRU " null " Valid IP address " The source address for ACL
   network_policy " src_address" string "No " CRU " null " {sequence|timer} " The network policy time
   security_group " src_address" integer "No " CRU " null " Valid security group ID " The security group ID
   subnet " src_address" list(dict) "No " CRUD " null " N/A " The root of subnet
   ip_prefix " subnet" string "No " CRUD " null " Valid IP address " The IP address of subnet
   ip_prefix_len " subnet" integer "No " CRUD " null " Valid prefix rength " The prefix of IP address
   virtual_network " src_address" string  "No " CRUD " null "Valid virtual network name " The virtual network attaching to ACL
   src_port " match_condition" list(dict) "No " CRUD " null " N/A " The destination port range 
   end_port " src_port" integer "No " CRU " null " -1-65535 " The end port of range
   start_port " src_port" integer "No " CRU " null " -1-65535 " The start port of range
   rule_uuid " acl_rule" uuid-str "No " CR " generated " N/A " The UUID of this attribute 
   dynamic " access_control_list_entries" bool "No " CRUD " null " {true|false} " Specifies whether access list is dynamic or not.
   display_name " access-control-list" string "No " CR " generated " N/A " Display name
   fq_name " access-control-list" list(str) "Yes " CR " [] " Valid full query name form <domain>,<tenant>,<name> " The full query name of this attribute
   href " access-control-list" string "No " R " generated " N/A " The URI of this instance IP
   id_perms " virtual-network" N/A "No " CR "generated " N/A " The root of id_perms
   created " id_perms" datetime "No " R " generated " N/A " The date time of created date of this attribute 
   description " id_perms" string "No " CRU " null " N/A " Description of this attribute
   enable " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is enable or not 
   last_modified " id_perms" datetime "No " R " generated " N/A " The date time of modified date of this attribute  
   permissions " id_perms" list(dict) "No " CRU " generated " N/A " The owner and access level
   group " permissions" string "No " CRU " generated " N/A " The group of this attribute
   group_access " permissions" int "No " CRU " generated " 0-7 " Access type of group 
   other_access " permissions" int "No " CRU " generated " 0-7 " Access type of others
   owner " permissions" string "No " CRU " generated " N/A  " The name of the ownter of this attribute
   owner_access " permissions" int "No " CRU " generated " 0-7 " Access type of the ownter
   user_visible " id_perms" bool "No " CRU " true "{true|false} " Specifies whethere this attribute is visible by user or not 
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of id_perms attribute  
   uuid_lslong " uuid" int "No " R " generated " N/A " for internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   name " access-control-list" Type "No " CRU " Default " Valid " ABCDE
   parent_href " access-control-list" string "No " R " generated " N/A " The URI of parent attribute
   parent_type " access-control-list" string "Yes " CR " null " Valid parent name " The parent attribute
   parent_uuid " access-control-list" uuid-str "No " R " generated "N/A " The UUID of parent attribute
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of id_perms attribute 

access-control-lists JSON
====
.. highlight:: json
   :linenothreshold: 5

::

   {
       "access-control-list": {
           "access_control_list_entries": {
               "acl_rule": [
                   {
                       "action_list": {
                           "apply_service": [], 
                           "assign_routing_instance": null, 
                           "gateway_name": null, 
                           "mirror_to": null, 
                           "simple_action": "pass"
                       }, 
                       "match_condition": {
                           "dst_address": {
                               "network_policy": null, 
                               "security_group": null, 
                               "subnet": null, 
                               "virtual_network": null
                           }, 
                           "dst_port": {
                               "end_port": 65535, 
                               "start_port": 0
                           }, 
                           "protocol": "any", 
                           "src_address": {
                               "network_policy": null, 
                               "security_group": null, 
                               "subnet": {
                                   "ip_prefix": "<IP_ADDRESS>", 
                                   "ip_prefix_len": "<PREFIX>" 
                               }, 
                               "virtual_network": null
                           }, 
                           "src_port": {
                               "end_port": 65535, 
                               "start_port": 0
                           }
                       }, 
                       "rule_uuid": "<UUID>"
                   }
               ], 
               "dynamic": null
           }, 
           "display_name": "ingress-access-control-list", 
           "fq_name": [
               "default-domain", 
               "demo", 
               "default", 
               "ingress-access-control-list"
           ], 
           "href": "http://<API-SERVER>/access-control-list/<UUID>", 
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
                   "uuid_lslong": <INTEGER>, 
                   "uuid_mslong": <INTEGER>
               }
           }, 
           "name": "ingress-access-control-list", 
           "parent_href": "http://<API-SERVER>/security-group/<DATE>", 
           "parent_type": "security-group", 
           "parent_uuid": "<DATE>", 
           "uuid": "<UUID>"
       }
   }
