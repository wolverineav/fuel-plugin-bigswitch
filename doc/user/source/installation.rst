Installation
============

#. Download plugin .rpm package

#. Upload package to Fuel master node.

#. Install the plugin with *fuel* command line tool:

   .. code-block:: bash

    [root@nailgun ~] fuel plugins --install fuel-plugin-bigswitch-1.0-1.0.0-1.noarch.rpm


#. Verify that the plugin is installed successfully:

  .. code-block:: bash

    [root@nailgun ~] fuel plugins
    id | name                  | version | package_version
    ---|-----------------------|---------|----------------
    1  | fuel-plugin-bigswitch | 1.0.0   | 3.0.0

After installation plugin can be used for new OpenStack clusters, it is not
possible to enable plugin on deployed clusters.

Uninstallation
--------------

Before uninstalling plugin be sure that there no environments left that use the
plugin, otherwise it is not possible to uninstall it.

To uninstall plugin run following:

.. code-block:: bash

   [root@nailgun ~] fuel plugins --remove fuel-plugin-bigswitch==1.0.0

.. _Fuel plugin catalog: https://www.mirantis.com/products/openstack-drivers-and-plugins/fuel-plugins
