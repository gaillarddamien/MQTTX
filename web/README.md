<img src="../assets/mqttx-logo.png" width="480" alt="MQTTX Logo" />

# MQTTX Web

[![GitHub Release](https://img.shields.io/github/release/emqx/mqttx?color=brightgreen)](https://github.com/emqx/mqttx/releases)
![build packages](https://github.com/emqx/MQTTX/workflows/build%20packages/badge.svg)
[![Total Downloads](https://img.shields.io/github/downloads/emqx/mqttx/total.svg)](https://github.com/emqx/mqttx/releases)
[![Docker](https://img.shields.io/docker/pulls/emqx/mqttx-web)](https://hub.docker.com/r/emqx/mqttx-web)
[![Slack](https://img.shields.io/badge/Slack-EMQX-39AE85?logo=slack)](https://slack-invite.emqx.io/) [![Discord](https://img.shields.io/discord/931086341838622751?label=Discord&logo=discord)](https://discord.gg/xYGf3fQnES)
[![Community](https://img.shields.io/badge/Community-MQTTX-yellow?logo=github)](https://github.com/emqx/MQTTX/discussions)
[![YouTube](https://img.shields.io/badge/Subscribe-EMQ-FF0000?logo=youtube)](https://www.youtube.com/channel/UC5FjR77ErAxvZENEWzQaO5Q)
[![Twitter](https://img.shields.io/badge/Follow-EMQ-1DA1F2?logo=twitter)](https://twitter.com/EMQTech)

---

[MQTTX Web](https://mqttx.app) is an open source MQTT 5.0 browser client and an online MQTT WebSocket client tool. Use WebSocket to connect to MQTT in your browser to help you develop and debug your MQTT services and applications faster without having to download and install MQTTX locally.

> [MQTT](https://mqtt.org/faq) stands for MQ Telemetry Transport. It is a publish/subscribe, extremely simple and lightweight messaging protocol, designed for constrained devices and low-bandwidth, high-latency or unreliable networks.

## Preview

![mqttx-preview](../assets/mqttx-web-preview.png)

## Documentation

For introduction, and usage, please refer to the [MQTTX Web Documentation](https://mqttx.app/docs/web).

## Usage

Visit MQTT WebSocket Client (MQTTX Web): [http://www.emqx.io/online-mqtt-client](http://www.emqx.io/online-mqtt-client)

## Deploy from Docker Image

```bash
docker pull emqx/mqttx-web:latest

docker run -d --name mqttx-web -p 80:80 emqx/mqttx-web:latest
```

## Better Together with EMQX

MQTTX is designed to connect to test MQTT Brokers such as EMQX, The one-click connection and simple graphical interface make it easy to connect to EMQX or EMQX Cloud to debug and explore functional features.

[Sign up EMQX Cloud for 14 days free trial](https://www.emqx.com/en/try?product=cloud)

[Download EMQX locally right now](https://www.emqx.com/en/try?product=enterprise)

## Get Involved

- Follow [@EMQTech on Twitter](https://twitter.com/EMQTech).
- If you have a specific question, check out our [discussion forums](https://github.com/emqx/emqx/discussions).
- For general discussions, join us on the [official Discord](https://discord.gg/xYGf3fQnES) team.
- Keep updated on [EMQX YouTube](https://www.youtube.com/channel/UC5FjR77ErAxvZENEWzQaO5Q) by subscribing.

## Develop

Recommended version for Node environment:

- v16.\*.\*

```shell
# Clone the repository
git clone git@github.com:emqx/MQTTX.git

# Install dependencies
cd MQTTX/web
yarn install

# Set Web app's title and description (customizable as per user requirements)
echo "VUE_APP_PAGE_TITLE=Easy-to-Use Online MQTT Client | Try Now" > .env.local
echo "VUE_APP_PAGE_DESCRIPTION=Online MQTT 5.0 client on the web, using MQTT over WebSocket to connect to the MQTT Broker and test message publishing and receiving in the browser." >> .env.local

# Compiles and hot-reloads for development
yarn run serve

# Compiles and minifies for production
yarn run build

# Compiles for production & serve generated files of site locally
yarn run start

# Compiles and prepares for Docker containerization
yarn run build:docker
```

## Contributing

Please make sure to read the [Contributing Guide](https://github.com/emqx/MQTTX/blob/main/.github/CONTRIBUTING.md) before making a pull request.

## Technology Stack

- [Vue](https://vuejs.org/) + [Element](https://element.eleme.io)
- [TypeScript](https://www.typescriptlang.org/)
- [MQTT.js](https://github.com/mqttjs/MQTT.js)

## License

Apache License 2.0, see [LICENSE](https://github.com/emqx/MQTTX/blob/main/LICENSE).
