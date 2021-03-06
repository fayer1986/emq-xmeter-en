
.. _overview:

============
Test spec
============

--------
Tools
--------

`XMeter`_ Online performanct test service provider

`JMeter-MQTT`_ MQTT JMeter plugin

`JMeter`_ 3.0

`fusesource-1.14`_ MQTT client Java lib

--------
Test env
--------

EMQ version: `emqttd-ubuntu16.04-v2.0.zip`_

EMQ server: QingCloud 8 core CPU，28GB Memory，Ubuntu-16.04.1

Test agent：QingCloud 8 core CPU，8GB Memeory，CentOS 7

Network：Intranet of 3rd zone, Beijing QingCloud with 500Mbps.

-------------
Test scenario
-------------

The test includes concurrent connection test and message throughput test, totally 27 test scenarios. Please refer to related report for detailed test scenario. The concurrent connection test includes TCP, SSL and dual SSL, totally 9 test scenarios. Message throughput test includes multi-sub/few-pub, few-sub/multi-pub, capacity, shared-topic, message send/receive and latency test etc.

It could be a big test scenario combination, after considering test coverage and test result comparision etc, we designed the 27 test scenario. 

----------------
Read test report
----------------

There are some links to www.xmeter.net in the document, you can directly read the report online. These reports include some basic test measurements collected from client, the measurements provided by EMQ are already included in this doc. If you'd like to open the links, just register an account in www.xmeter.net with 1 step and then click them.

Please notice: Some of measurements in subscription report are not applicable because the JMeter sub plugin limitation when the performance test is executed at Dec, 2016. Only virtual user number, response code successful rate and download byte size are applicable. The latest new version of `JMeter-MQTT`_ MQTT JMeter plugin, which was released at Feb, 2017,  has fixed the problem. The response time and throughput measurements are also applicable, so we strongly recommend you to use latest JMeter MQTT plugin.

.. _XMeter: http://xmeter.net
.. _JMeter-MQTT: https://github.com/emqtt/mqtt-jmeter
.. _JMeter: http://jmeter.apache.org
.. _fusesource-1.14: https://github.com/fusesource/mqtt-client
.. _emqttd-ubuntu16.04-v2.0.zip: http://emqtt.com/downloads/2006/ubuntu16_04

