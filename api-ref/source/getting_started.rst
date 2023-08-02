:original_name: ces_03_0014.html

.. _ces_03_0014:

Getting Started
===============

Overview
--------

This topic describes how to invoke a number of Cloud Eye APIs to create an alarm rule for the ECS CPU usage.

.. note::

   The validity period of a token obtained from IAM is 24 hours. If you want to use a token for authentication, cache it to avoid frequently calling the IAM API.

Procedure
---------

#. .. _ces_03_0014__li13561185565518:

   Obtain the token by referring to :ref:`Authentication <ces_03_0011>`.

#. Query the list of metrics that can be monitored.

   Send **GET https://**\ *Cloud Eye endpoint*\ **/V1.0/{project_id}/metrics**.

   Add **X-Auth-Token** obtained in :ref:`1 <ces_03_0014__li13561185565518>` to the request header.

   After the request is successfully responded, the **metrics** information is returned, such as **"metric_name":** **"cpu_util"** in the following figure.

   .. code-block::

      {
          "metrics": [
              {
                  "namespace": "SYS.ECS",
                  "dimensions": [
                      {
                          "name": "instance_id",
                          "value": "d9112af5-6913-4f3b-bd0a-3f96711e004d"
                      }
                  ],
                  "metric_name": "cpu_util",
                  "unit": "%"
              }
          ],
          "meta_data": {
              "count": 1,
              "marker": "SYS.ECS.cpu_util.instance_id:d9112af5-6913-4f3b-bd0a-3f96711e004d",
              "total": 7
          }
      }

   If the request fails, an error code and error information are returned. For details, see :ref:`Error Codes <errorcode>`.

#. .. _ces_03_0014__li15628194054711:

   Create an alarm rule.

   Send **POST https://**\ *Cloud Eye endpoint*\ **/V1.0/{project_id}/alarms**.

   Specify the following parameters in the request body:

   .. code-block::

      {
          "alarm_name": "alarm-rp0E",  //Alarm rule name (mandatory, string)
          "alarm_description": "",
          "metric": {
              "namespace": "SYS.ECS",  //Namespace (mandatory, string)
              "dimensions": [
                  {
                      "name": "instance_id",
                      "value": "33328f02-3814-422e-b688-bfdba93d4051"
                  }
              ],
              "metric_name": "cpu_util"   //Metric name (mandatory, string)
          },
          "condition": {
              "period": 300,      //Monitoring period (mandatory, integer)
              "filter": "average",     //Data rollup method (mandatory, string)
              "comparison_operator": ">=",    //Operator of the alarm threshold (mandatory, string)
              "value": 80, //Threshold (mandatory, string)
              "unit": "%",  //Data unit (mandatory, string)
              "count": 1
          },
          "alarm_enabled": true,
          "alarm_action_enabled": true,
          "alarm_level": 2,
          "alarm_actions": [
              {
                  "type": "notification",
                  "notificationList": [ ]
              }
          ],
          "ok_actions": [
              {
                  "type": "notification",
                  "notificationList": [ ]
              }
          ]
      }

   If the request is responded, the alarm rule ID is returned.

   .. code-block::

      {
          "alarm_id":"al1450321795427dR8p5mQBo"
      }

   If the request fails, an error code and error information are returned. For details, see :ref:`Error Codes <errorcode>`.

   You can query, enable, disable, or delete alarm rules based on the alarm rule ID obtained in :ref:`3 <ces_03_0014__li15628194054711>`.
