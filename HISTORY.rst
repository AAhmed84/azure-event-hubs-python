.. :changelog:

Release History
===============

0.2.0rc1 (2018-07-06)
+++++++++++++++++++++

- **Breaking change** Restructured library to support Python 3.7. Submodule `async` has been renamed and all classes from
  this module can now be imported from azure.eventhub directly.
- **Breaking change** Removed optional `callback` argument from `Receiver.receive` and `AsyncReceiver.receive`.
- **Breaking change** `EventData.properties` has been renamed to `EventData.application_properties`.
  This removes the potential for messages to be processed via callback for not yet returned
  in the batch.
- Updated uAMQP dependency to v0.1.0
- Added support for constructing IoTHub connections.
- Fixed memory leak in receive operations.
- Dropped Python 2.7 wheel support.


0.2.0b2 (2018-05-29)
++++++++++++++++++++

- Added `namespace_suffix` to EventHubConfig() to support national clouds.
- Added `device_id` attribute to EventData to support IoT Hub use cases.
- Added message header to workaround service bug for PartitionKey support.
- Updated uAMQP dependency to vRC1.


0.2.0b1 (2018-04-20)
++++++++++++++++++++

- Updated uAMQP to latest version.
- Further testing and minor bug fixes.


0.2.0a2 (2018-04-02)
++++++++++++++++++++

- Updated uAQMP dependency.


0.2.0a1 (unreleased)
++++++++++++++++++++

- Swapped out Proton dependency for uAMQP.