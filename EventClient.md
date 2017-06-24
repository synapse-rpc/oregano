# Event Client Protocol

## The Event Server use routing key like:

> "event." + AppName + "." + eventName

## JSON format:

```json
{
"from":"AppName + AppId",
"to":"event",
"action": "EventName",
"params": "PARAMS JSON STRING"
}
```

## System Flow

1. publish a message to the exchange use routing key