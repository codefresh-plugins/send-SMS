# Codefresh plugin for send SMS notification

Codefresh plugin for send SMS notification via Twilio

## Main env variables
- `TWILIO_SID`
- `TWILIO_TOKEN`
- `TWILIO_PHONE_FROM`
- `TWILIO_PHONE_TO`
- `TWILIO_TYPE` - type of message [build, message, hello]

For **message** type you must provide `TWILIO_MESSAGE` env

## Config for codefresh.yml
```
version: '1.0'
...
steps:
  ...
  TestSMS:
    title: Test SMS
    image: potterua/twilioplugincodefresh:latest
  ...
...
```
