===========================
Next release: Ocata release
===========================

* The documentation sites ``developer.openstack.org`` and
  ``docs.openstack.org`` are now using ``https`` and links to
  pages have been changed to use ``https`` by default.

Administrator Guide
~~~~~~~~~~~~~~~~~~~

* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed. Legacy commands changed include ``nova``,
  ``neutron``, ``cinder``, ``glance``, and ``manila`` clients.
* Updated identity and compute content - PCI DSS v3.1 compliance, and Huge
  Page functionality, respectively.
* General bug fixes and updates.

API guides
~~~~~~~~~~

* Updated the landing page at
  `developer.openstack.org <https://developer.openstack.org/>`_ to point to
  development environments, "Writing your first OpenStack application,"
  and application reference architectures.

Command-Line Interface Reference
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed. Legacy commands changed include ``sahara``.

Configuration Reference
~~~~~~~~~~~~~~~~~~~~~~~

* Cleaned up content that is not directly configuration options.
* Created sections for newly added vendor plug-ins for Ocata.

Contributor Guide
~~~~~~~~~~~~~~~~~

* Added content about building documentation from end-of-life releases.
* General bug fixes and updates.

Deployment Guides
~~~~~~~~~~~~~~~~~

* Created new section for project-specific Deployment Guides (guides for
  using automated installation tools).
* OpenStack-Ansible Deployment guide created.

End User Guide
~~~~~~~~~~~~~~

* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed. Legacy commands changed include ``nova``,
  ``neutron``, ``cinder``, ``glance``, and ``manila`` clients.
* Deleted references to default flavors.
* Changes to swift content on ``.rlistings``, and  neutron dnsmasq log file
  content.

Installation Tutorials and Guides
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Updated landing page to improve ease of use.
* Deleted references to default flavors.
* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed.
* General bug fixes and updates.

Networking Guide
~~~~~~~~~~~~~~~~

* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed.
* Added routed provider networks.
* Added VLAN trunking.
* Added RFC 5737 and 3849 compliance policy.
* Improved Open vSwitch HA DVR deployment.
* Improved Quality of Service (QoS).
* Improved service subnets.
* Improved SR-IOV.
* Improved MTU considerations.
* Improved Load-Balancer-as-a-Service.

Operations Guide
~~~~~~~~~~~~~~~~

* Added links to upgrade documentation for nova, keystone, cinder, glance,
  swift, and ceilometer.
* General updates to the Upgrades chapter.
* Removed legacy commands in favor of the ``openstack`` client commands where
  equivalent functions existed.

Translations
~~~~~~~~~~~~

Besides updating the existing translated manuals,
the Internationalization (i18n) team added the following new manuals:

* German:
  * Published Installation Tutorials for Newton.
* Indonesian:
  * Published Installation Tutorials for Newton.
* Japanese:
  * Published High Availability Guide.
  * Published Installation Tutorials for Newton.
  * Published Operations Guide.
* Korean:
  * Published Installation Tutorials for Newton.
* Simplified Chinese:
  * Published End User Guide.
