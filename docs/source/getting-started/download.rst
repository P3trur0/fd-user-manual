
Download
========

Latest stable release (recommended)
-----------------------------------

This is the currently **RECOMMENDED** versions for most users. You can also try the latest dailybuild if you feel brave.

+--------------------------------------------------------------------------------------------------------------------------------+--------------+-----------+--------------+-------+
| Release                                                                                                                        | Java Version | Size (MB) | Release Date | Notes |
+=====================================+==========================================================================================+==============+===========+==============+=======+
| `Freedomotic Commander RC3 <https://sourceforge.net/projects/freedomotic/files/freedomotic-commander-5.6.0-rc3.zip/download>`_ | JRE 8+       | 45        | 1 Jul 2016   |       |
+--------------------------------------------------------------------------------------------------------------------------------+--------------+-----------+--------------+-------+
| `Freedomotic Commander RC2 <https://sourceforge.net/projects/freedomotic/files/freedomotic-commander-5.6.0-rc2.zip/download>`_ | JRE 8+       | 45        | 16 Nov 2015  |       |
+--------------------------------------------------------------------------------------------------------------------------------+--------------+-----------+--------------+-------+
| `Freedomotic Commander RC1 <https://sourceforge.net/projects/freedomotic/files/freedomotic-commander-5.6.0-rc1.zip/download>`_ | JRE 8+       | 45        | 17 Oct 2015  |       |
+--------------------------------------------------------------------------------------------------------------------------------+--------------+-----------+--------------+-------+
| `Freedomotic Bender 5.5.1 <https://sourceforge.net/projects/freedomotic/files/freedomotic-bender-5.5.1.zip/download>`_         | JRE 6+       | 44        | 11 Mar 2014  |       |
+--------------------------------------------------------------------------------------------------------------------------------+--------------+-----------+--------------+-------+

`Downloads statistics on Sourceforge <http://sourceforge.net/projects/freedomotic/files/stats/timeline>`_

Dailybuilds
-----------

These releases are created daily by our Continuous Integration System on Jetbrains Teamcity. Try one of them if you want to be on the bleeding edge of Freedomotic development.

**These releases are unstable** so don't use them in production environments.

`Download the latest available dailybuild (JRE 8+ required) <http://teamcity.jetbrains.com/guestAuth/repository/download/bt1177/.lastSuccessful/freedomotic-5.6.0-%7Bbuild.number%7D.zip>`_

.. note:: The dailybuilds are created and stored on an external host (teamcity.jetbrains.com). Sometimes it is down due to maintenance, we are sorry for the inconvenience, please be patient.

Docker container (experimental)
-------------------------------

For those of you willing to try Freedomotic dailybuild inside a Docker environment, we just created a demo container with some simple usage instructions.

Given you have Docker already installed on your machine you can start the container with the following instruction
 
.. code:: 
      
      docker run -d --name=freedomotic -p 9111:9111 -p 8090:8090 freedomotic/freedomotic
     

After a few seconds RESTapi interface will be available on port 9111 and the web client on port 8090 of the host machine. 
For tech details please go to https://hub.docker.com/r/freedomotic/freedomotic/.

.. note:: The latest version is mapped to [dailybuild] tag. If you want to try another version please specify the correct tag as in the following table. 

.. csv-table:: Docker images
   :header: "Tag", "Architecture", "Hw platforms", "Notes"
   :widths: 10, 30, 40, 20
   
   "latest","x86_64","","points to the last dailybuild"
   "dailybuild","x86_64","","unstable"
   "armhf","ARMv7","Raspberry Pi v1-2",""
   "arm64","ARMv8","Raspberry Pi v3, Odroid C2",""


On next days we'll try to test P2P feature in a Docker environment with (at least) two Freedomotic instances. 
If you think there may be more interesting usage scenarios for such containers, just share!

Debian packages
---------------


Old releases
------------

Do not use them. These are listed here just for historical reasons. No support will be provided for these versions.
