====================
virtual-machine
====================

 Put here  description of attribute 

virtual-machines Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   display_name " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_back_refs " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
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
   fq_name " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-machine" Type "Requ " CRU " Default " Valid " ABCDE
virtual-machines JSON
====

.. highlight:: json
   :linenothreshold: 5

::

   {
       "virtual-machine": {
           "display_name": "7a39517d-8f1c-4c3c-9b89-5fd055f20350", 
           "fq_name": [
               "7a39517d-8f1c-4c3c-9b89-5fd055f20350"
           ], 
           "href": "http://127.0.0.1:8082/virtual-machine/7a39517d-8f1c-4c3c-9b89-5fd055f20350", 
           "id_perms": {
               "created": "2015-01-21T12:16:38.913290", 
               "description": null, 
               "enable": true, 
               "last_modified": "2015-01-21T12:16:38.913290", 
               "permissions": {
                   "group": "cloud-admin-group", 
                   "group_access": 7, 
                   "other_access": 7, 
                   "owner": "cloud-admin", 
                   "owner_access": 7
               }, 
               "user_visible": true, 
               "uuid": {
                   "uuid_lslong": 11207594496087950160, 
                   "uuid_mslong": 8807160146013473852
               }
           }, 
           "name": "7a39517d-8f1c-4c3c-9b89-5fd055f20350", 
           "uuid": "7a39517d-8f1c-4c3c-9b89-5fd055f20350", 
           "virtual_machine_interface_back_refs": [
               {
                   "attr": null, 
                   "href": "http://127.0.0.1:8082/virtual-machine-interface/1ae35391-f7c3-4b80-9fdc-9963e6568c02", 
                   "to": [
                       "default-domain", 
                       "admin", 
                       "1ae35391-f7c3-4b80-9fdc-9963e6568c02"
                   ], 
                   "uuid": "1ae35391-f7c3-4b80-9fdc-9963e6568c02"
               }
           ]
       }
   }

