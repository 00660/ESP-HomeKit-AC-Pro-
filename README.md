# ❄️ Universal AC HomeKit Bridge Pro

> **可能是目前功能最全、体验最好的 ESP8266 空调红外改机固件。**
> **Probably the most advanced ESP8266 IR AC firmware with native HomeKit support.**

![PlatformIO](https://img.shields.io/badge/Platform-PlatformIO-orange)
![ESP8266](https://img.shields.io/badge/Device-ESP8266-red)
![HomeKit](https://img.shields.io/badge/Support-Native%20HomeKit-blue)
![License](https://img.shields.io/badge/license-MIT-green)

将你的普通空调瞬间变成 **Apple HomeKit** 智能家电。无需 HomeBridge，无需服务器，直接直连！支持网页配置、MQTT、OTA 升级以及独家的 Bark 配对码推送功能。

Turn your dumb AC into a smart **Apple HomeKit** device instantly. No HomeBridge required. Features Web UI, MQTT, OTA updates, and unique Bark notification for pairing codes.

## ✨ 核心特性 / Key Features

### 🚀 独家增强功能 (Pro Features)
*   **🍎 原生 HomeKit 支持**: 彻底修复了常见的“模式错乱”问题（制冷/自动/制热逻辑完美映射）。
*   **💨 风速控制 (Fan Speed)**: 独家支持在 HomeKit 中调节风速（0% 自动，1-33% 低，34-66% 中，67-100% 高）。
*   **📱 Bark 自动推送**: 设备启动时，根据 MAC 地址自动生成唯一配对码，并推送到你的 iPhone (Bark App)，再也不怕忘记配对码。
*   **🔄 动态协议切换**: 支持格力、美的、海尔、大金等 15+ 主流品牌，**网页端一键切换**，无需重新编译固件。
*   **🔌 GPIO 动态配置**: 可以在网页端自定义 IR 发射脚、LED 脚和 Reset 脚，兼容各种 ESP8266 开发板。

### 🛠️ 基础功能 (Basic Features)
*   **Web 控制台**: 漂亮的响应式网页界面，支持手机操作。
*   **MQTT 集成**: 完美接入 Home Assistant。
*   **WiFi 配网**: 首次启动进入 AP 模式，手机连接即可配置 WiFi。
*   **OTA 升级**: 支持网页端上传 `.bin` 文件升级固件。
*   **状态同步**: 红外遥控器、网页、HomeKit、MQTT 状态四向实时同步。

---

## 📸 截图 / Screenshots

*(建议在此处放 3 张图：1. 网页控制台界面 2. HomeKit 空调控制界面 3. Bark 推送通知截图)*

| Web UI | HomeKit Control | Bark Notification |
| :---: | :---: | :---: |
| ![WebUI](path/to/screenshot1.png) | ![HK](path/to/screenshot2.png) | ![Bark](path/to/screenshot3.png) |

---

## 📋 支持品牌 / Supported Brands

目前支持以下品牌（可在网页端直接切换）：

*   **Gree (格力)**
*   **Midea (美的)**
*   **Haier (海尔)**
*   **Daikin (大金)**
*   **Mitsubishi (三菱电机 & 重工)**
*   **Toshiba (东芝)**
*   **Panasonic (松下)**
*   **Fujitsu (富士通)**
*   **Samsung (三星)**
*   **LG**
*   **Hitachi (日立)**
*   **TCL**
*   **AUX (奥克斯)**
*   **Coolix (通用协议)**

---

## 🛠️ 硬件准备 / Hardware

1.  **ESP8266 开发板**: NodeMCU v3, Wemos D1 Mini, 或 ESP-01S。
2.  **红外发射管**: 连接到 GPIO (默认 D5/GPIO14)。
3.  **红外接收管 (可选)**: 用于学习遥控器状态（本项目主要为发射）。
