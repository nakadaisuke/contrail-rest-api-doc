====================
network-ipam
====================

 network-ipam includes IP address,DNS,host route,DHCP and so on

network-ipams Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " network-ipam" list(str) "Yes " CR " [] " Valid form <domain>,<project>,<name>" The full query name of this attribute 
   href " network-ipam" string "No " R " generated " N/A " The URI of this attribute
   id_perms " network-ipam" N/A "No " CR "generated " N/A " The root of this attribute
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
   uuid " id_perms" uuid-str "No " R " generated " N/A " The UUID of this attribute
   uuid_lslong " uuid" int "No " R " generated " N/A " For internal use
   uuid_mslong " uuid" int "No " R " generated " N/A " For internal use 
   name " network-ipam" string "No " CRU " generated " N/A " The name of thie attribute  
   network_ipam_mgmt " network-ipam" N/A "No " CR " generated " N/A " The root of this attribute
   ipam_dns_method " network_ipam_mgmt" string "Yes " CRU " N/A " {none|default-dns-server|tenant-dns-serer|virtual-dns-server} " The IPAM DNS method
   ipam_dns_server " network_ipam_mgmt" N/A "No " CR " generated " N/A " The root of this attribute  
   tenant_dns_server_address " ipam_dns_server" String "No " CRU " null " Valid IP address" Tenant DNS server IP address
   virtual_dns_server_name " ipam_dns_server" string "No " CRUD " null " N/A " The virtual DNS server name
   parent_href " network-ipam" string "No " R " generated " N/A " The URI of this attribute
   parent_type " network-ipam" string "Yes " CR " null " Valid parent name " The parent attribute 
   parent_uuid " network-ipam" uuid-str "No " R " generated " N/A " The UUID of this attribute 
   uuid " network-ipam" uuid-str "No " R " generated " N/A " The UUID of this attribute
   virtual_DNS_refs " network-ipam" N/A "No " CR " generated " N/A " The root of this attribute 
   attr " virtual_DNS_refs" N/A "No " CR " generated " N/A " The root of this attribute 
   sequence " attr" N/A "No " CR " generated " N/A " The root of this attribute 
   major " sequence" integer "No " CRU " 0 " N/A " The major sequence
   minor " sequence" integer "No " CRU " 0 " N/A " The minor sequence
   href " virtual_DNS_refs" string "No " R " generated " N/A " The URI of this attribute 
   to " virtual_DNS_refs" list(str) "No " CR " [] " Valid form <domain>,<name> " The list of this attribute
   uuid " virtual_DNS_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute  
   virtual_network_back_refs " network-ipam" N/A "No " CR " generated " N/A " The root of this attribute  
   attr " virtual_network_back_refs" N/A "No " CR " generated " N/A " The root of this attribute 
   ipam_subnets " attr" N/A "No " CR " generated " N/A " The root of this attribute 
   addr_from_start " ipam_subnets" bool "Yes " CRU " N/A " {true|false}" Specifies whether the address allocation method is start or end
   allocation_pools " ipam_subnets" N/A "No " CR " [] " N/A " The root of this attribute 
   end " allocation_pools" string "No " CRUD " null " Valid IP address " The end of allocation pool
   start " allocation_pools" string "No " CRUD " null " Valid IP address" The start of allocation pool
   default_gateway " ipam_subnets" string "No " CRUD " null " Valid IP address" The default gateway IP address
   dhcp_option_list " ipam_subnets" N/A "No " CR " [] " N/A " The root of this attribute
   dhcp_option " dhcp_option_list" list(dict) "No " CRUD " [] " Valid DHCP option " The DHCP option     
   dns_nameservers " ipam_subnets" list(str) "No " CRUD " null " N/A " The DNS namesarver name
   dns_server_address " ipam_subnets" string "No " CRUD " null " Valid IP address " The DNC server IP address
   enable_dhcp " ipam_subnets" bool "Yes " CRU " N/A " {true|false} " Specifies whether the DHCP enable or disable
   host_routes " ipam_subnets" N/A "No " CR " null " N/A " The root of this attribute
   route " host_routes" N/A "No " CR " [] " N/A " The root of this attribute
   next_hop " route" string "No " CRUD " null " Valid IP address " The next hop IP address
   next_hop_type " route" string "No " CRUD " null " N/A " The next hop Type
   prefix " route" string "No " CRD " null " Valid network address " The network address with prefix
   subnet " ipam_subnets" N/A "No " CRD " generated " N/A " The root of this attribute
   ip_prefix " subnet" string "No " CRD " null " Valid network address " The network address of the subnet
   ip_prefix_len " subnet" int "No " CRD " null " Valid IP prefix " The prefix of the subnet
   subnet_uuid " ipam_subnets" uuid-str "No " R " generated " N/A " The UUID of this attribute  
   href " virtual_network_back_refs" string "No " R " generated " N/A " The URI of this attribute 
   to " virtual_network_back_refs" list(str) "No " CR " [] " Valid form <uuid> " The list of this attribute 
   uuid " virtual_network_back_refs" uuid-str "No " R " generated " N/A " The UUID of this attribute  
 
network-ipams JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "network-ipam": {
           "fq_name": [
               "<DOMAIN>", 
               "<PROJECT>", 
               "<NAME>"
           ], 
           "href": "http://<API-SERVER>/network-ipam/<UUID>", 
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
                   "uuid_lslong": 10709772514233599446, 
                   "uuid_mslong": 13267335360305971946
               }
           }, 
           "name": "default-network-ipam", 
           "network_ipam_mgmt": {
               "ipam_dns_method": "virtual-dns-server", 
               "ipam_dns_server": {
                   "tenant_dns_server_address": null, 
                   "virtual_dns_server_name": "<DOMAIN>:<NAME>"
               }
           }, 
           "parent_href": "http://<API-SERVER>/project/<UUID>", 
           "parent_type": "project", 
           "parent_uuid": "<UUID>", 
           "uuid": "<UUID>", 
           "virtual_DNS_refs": [
               {
                   "attr": {
                       "sequence": {
                           "major": 0, 
                           "minor": 0
                       }
                   }, 
                   "href": "http://<API-SERVER>/virtual-DNS/<UUID>", 
                   "to": [
                       "<DOMAIN>", 
                       "<NAME>"
                   ], 
                   "uuid": "<UUID>"
               }
           ], 
           "virtual_network_back_refs": [
               {
                   "attr": {
                       "ipam_subnets": [
                           {
                               "addr_from_start": true, 
                               "allocation_pools": [
                                   {
                                       "end": "<IP_ADDRESS>", 
                                       "start": "<IP_ADDRESS>"
                                   }
                               ], 
                               "default_gateway": "<IP_ADDRESS>", 
                               "dhcp_option_list": {
                                   "dhcp_option": []
                               }, 
                               "dns_nameservers": [], 
                               "dns_server_address": "<IP_ADDRESS>", 
                               "enable_dhcp": true, 
                               "host_routes": {
                                   "route": [
                                       {
                                           "next_hop": "<IP_ADDRESS>", 
                                           "next_hop_type": null, 
                                           "prefix": "<IP_PREFIX>"
                                       }
                                   ]
                               }, 
                               "subnet": {
                                   "ip_prefix": "<NETWORK>", 
                                   "ip_prefix_len": <PREFIX>
                               }, 
                               "subnet_uuid": "<UUID>"
                           }
                       ]
                   }, 
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
