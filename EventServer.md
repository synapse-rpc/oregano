# Event Server Protocol

## The Event Server use a queue name:

> SysName + "\_event\_" + AppName

## The Event Server use routing key like:

> "event." + EventName

## The Event Server Consumer name:

> SysName + "." + AppName + ".event." + AppId

## Event Server System Flow

1. Event Server listen to this queue first
2. Event Server bind routing key to queue
3. Event Server create a consumer for events
4. listen the message
5. when receive the message , use the callback to process message
6. if event process success , ack the messge. other,reject the message