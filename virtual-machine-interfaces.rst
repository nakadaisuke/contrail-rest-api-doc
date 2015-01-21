====================
virtual-machine-interface
====================

 Put here  description of attribute 

virtual-machine-interfaces Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   fq_name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_network_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_network_refs" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_machine_interface_mac_addresses " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   mac_address " virtual_machine_interface_mac_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   instance_ip_back_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " instance_ip_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   routing_instance_refs " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
   to " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   dst_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   protocol " attr" Type "Requ " CRU " Default " Valid " ABCDE
   direction " attr" Type "Requ " CRU " Default " Valid " ABCDE
   mpls_label " attr" Type "Requ " CRU " Default " Valid " ABCDE
   vlan_tag " attr" Type "Requ " CRU " Default " Valid " ABCDE
   src_mac " attr" Type "Requ " CRU " Default " Valid " ABCDE
   service_chain_address " attr" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " routing_instance_refs" Type "Requ " CRU " Default " Valid " ABCDE
   name " virtual-machine-interface" Type "Requ " CRU " Default " Valid " ABCDE
virtual-machine-interfaces JSON
====

.. highlight:: json
   :linenothreshold: 5

::