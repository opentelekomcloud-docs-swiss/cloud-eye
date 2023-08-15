:original_name: ces_01_0072.html

.. _ces_01_0072:

Adding Subscriptions
====================

Scenarios
---------

A topic is a channel used by SMN to broadcast messages. Therefore, after you create a topic, add subscriptions. In this way, when the metric triggers an alarm, Cloud Eye sends the alarm information to subscription endpoints of the topic.

Adding a Subscription
---------------------

#. Log in to the management console.

#. In the service list, select **Simple Message Notification**.

   The SMN console is displayed.

#. In the navigation tree on the left, choose **Topics**.

   The **Topics** page is displayed.

#. Click the topic name. The topic details are displayed.

#. On the **Subscriptions** tab, query the subscription list.

#. Click **Add Subscription** in the upper right of the subscription list.

   The **Add Subscription** page is displayed.

#. Specify the subscription protocol and endpoint.

   .. table:: **Table 1** Information required for adding a subscription

      +-----------------------------------+--------------------------------------------------------------------------------------------------------------------+
      | Parameter                         | Description                                                                                                        |
      +===================================+====================================================================================================================+
      | Topic Name                        | Provides the name of the topic to be subscribed to, which cannot be changed.                                       |
      +-----------------------------------+--------------------------------------------------------------------------------------------------------------------+
      | Protocol                          | Specifies the protocol the subscription endpoint supports.                                                         |
      |                                   |                                                                                                                    |
      |                                   | The available options include **SMS**, **Email**, **HTTP**, and **HTTPS**.                                         |
      +-----------------------------------+--------------------------------------------------------------------------------------------------------------------+
      | Endpoint                          | Specifies the subscription endpoint. You can enter up to 10 endpoints, with every two separated with a line break. |
      |                                   |                                                                                                                    |
      |                                   | -  **SMS**: Enter one or more phone numbers.                                                                       |
      |                                   |                                                                                                                    |
      |                                   |    The phone number must be preceded by a plus sign (+) and the country code.                                      |
      |                                   |                                                                                                                    |
      |                                   |    For example:                                                                                                    |
      |                                   |                                                                                                                    |
      |                                   |    **+8600000000000**                                                                                              |
      |                                   |                                                                                                                    |
      |                                   |    **+8600000000001**                                                                                              |
      |                                   |                                                                                                                    |
      |                                   | -  **Email**: Enter one or more email addresses.                                                                   |
      |                                   |                                                                                                                    |
      |                                   |    For example:                                                                                                    |
      |                                   |                                                                                                                    |
      |                                   |    **username@example.com**                                                                                        |
      |                                   |                                                                                                                    |
      |                                   |    **username2@example.com**                                                                                       |
      |                                   |                                                                                                                    |
      |                                   | -  **HTTP** or **HTTPS**: Enter one or more public network URLs.                                                   |
      |                                   |                                                                                                                    |
      |                                   |    For example:                                                                                                    |
      |                                   |                                                                                                                    |
      |                                   |    **http://example.com/notification/action**                                                                      |
      |                                   |                                                                                                                    |
      |                                   |    **http://example2.com/notification/action**                                                                     |
      +-----------------------------------+--------------------------------------------------------------------------------------------------------------------+

#. Click **OK**.

   The subscription you added is displayed in the subscription list. SMN automatically sends a confirmation message to the subscription endpoint, and the subscriber must confirm the subscription within 48 hours so that they can receive notification messages. Otherwise, you need to send a new confirmation message to the subscriber.
