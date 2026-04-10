# Surge Rule-Sets

## 🚀 Project Overview

`surge-rulesets` is a meticulously maintained collection of rule-sets for the Surge proxy tool. It aims to provide users with efficient, stable, and feature-rich network proxy configurations. This repository covers various aspects such as ad blocking, optimization for specific country/region services, and privacy protection, helping users better manage network traffic and enhance their online experience.

## ✨ Key Features

*   **Ad and Tracker Blocking**: Effectively blocks various advertisements, malicious trackers, and potentially harmful domains, offering a cleaner browsing environment.
*   **Service Optimization**: Optimized for specific applications and services (e.g., Apple services, Microsoft services) to ensure stable operation and optimal performance.
*   **Geo-Routing**: Provides traffic splitting rules for different countries/regions, such as `china.list` for accelerating access to Chinese services and `us.list` for accessing US services.
*   **Easy Integration**: Rule files are designed to be simple and can be easily imported into Surge and other compatible proxy tools.
*   **Continuous Updates**: The rule-sets are regularly maintained and updated to adapt to the ever-changing network environment and application requirements.

## 📦 Rule File List

This repository includes the following main rule files:

| Filename           | Description                                     | Purpose                                       |
| :--------------- | :---------------------------------------------- | :-------------------------------------------- |
| `adblock.list`   | Ad blocking rules                               | Blocks ads, trackers, and malicious domains    |
| `apple.list`     | Apple services optimization rules               | Ensures normal operation of Apple official services, iCloud, App Store |
| `bytedance.list` | ByteDance services optimization rules           | Optimizes access to ByteDance apps like Douyin, TikTok |
| `china.list`     | China mainland services direct connection rules | Optimizes access to China, ensuring direct traffic for mainland services |
| `malaysia.list`  | Malaysia services optimization rules            | Optimizes network service access for the Malaysia region |
| `microsoft.list` | Microsoft services optimization rules           | Ensures normal operation of Microsoft official services, Office 365 |
| `porn.list`      | Adult content blocking rules                    | Blocks adult websites and related content     |
| `us.list`        | US services optimization rules                  | Optimizes network service access for the US region |
| `BackCN.conf`    | Comprehensive China-access configuration (Surge Config) | Complete Surge configuration for accessing Chinese services |

## 🛠️ How to Use

### 1. Import Rule-Sets

You can choose to import individual rule files or import `BackCN.conf` into Surge as a complete configuration.

**Method One: Import Individual Rule Files (Recommended)**

In your Surge configuration, you can reference the rule files from this repository using the `RULE-SET` syntax. For example, to import `adblock.list`, add the following to your `[Rule]` section:

```ini
RULE-SET,https://cdn.jsdelivr.net/gh/SantaG3225/surge-rulesets@main/adblock.list,REJECT
```

Please replace `adblock.list` with the name of the rule file you wish to import, and adjust the policy (e.g., `DIRECT`, `PROXY`, `REJECT`) as needed.

**Method Two: Import `BackCN.conf` (Complete Configuration)**

`BackCN.conf` is a complete Surge configuration file that includes all necessary rules and configurations for accessing Chinese services. You can directly import it as your Surge configuration.

1.  Copy the raw link for `BackCN.conf`: `https://cdn.jsdelivr.net/gh/SantaG3225/surge-rulesets@main/BackCN.conf`
2.  In the Surge application, go to "Configuration" -> "Download Configuration from URL", then paste the link and import.

### 2. Update Rule-Sets

To ensure the timeliness of the rule-sets, it is recommended to update them regularly. If you import rule-sets via URL, Surge usually checks for updates automatically. You can also manually trigger updates within the Surge application.

## 🤝 Contribution

We welcome contributions from community members to this rule-set! If you find any rules are invalid, have new rule suggestions, or wish to improve existing rules, please participate through the following methods:

1.  **Submit an Issue**: Report problems or suggest improvements.
2.  **Submit a Pull Request**: Directly modify rule files and submit them.

Before submitting a Pull Request, please ensure your changes conform to the existing rule format and include a brief description.

## 📜 License

All rule-sets in this repository are open-sourced under the [MIT License](https://github.com/SantaG3225/surge-rulesets/blob/main/LICENSE). This means you are free to use, modify, and distribute these rule-sets, provided that the copyright notice is retained.

## ⭐ Star History

[![Stargazers over time](https://starchart.cc/SantaG3225/surge-rulesets.svg)](https://starchart.cc/SantaG3225/surge-rulesets)

## 📅 Changelog

*   **2026-04-11**: Added detailed README.md documentation, added MIT License.
*   **2026-04-04**: Initial release, including basic rule-sets.

---

**Author**: SantaG3225
**Date**: April 11, 2026
