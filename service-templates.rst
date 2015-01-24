====================
service-template
====================

 Put here  description of attribute 

service-templates Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   href " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   service_template_properties " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   availability_zone_enable " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   interface_type " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   static_route_enable " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   shared_ip " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   service_interface_type " interface_type" Type "Requ " CRU " Default " Valid " ABCDE
   image_name " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_mode " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_type " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   flavor " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   service_scaling " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   ordered_interfaces " service_template_properties" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " service-template" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   name " service-template" Type "Requ " CRU " Default " Valid " ABCDE
service-templates JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "service-template": {
           "display_name": "NFV2", 
           "fq_name": [
               "default-domain", 
               "NFV2"
           ], 
           "href": "http://127.0.0.1:8082/service-template/33a7ae4f-ddba-4839-89da-f18939278bbb", 
           "id_perms": {
               "created": "2014-12-03T01:56:43.466545", 
               "description": null, 
               "enable": true, 
               "last_modified": "2014-12-03T01:56:43.466545", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 9933517499790756795, 
                   "uuid_mslong": 3722135275090626617
               }
           }, 
           "name": "NFV2", 
           "parent_href": "http://127.0.0.1:8082/domain/11e2ba75-241a-435c-879d-0dcad6253169", 
           "parent_type": "domain", 
           "parent_uuid": "11e2ba75-241a-435c-879d-0dcad6253169", 
           "service_template_properties": {
               "availability_zone_enable": true, 
               "flavor": "m1.medium", 
               "image_name": "ubuntu", 
               "interface_type": [
                   {
                       "service_interface_type": "management", 
                       "shared_ip": false, 
                       "static_route_enable": false
                   }, 
                   {
                       "service_interface_type": "left", 
                       "shared_ip": true, 
                       "static_route_enable": false
                   }, 
                   {
                       "service_interface_type": "right", 
                       "shared_ip": true, 
                       "static_route_enable": false
                   }
               ], 
               "ordered_interfaces": true, 
               "service_mode": "in-network", 
               "service_scaling": true, 
               "service_type": "firewall"
           }, 
           "uuid": "33a7ae4f-ddba-4839-89da-f18939278bbb"
       }
   }

