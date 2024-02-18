<div align="center">
    <a href="https://github.com/zigbee2mqtt/hassio-zigbee2mqtt">
        <img width="150" height="150" src="zigbee2mqtt/logo.png">
    </a>
    <br>
    <br>
    <div style="display: flex;">
        <a href="https://github.com/zigbee2mqtt/hassio-zigbee2mqtt/actions?query=workflow%3ACI">
            <img src="https://github.com/zigbee2mqtt/hassio-zigbee2mqtt/workflows/CI/badge.svg">
        </a>
        <a href="https://github.com/zigbee2mqtt/hassio-zigbee2mqtt/releases">
            <img src="https://img.shields.io/github/release/zigbee2mqtt/hassio-zigbee2mqtt.svg">
        </a>
        <a href="https://github.com/zigbee2mqtt/hassio-zigbee2mqtt/stargazers">
            <img src="https://img.shields.io/github/stars/zigbee2mqtt/hassio-zigbee2mqtt.svg">
        </a>
        <a href="https://discord.gg/dadfWYE">
            <img src="https://img.shields.io/discord/556563650429583360.svg">
        </a>
        <a href="http://zigbee2mqtt.discourse.group/">
            <img src="https://img.shields.io/discourse/https/zigbee2mqtt.discourse.group/status.svg">
        </a>
    </div>
    <h1>Official Zigbee2MQTT Home Assistant addon</h1>
</div>

## Info
homeassistant: true  
advanced:
  channel: 20 #信道修改成 15 20 25
mqtt:
  server: mqtt://localhost:1883 #mqtt设置  #(localhost=ha安装Mosquitto的局域网地址)
  base_topic: zigbee2mqtt2   #base_topic多加一个2 以此类推
  user: mqtt
  password: mqtt
  client_id: zigbee2mqtt2 #client_id多加一个2 以此类推
frontend:
  port: 8099
serial:
  port: tcp://localhost:端口号 #网关设置  #(localhost=网关局域网地址)企业版+多模旧版端口8888,多模自动版端口6638
  adapter: ezsp
