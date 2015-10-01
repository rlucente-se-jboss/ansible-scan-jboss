ansible-scan-jboss
==================

[Ansible](http://ansible.com) is a configuration management tool that
enables running modules on remote systems without the need for remote
agent infrastructure.

For more information, see the [Ansible web site](http://ansible.com).

This Ansible module scans for deployed JBoss instances by searching
for the jboss-modules.jar and run.jar files and then extracts the
version from the pom.properties and MANIFEST.MF, respectively, to
determine which distribution contained the jar.

NB:  This script is up to date through EAP 6.4 CP03 and WildFly 10.0.0.Beta2.

This has now been updated with a python script in addition to a
bash script.  The python script correctly works on both Linux and
Mac OSX, but it has not yet been tested with Microsoft Windows.
Also, the python script needs to be reviewed to ensure it matches
ansible expectations.  The ["Ansible Configuration Management" book](http://www.packtpub.com/ansible-configuration-management/book)
is a good resource for this.

