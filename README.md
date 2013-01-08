# Overview

This charm provides joomla from http://www.joomla.org. Joomla is an award-winning content management system (CMS), which enables you to build Web sites and powerful online applications.

# Installation

To install this charm you should schedule the following juju actions:

    juju deploy mysql
    juju deploy joomla

You can then add a relation between joomla and mysql with:

    juju add-relation joomla mysql

Finally you need to expose your joomla instance:

    juju expose joomla

Note that the mysql reation addition will create the database and populated it with the admin user. The default password for the admin user is 123. Make sure you change IMMEDIATELY after installing. Failure to do so may have others change your website without your consent.

You may change the admin password and perform other administrative functions at the exposed service URL http://public-ip-address/administrator

# Configuration

None at this time.

TODO: Add configuration options. The most important one being the admin password.

# Contact Information

Author:
Report bugs at: http://bugs.launchpad.net/charms/+source/joomla
Location: http://jujucharms.com/charms/precise/joomla
