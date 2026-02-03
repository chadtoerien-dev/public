# Security Policy

## Reporting a Security Issue
If you believe you have found a security issue, please report it privately.

Contact: security@petbae.example

## Public Repository Scope
This repository is a public showcase. It intentionally excludes application
source code, infrastructure, and deployment details.

## Local Secret Scan (Before Publishing)
Run these commands from the `public/` folder:

PowerShell:
`rg -nI "(api[_-]?key|secret|token|password|authorization|private[_-]?key|BEGIN (RSA|OPENSSH) PRIVATE)"`

If any matches appear, remove or sanitize them before pushing.

