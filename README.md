# 🚨 Log Alerting & SIEM Mini Tool

## 🎯 What Is It?
A small-scale SIEM-like tool built in Python that parses logs, matches them against simple detection rules, and triggers alerts. The idea is to simulate how enterprise tools like Splunk or Sentinel might do basic correlation.

## 🛠️ Core Components
- Log Parser (auth.log, syslog, web logs)
- Rule engine (regex + logic-based)
- Alert trigger system (JSON or CLI output)
- (Optional) Timeline-style basic visualization

## 💡 Why I'm Building This
While learning SOC and blue team roles, I realized many alerts start with **parsing something correctly**. So this tool is an attempt to build intuition by doing.

## 📦 Stack
- Python 3.x
- Regex, datetime, logging modules
- Sample logs & dummy rules
- Optional Flask backend later

## 🚧 Status
Folder structure ready. First parser will be written by July 1. Target is to make it extensible and simple enough to debug.
