# Access Log Threat Hunter

A lightweight Node.js utility for analyzing web server access logs and flagging potentially suspicious requests.

## Overview
This project parses standard Apache/Nginx-style access logs and applies rule-based detections to identify common web attack patterns such as SQL injection, XSS attempts, path traversal, scanner activity, and probing for sensitive files.

The goal is to support basic triage and investigation workflows similar to those performed in a SOC environment.

## Features
- Parses access log lines into structured fields
- Applies detection rules using regular expressions
- Flags suspicious requests with severity levels
- Generates JSON output for further review

## Requirements
- Node.js (no additional dependencies)

## Usage
```bash
node analyzer.js --in sample_logs/access.log
