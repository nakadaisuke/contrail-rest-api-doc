====================
virtual-router
====================

 Put here  description of attribute 

virtual-routers Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_router_type " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_router_ip_address " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   physical_router_back_refs " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   to " physical_router_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " physical_router_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " physical_router_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " physical_router_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
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
   name " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_refs " virtual-router" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_refs" Type "Requ " CRU " Default " Valid " ABCDE

virtual-routers JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-router": {
           "display_name": "system003-1", 
           "fq_name": [
               "default-global-system-config", 
               "system003-1"
           ], 
           "href": "http://127.0.0.1:8082/virtual-router/2e25cd0e-b0f0-4fc4-868e-c188a502d950", 
           "id_perms": {
               "created": "2014-11-25T09:16:19.869944", 
               "description": null, 
               "enable": true, 
               "last_modified": "2014-11-25T09:16:19.869944", 
               "permissions": {
                   "group": "admin", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 9695899840403396944, 
                   "uuid_mslong": 3325289362864754628
               }
           }, 
           "name": "system003-1", 
           "parent_href": "http://127.0.0.1:8082/global-system-config/ee6b566c-3d5b-43d2-bd3e-a86bb3b7779b", 
           "parent_type": "global-system-config", 
           "parent_uuid": "ee6b566c-3d5b-43d2-bd3e-a86bb3b7779b", 
           "physical_router_back_refs": [
               {
                   "attr": null, 
                   "href": "http://127.0.0.1:8082/physical-router/703ecc26-73ad-4ba9-8380-c2b4beff1b70", 
                   "to": [
                       "default-global-system-config", 
                       "fuda"
                   ], 
                   "uuid": "703ecc26-73ad-4ba9-8380-c2b4beff1b70"
               }
           ], 
           "uuid": "2e25cd0e-b0f0-4fc4-868e-c188a502d950", 
           "virtual_machine_refs": [
               {
                   "attr": null, 
                   "href": "http://127.0.0.1:8082/virtual-machine/76187277-7b08-4d07-b879-21d5ba32beaf", 
                   "to": [
                       "default-domain__admin__9bdadf31-ff39-4c8b-9940-e679d93a2214__2"
                   ], 
                   "uuid": "76187277-7b08-4d07-b879-21d5ba32beaf"
               }
           ], 
           "virtual_router_ip_address": "10.84.50.3", 
           "virtual_router_type": [
               "tor-agent"
           ]
       }
   }

