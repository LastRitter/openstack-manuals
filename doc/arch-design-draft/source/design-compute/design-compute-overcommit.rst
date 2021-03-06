==============
Overcommitting
==============

OpenStack allows you to overcommit CPU and RAM on compute nodes. This
allows you to increase the number of instances you can have running on
your cloud, at the cost of reducing the performance of the instances.
OpenStack Compute uses the following ratios by default:

* CPU allocation ratio: 16:1
* RAM allocation ratio: 1.5:1

The default CPU allocation ratio of 16:1 means that the scheduler
allocates up to 16 virtual cores per physical core. For example, if a
physical node has 12 cores, the scheduler sees 192 available virtual
cores. With typical flavor definitions of 4 virtual cores per instance,
this ratio would provide 48 instances on a physical node.

The formula for the number of virtual instances on a compute node is
``(OR*PC)/VC``, where:

OR
    CPU overcommit ratio (virtual cores per physical core)

PC
    Number of physical cores

VC
    Number of virtual cores per instance

Similarly, the default RAM allocation ratio of 1.5:1 means that the
scheduler allocates instances to a physical node as long as the total
amount of RAM associated with the instances is less than 1.5 times the
amount of RAM available on the physical node.

For example, if a physical node has 48 GB of RAM, the scheduler
allocates instances to that node until the sum of the RAM associated
with the instances reaches 72 GB (such as nine instances, in the case
where each instance has 8 GB of RAM).

.. note::
   Regardless of the overcommit ratio, an instance can not be placed
   on any physical node with fewer raw (pre-overcommit) resources than
   the instance flavor requires.

You must select the appropriate CPU and RAM allocation ratio for your
particular use case.

Logging
~~~~~~~

Logging is described in more detail in `Logging and Monitoring
<https://docs.openstack.org/ops-guide/ops-logging-monitoring.html>`_. However,
it is an important design consideration to take into account before
commencing operations of your cloud.

OpenStack produces a great deal of useful logging information, however,
for the information to be useful for operations purposes, you should
consider having a central logging server to send logs to, and a log
parsing/analysis system (such as logstash).

Networking
~~~~~~~~~~

Networking in OpenStack is a complex, multifaceted challenge. See
:doc:`../design-networking/design-networking-concepts`.
