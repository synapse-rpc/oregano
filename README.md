# Synapse Documents

This system is based on RabbitMQ, all components will connect the queue, and exchange data on the queue.

The components make communications use json with RabbitMQ.

## Common Parameters

> If the parameter have default value, it isn't a required parameter.

param|type|default|description
----|----|----|----
MqHost|string|-|RabbitMQ Host Address
MqPort|int|-|RabbitMQ Host port
MqUser|string|-|RabbitMQ User
MqPass|string|-|RabbitMQ Password
SysName|string|-|Same SysName can communication
AppName|string|-|App Name for Component
AppId|string|random string|Only Id for app
RpcTimeout|int|60|Thread timeout for process request
ProcessNum|int|10|Thread numbers for process request
DisableEventClient|bool|false|Event Client Switch
DisableRpcClient|bool|false|Rpc Client Switch
Debug|bool|false|Debug Mode Switch

## Communication Protocol

1. [EventServer](https://github.com/synapse-rpc/synapse/blob/master/EventServer.md)
2. [EventClient](https://github.com/synapse-rpc/synapse/blob/master/EventClient.md)
3. [RpcServer](https://github.com/synapse-rpc/synapse/blob/master/RpcServer.md)
4. [RpcClient](https://github.com/synapse-rpc/synapse/blob/master/RpcClient.md)