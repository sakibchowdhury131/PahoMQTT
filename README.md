# PahoMQTT

A minimal MQTT publish/subscribe example using the [Eclipse Paho](https://www.eclipse.org/paho/) library. Includes both Python and C implementations.

## Overview

This repository provides starter scripts for connecting to an MQTT broker, publishing messages to a topic, and subscribing to receive them. Useful as a reference or boilerplate for IoT and home-automation projects.

## Files

| File | Description |
|------|-------------|
| `paho-mqtt-test-publish.py` | Python MQTT publisher — connects to broker and sends periodic messages |
| `paho-mqtt-test-subscribe.py` | Python MQTT subscriber — listens to a topic and prints received messages |
| `test.c` | C MQTT client example |

## Requirements

```
paho-mqtt>=1.6
```

Install with:

```bash
pip install paho-mqtt
```

## Configuration

Edit the broker settings at the top of each script:

```python
broker   = '192.168.1.4'   # MQTT broker IP
port     = 1883
topic    = "/sakib/test1"
username = 'your_username'
password = 'your_password'
```

## Usage

**Publish messages:**

```bash
python paho-mqtt-test-publish.py
```

**Subscribe to messages:**

```bash
python paho-mqtt-test-subscribe.py
```

## License

MIT
