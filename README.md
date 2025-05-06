# Home-Assistant-Universal-TCP-Server-Integration
This custom integration creates a TCP socket server in Home Assistant that can control and monitor various smart devices over a local network (LAN), without requiring MQTT or cloud services.
Supported Devices:
✅ Lights (on/off, brightness)

✅ Switches / Relays

✅ Air Conditioners (mode, temperature)

✅ Fans (on/off, speed control)

✅ Smart Locks

✅ Keypads (e.g., for triggering automations)

🚀 Key Features:
Runs a TCP server directly from Home Assistant.

Supports dynamic registration of devices.

Bi-directional communication: receive status updates and send control commands.

Flexible message format (e.g., JSON).

Clean and modular Python structure (custom component).

Works entirely offline (no internet or cloud required).

Easy to extend for new device types.

📦 Installation:
Copy this repo into your custom_components/ directory:

swift
Copy
Edit
/config/custom_components/tcp_devices/
Restart Home Assistant.

Configure via configuration.yaml or UI (if supported).

Ensure your smart devices are configured to send/receive data via TCP to the server's IP and port.

📨 Example TCP Payloads:
json
Copy
Edit
{ "device": "fan_1", "command": "turn_on", "speed": "medium" }
{ "device": "ac_living", "mode": "cool", "temperature": 24 }
{ "device": "lock_main_door", "command": "unlock" }
📘 Use Cases:
Custom smart home systems using LAN communication.

Offline/air-gapped smart homes.

Smart device hubs that use TCP/IP (vs MQTT or HTTP).

Industrial automation with local network control.

🤝 About Me
I’m a Computer Science student at Nirma University, with experience building advanced Home Assistant custom integrations using Python, MQTT, and TCP.

I'm open to collaboration, contributions, or freelance projects related to this and other smart home automations.

