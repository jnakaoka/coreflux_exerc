# coreflux_exerc
coreflux mqtt broker LOT exercise


# ⚠️ Current Overload Alert

# ⚡ Shelly Device Monitoring – High Current Alert

This LOT Notebook monitors current consumption of Shelly smart devices. If the current goes above `0.5A`, a high current alert is triggered and published to an alert topic.

## 📥 Model: ShellyDeviceStatus

This model listens for JSON messages from your Shelly devices under the pattern `ShellyDevice/<LampName>/status`.

💡 + is used as a wildcard to match any Shelly device name.

🚨 Action: High Current Alert
This action listens to the parsed model ShellyDeviceStatus and sends a warning if the current exceeds 0.5A.

# System Config
Action on every minute that defines the current treshold

links
https://marketplace.visualstudio.com/items?itemName=Coreflux.vscode-lot-notebooks

https://coreflux.org/

https://campus.coreflux.org/courses/take/lot-actions-basic/assignments/65763912-provide-a-public-github-link-with-a-simple-lot-notebook-that-includes