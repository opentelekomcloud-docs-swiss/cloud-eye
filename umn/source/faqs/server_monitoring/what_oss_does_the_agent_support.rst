:original_name: ces_faq_0024.html

.. _ces_faq_0024:

What OSs Does the Agent Support?
================================

The following table lists OSs compatible with the Agent. OSs not included in the table are being tested.

.. important::

   Using the OSs or versions that have not been verified may adversely affect your services. Exercise caution when using them.

:ref:`Table 1 <ces_faq_0024__en-us_topic_0079414514_en-us_topic_0077827618_table4718621518148>` lists the supported OSs.

.. _ces_faq_0024__en-us_topic_0079414514_en-us_topic_0077827618_table4718621518148:

.. table:: **Table 1** ECS versions supported

   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | OS (64 bit)                       | Version                                                                                      |
   +===================================+==============================================================================================+
   | CentOS                            | 6.3, 6.5, 6.8, 6.9, 7.1, 7.2, 7.3, 7.4, 7.5, 7.6                                             |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | OpenSUSE                          | 13.2, 42.2                                                                                   |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Debian                            | 7.5.0, 8.2.0, 8.8.0, 9.0.0                                                                   |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Ubuntu                            | 14.04 server, 16.04 server                                                                   |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | EulerOS                           | 2.2, 2.3                                                                                     |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | SUSE                              | Enterprise11 SP4, Enterprise12 SP1, Enterprise12 SP2                                         |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Fedora                            | 24, 25                                                                                       |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Oracle Linux                      | 6.9, 7.4                                                                                     |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | CoreOS                            | 10.10.5                                                                                      |
   |                                   |                                                                                              |
   |                                   | .. note::                                                                                    |
   |                                   |                                                                                              |
   |                                   |    Cloud-Init cannot be installed automatically. Install it manually in the **/** directory. |
   |                                   |                                                                                              |
   |                                   |    To query the Agent status, run **systemctl telescoped status**.                           |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Other                             | Gentoo Linux 13.0, Gentoo Linux 17.0                                                         |
   |                                   |                                                                                              |
   |                                   | .. note::                                                                                    |
   |                                   |                                                                                              |
   |                                   |    To query the Agent status, run **rc-service telescoped status**.                          |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Windows                           | Windows Server 2016 Standard 64-bit                                                          |
   |                                   |                                                                                              |
   |                                   | Windows Server 2016 Datacenter 64-bit                                                        |
   |                                   |                                                                                              |
   |                                   | Windows Server 2012 R2 Standard 64-bit                                                       |
   |                                   |                                                                                              |
   |                                   | Windows Server 2012 R2 Datacenter 64-bit                                                     |
   |                                   |                                                                                              |
   |                                   | Windows Server 2008 R2 Standard 64-bit                                                       |
   |                                   |                                                                                              |
   |                                   | Windows Server 2008 R2 Datacenter 64-bit                                                     |
   |                                   |                                                                                              |
   |                                   | Windows Server 2008 R2 Enterprise 64-bit                                                     |
   |                                   |                                                                                              |
   |                                   | Windows Server 2008 R2 Web 64-bit                                                            |
   +-----------------------------------+----------------------------------------------------------------------------------------------+
   | Arm general-computing             | CentOS 7.4 64bit with ARM (40 GB)                                                            |
   |                                   |                                                                                              |
   |                                   | CentOS 7.5 64bit with ARM (40 GB)                                                            |
   |                                   |                                                                                              |
   |                                   | CentOS 7.6 64bit with ARM (40 GB)                                                            |
   |                                   |                                                                                              |
   |                                   | EulerOS 2.8 64bit with ARM (40 GB)                                                           |
   |                                   |                                                                                              |
   |                                   | Fedora 29 64bit with ARM (40 GB)                                                             |
   |                                   |                                                                                              |
   |                                   | Ubuntu 18.04 64bit with ARM (40 GB)                                                          |
   +-----------------------------------+----------------------------------------------------------------------------------------------+

.. note::

   The GPU plug-in supports only Ubuntu 14.04 server and CentOS 7.3.
