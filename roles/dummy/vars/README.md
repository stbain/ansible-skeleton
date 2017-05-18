# Role Variables Directory

The files in the vars directory are lower in the precedent chain but are considered internal to the role and essential for proper execution of the role. These are variables that the end user of the role shouldn't have to override except in rare cases. For example, having a rhel.yml vs. ubuntu.yml in this directory for an inclusion based on OS facts for specific Apache configuration locations.

Best practices
==============
* Namespace your variables by prefixing them with the role name. For example:
  * dummy_var1
  * dummy_var2
  * smarty_var1
  * smarty_var2
* Keep different environements in separate files. For example, have a different vars file for ec2 vs. azure or RHEL vs. Ubuntu.
