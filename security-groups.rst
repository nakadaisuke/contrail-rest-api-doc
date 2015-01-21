====================
security-group
====================

 Put here  description of attribute 

security-groups Attributes
====

.. csv-table::
   :header: Attribute, Parent, Type,Required,CRUD, Default Value, Validation Constraints, Notes
   :widths: 10, 10, 8, 3, 4, 9, 10, 20
   :delim: " 

   virtual_machine_interface_back_refs " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   to " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   href " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   attr " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " virtual_machine_interface_back_refs" Type "Requ " CRU " Default " Valid " ABCDE
   fq_name " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   access_control_lists " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   to " access_control_lists" Type "Requ " CRU " Default " Valid " ABCDE
   href " access_control_lists" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " access_control_lists" Type "Requ " CRU " Default " Valid " ABCDE
   parent_uuid " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   parent_href " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   parent_type " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   security_group_id " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   href " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   id_perms " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   enable " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_mslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   uuid_lslong " uuid" Type "Requ " CRU " Default " Valid " ABCDE
   created " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   user_visible " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   last_modified " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   permissions " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   owner " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   owner_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   other_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   group_access " permissions" Type "Requ " CRU " Default " Valid " ABCDE
   description " id_perms" Type "Requ " CRU " Default " Valid " ABCDE
   security_group_entries " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   policy_rule " security_group_entries" Type "Requ " CRU " Default " Valid " ABCDE
   direction " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   protocol " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   dst_addresses " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   security_group " dst_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   subnet " dst_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_network " dst_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   network_policy " dst_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   action_list " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   rule_uuid " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   dst_ports " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   end_port " dst_ports" Type "Requ " CRU " Default " Valid " ABCDE
   start_port " dst_ports" Type "Requ " CRU " Default " Valid " ABCDE
   application " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   src_addresses " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   security_group " src_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   subnet " src_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   virtual_network " src_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   network_policy " src_addresses" Type "Requ " CRU " Default " Valid " ABCDE
   rule_sequence " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   src_ports " policy_rule" Type "Requ " CRU " Default " Valid " ABCDE
   end_port " src_ports" Type "Requ " CRU " Default " Valid " ABCDE
   start_port " src_ports" Type "Requ " CRU " Default " Valid " ABCDE
   display_name " security-group" Type "Requ " CRU " Default " Valid " ABCDE
   name " security-group" Type "Requ " CRU " Default " Valid " ABCDE
security-groups JSON
====

.. highlight:: json
   :linenothreshold: 5

::