# 🧠 Detection Rule Engine

## 📜 What Is This?
This is a lightweight Python-based detection engine designed to simulate how a SOC analyst might write rules to flag suspicious patterns in system logs.

It's **not a full SIEM** — it's a learning-focused utility that helps me understand:
- Log structures
- Pattern matching using regex
- Writing basic alerting logic
- Triggering alerts from real-world-looking data

## 🔍 Key Features
- Parse logs from `/var/log/auth.log`, `/var/log/syslog`, and custom files
- Apply detection rules (regex + logic)
- Generate alerts in JSON or console format
- Easy to extend with new rules and log formats

## 💡 Why I’m Building This
I’ve already created a Mini-SIEM API focused on ingestion and routing. This project complements that by shifting focus to **rule logic** and **on-the-ground detection**, similar to what an actual SOC tool might use for Tier 1 alerting.

## 🧱 Tech Stack
- Python 3.x
- Built-in modules only: `re`, `datetime`, `json`, `argparse`
- Optional: Flask (later) if I want to expose it via API

## 📁 Structure
```
/logs/              -> Sample logs for testing
/rules/             -> Detection rules in plain text or JSON
engine.py           -> Main rule engine logic
alert_generator.py  -> Alert formatting and output
README.md           -> You're reading it
```

## 🧪 Example Use Case
> Detect brute force attempts in SSH logs  
> Detect port scan patterns  
> Detect failed login spamming within time windows

## 📍 Status
Currently setting up the base structure.  
First working rule expected by early July 2025.
