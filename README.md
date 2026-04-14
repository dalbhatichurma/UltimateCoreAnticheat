🛡️ Ultimate AntiCheat - Minecraft Plugin

A fully working, lightweight and powerful AntiCheat plugin for Paper/Spigot 1.21+ designed to detect and prevent common hacks while keeping server performance smooth and stable.

⚙️ Features
🚫 Advanced Cheat Detection - Detects KillAura, Fly, Speed, Reach, AutoClicker, and more
⚡ High Performance - Optimized for minimal lag impact
🧠 Smart Detection System - Reduces false flags with intelligent checks
📊 Real-Time Monitoring - Tracks suspicious player behavior instantly
🔧 Highly Configurable - Enable/disable checks via config
🔒 Secure & Stable - Built for long-term server protection
📢 Staff Alerts - Alerts staff when suspicious activity is detected
🧪 Punishment Support - Kick/ban commands (optional configurable)
🧩 Detection Modules
KillAura Detection
Reach Check
Fly Hack Detection
Speed Hack Detection
AutoClicker Detection
NoFall Detection
Scaffold Detection (optional advanced)
Movement irregularity checks
🎮 Commands
/ac - Main AntiCheat command
/ac reload - Reload configuration
/ac alerts - Toggle staff alerts
/ac check <player> - View player violation status
/ac debug <player> - Debug player movement checks (admin)
🔐 Permissions
ultimateac.admin - Full admin access
ultimateac.alerts - Receive cheat alerts
ultimateac.bypass - Bypass AntiCheat checks
📦 Installation
Build the plugin:
mvn clean package
Install:
Find UltimateAntiCheat.jar in the target/ folder
Copy it into your server's plugins/ folder
Restart your server
⚙️ Configuration

config.yml example:

checks:
  fly: true
  speed: true
  killaura: true
  reach: true
  autoclicker: true

settings:
  alert_staff: true
  punish_on_violation: false
  max_violations: 5

punishments:
  type: "kick" # kick / ban / none
  message: "&cYou have been removed for cheating!"
📁 Project Structure
UltimateAntiCheat/
├── src/main/java/com/ultimateac/
│   ├── UltimateAntiCheat.java (Main class)
│   ├── check/
│   │   ├── CheckManager.java
│   │   ├── FlyCheck.java
│   │   ├── SpeedCheck.java
│   │   ├── KillAuraCheck.java
│   │   ├── ReachCheck.java
│   │   └── AutoClickerCheck.java
│   ├── manager/
│   │   ├── AlertManager.java
│   │   └── ViolationManager.java
│   └── command/
│       └── ACCommand.java
├── src/main/resources/
│   ├── plugin.yml
│   └── config.yml
└── pom.xml
🧪 Requirements
Java 21+
Paper / Spigot 1.21+
Maven (for building)
🧾 Violation System

Players get violation points when suspicious behavior is detected:

Low violations → warning
Medium violations → alerts to staff
High violations → auto punishment (if enabled)

Stored temporarily in memory for performance.

📢 Permissions Node Summary
Permission	Description
ultimateac.admin	Full control
ultimateac.alerts	Receive alerts
ultimateac.bypass	Ignore checks
🧠 License

Free to use and modify. You may customize it for your server or private use.
