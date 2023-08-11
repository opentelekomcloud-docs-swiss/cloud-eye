:original_name: en-us_topic_0084572213.html

.. _en-us_topic_0084572213:

Creating an Alarm Rule by Using an Alarm Template
=================================================

Cloud Eye allows you to use alarm templates to create alarm rules, making it easy and convenient to add or modify alarm rules for resources or cloud services, especially for a large number of resources and cloud services.

This topic describes how to use a default alarm template to create an alarm rule for a cloud service resource.

Creating an Alarm Rule
----------------------

#. Log in to the management console.
#. Click **Service List** in the upper left corner, and select **Cloud Eye**.
#. In the navigation pane on the left, choose **Alarm Management** > **Alarm Rules**.
#. Click **Create Alarm Rule** in the upper right corner.
#. On the **Create Alarm Rule** page, follow the prompts to configure the parameters.

   a. Select an object and configure other parameters listed in :ref:`Table 1 <en-us_topic_0084572213__table2902443185911>`. Click **Next**.

      .. note::

         You can search for ECSs by name, ID, and IP address. For other cloud services, you can search only by ID.

      .. _en-us_topic_0084572213__table2902443185911:

      .. table:: **Table 1** Parameters

         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Parameter                         | Description                                                                                                             |
         +===================================+=========================================================================================================================+
         | Name                              | Specifies the alarm rule name. The system generates a random name, which you can modify.                                |
         |                                   |                                                                                                                         |
         |                                   | Example value: **alarm-b6al**                                                                                           |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Description                       | (Optional) Provides supplementary information about the alarm rule.                                                     |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Resource Type                     | Specifies the type of the resource the alarm rule is created for.                                                       |
         |                                   |                                                                                                                         |
         |                                   | Example value: **Elastic Cloud Server**                                                                                 |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Dimension                         | Specifies the metric dimension of the selected resource type.                                                           |
         |                                   |                                                                                                                         |
         |                                   | Example value: **ECSs**                                                                                                 |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Monitoring Scope                  | Specifies the monitoring scope the alarm rule applies to. You can select **Resource groups** or **Specific resources**. |
         |                                   |                                                                                                                         |
         |                                   | .. note::                                                                                                               |
         |                                   |                                                                                                                         |
         |                                   |    -  If **Resource groups** is selected, an alarm is triggered when any resource in the group meets the alarm policy.  |
         |                                   |    -  If **Resource groups** is selected, alarm rules cannot be created using templates.                                |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+
         | Monitored Object                  | Specifies the resource the alarm rule is created for. You can specify one or more resources.                            |
         +-----------------------------------+-------------------------------------------------------------------------------------------------------------------------+

   b. If you select **Use template** for **Method**, you also need to specify the parameters listed in :ref:`Table 2 <en-us_topic_0084572213__table17310615145610>`.

      .. _en-us_topic_0084572213__table17310615145610:

      .. table:: **Table 2** Parameters

         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
         | Parameter                         | Description                                                                                                                           |
         +===================================+=======================================================================================================================================+
         | Method                            | Specifies the means you use to create the alarm rule.                                                                                 |
         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
         | Template                          | Specifies the template to be used.                                                                                                    |
         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
         | Alarm Notification                | Specifies whether to notify users when alarms are triggered. Notifications can be sent by email, text message, or HTTP/HTTPS message. |
         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
         | Validity Period                   | Cloud Eye sends notifications only within the validity period specified in the alarm rule.                                            |
         |                                   |                                                                                                                                       |
         |                                   | If **Validity Period** is set to **08:00-20:00**, Cloud Eye sends notifications only within 08:00-20:00.                              |
         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+
         | Trigger Condition                 | You can select **Generated alarm** (when an alarm is generated), **Cleared alarm** (when an alarm is cleared), or both.               |
         +-----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------+

After the alarm rule is created, if the metric data reaches the specified threshold, Cloud Eye immediately informs you that an exception has occurred.
