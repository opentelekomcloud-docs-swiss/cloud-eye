:original_name: en-us_topic_0015479882.html

.. _en-us_topic_0015479882:

What Is Cloud Eye?
==================

Cloud Eye is a multi-dimensional resource monitoring service. You can use Cloud Eye to monitor resources, set alarm rules, identify resource exceptions, and quickly respond to resource changes. :ref:`Figure 1 <en-us_topic_0015479882__fig1135112504519>` shows the Cloud Eye architecture.

.. _en-us_topic_0015479882__fig1135112504519:

.. figure:: /_static/images/en-us_image_0000001614075552.png
   :alt: **Figure 1** Cloud Eye architecture

   **Figure 1** Cloud Eye architecture

Cloud Eye provides the following functions:

-  Automatic monitoring

   Monitoring starts automatically after you created resources such as Elastic Cloud Servers (ECSs). On the Cloud Eye console, you can view the service status and set alarm rules for these resources.

-  Flexible alarm rule configuration

   You can create alarm rules for multiple resources at the same time. After you create an alarm rule, you can modify, enable, disable, or delete it at any time.

-  Real-time notification

   You can enable **Alarm Notification** when creating alarm rules. When the cloud service status changes and metrics reach the thresholds specified in alarm rules, Cloud Eye notifies you by SMS messages, emails, or by sending messages to server addresses, allowing you to monitor the cloud resource status and changes in real time.

-  Monitoring panel

   The panel enables you to view cross-service and cross-dimension monitoring data. It displays key metrics, providing an overview of the service status and monitoring details that you can use for troubleshooting.

-  Resource group

   A resource group allows you to add and monitor correlated resources and provides a collective health status for all resources that it contains.

-  Event monitoring

   You can query system events that are automatically reported to Cloud Eye and custom events reported to Cloud Eye through the API. You can create alarm rules for both system events and custom events. When specific events occur, Cloud Eye generates alarms for you.
