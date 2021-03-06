This repository contains the cloud administrator documentation for the 
OpenStack project. It includes documentation for OpenStack Compute, OpenStack
Identity Service, OpenStack Image Service, and OpenStack Object Storage as
well as the Dashboard.

For more details, see the `OpenStack Documentation HowTo wiki page
<http://wiki.openstack.org/Documentation/HowTo>`_.

Prereqs
=======
`Apache Maven <http://maven.apache.org/>`_ must be installed to build the
documentation.

Building
========
To build the Compute Admin Manual, Object Storage Admin Manual, and Image
Service Manual::

    cd openstack-manuals/doc
    mvn clean generate-sources

The different manuals are in subdirectories of the
``openstack-manuals/doc/src/docbkx`` directory. For example, the root
directory of the `OpenStack Compute Administration Guide` is
``openstack-manuals/doc/src/docbkx/openstack-compute-admin``.

To build a specific guide, look for a pom.xml file within a subdirectory, then
run the mvn command in that directory. For example::

    cd openstack-manuals/doc/src/docbkx/openstack-compute-admin
    mvn clean generate-sources

The generated PDF documentation file is::

    openstack-manuals/doc/src/docbkx/openstack-compute-admin/target/docbkx/webhelp/trunk/openstack-compute/admin/os-compute-adminguide-trunk.pdf

The root of the generated HTML documentation is::

    openstack-manuals/doc/src/docbkx/openstack-compute-admin/target/docbkx/webhelp/os-compute-adminguide/content/index.html

Contributing
============
Our community welcomes all people interested in open source cloud computing,
and there are no formal membership requirements. The best way to join the
community is to talk with others online or at a meetup and offer contributions
through Launchpad, the OpenStack wiki, or blogs. We welcome all types of
contributions, from blueprint designs to documentation to testing to 
deployment scripts.

Installing
==========
Refer to http://docs.openstack.org to see where these documents are published
and to learn more about the OpenStack project.
