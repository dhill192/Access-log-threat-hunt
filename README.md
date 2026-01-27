# Access Log Threat Hunter

A lightweight Node.js command-line utility for analyzing web server access logs and flagging potentially suspicious activity.

## Overview

This project parses standard Apache/Nginx-style access logs and applies rule-based detections to identify common web attack patterns such as:

- SQL injection attempts
- Automated scanner activity
- Path traversal
- Probing for sensitive files

The tool is designed to support basic triage and investigation workflows similar to those performed by a Tier 1 SOC analyst.

## Features

- Parses access log lines into structured fields
- Applies detection rules using regular expressions
- Flags suspicious log entries with severity levels
- Outputs a summarized JSON report for review

## Requirements

- Node.js (no external dependencies)

## Usage

```bash
node Analyzer.js --in sample_logs/access.log
