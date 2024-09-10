:original_name: ces_01_0071.html

.. _ces_01_0071:

Creating a Topic
================

Scenarios
---------

A topic is a specified event to publish messages and subscribe to notifications. It serves as a message sending channel, where publishers and subscribers can interact with each other.


Creating a Topic
----------------

#. Log in to the management console.

#. Click |image1| on the upper left to select the desired region and project.

#. In the service list, select **Simple Message Notification**.

   The SMN console is displayed.

#. In the navigation pane, choose **Topics**.

   The **Topics** page is displayed.

#. In the upper right corner, click **Create Topic**.


   .. figure:: /_static/images/en-us_image_0000001614235704.png
      :alt: **Figure 1** Create Topic

      **Figure 1** Create Topic

#. Enter a topic name and display name.

   .. table:: **Table 1** Information required for creating a topic

      +-----------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
      | Parameter                         | Description                                                                                                                                                                                         |
      +===================================+=====================================================================================================================================================================================================+
      | Topic Name                        | Topic name, which:                                                                                                                                                                                  |
      |                                   |                                                                                                                                                                                                     |
      |                                   | -  Contains only letters, digits, hyphens (-), and underscores (_), and must start with a letter or digit.                                                                                          |
      |                                   | -  Contain 1 to 255 characters.                                                                                                                                                                     |
      |                                   | -  Must be unique and cannot be modified once the topic is created.                                                                                                                                 |
      +-----------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
      | Display Name                      | Message sender name, which must be fewer than 192 characters.                                                                                                                                       |
      |                                   |                                                                                                                                                                                                     |
      |                                   | .. note::                                                                                                                                                                                           |
      |                                   |                                                                                                                                                                                                     |
      |                                   |    After you specify a display name, the sender in email messages will be presented as *Display name*\ **<username@example.com>**. Otherwise, the sender will be **username@example.com**.          |
      +-----------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
      | Tag                               | Tags consist of keys and values. They identify cloud resources so that you can easily categorize and search for your resources.                                                                     |
      |                                   |                                                                                                                                                                                                     |
      |                                   | -  A key or value can contain letters, digits, and special characters -_@ and cannot start or end with a space. A key can contain up to 36 characters, and a value can contain up to 43 characters. |
      |                                   | -  You can add up to 10 tags for each topic.                                                                                                                                                        |
      +-----------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

#. Click **OK.**

   The topic you created is displayed in the topic list. The system generates a topic URN, which is the unique resource identifier of the topic and cannot be changed.

#. Click the name of the topic to view its details, including the URN, display name, and subscriptions.

.. |image1| image:: /_static/images/en-us_image_0000001662155781.png
