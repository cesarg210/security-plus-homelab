# Authentication Failure Simulation

## Objective
Simulate authentication failures to generate security logs.

## Windows Testing
![windows testing](../screenshots/client-login-attempts.png)
Performed multiple failed login attempts.
Observed Event ID 4625.

## Linux Testing
![linux testing](../screenshots/linux-login-testing.png)
![client testing](../screenshots/client-ssh-testing.png)
Generated failed sudo and SSH attempts.
Observed entries in /var/log/auth.log.

## Key Findings
Failed authentication attempts generate identifiable log patterns.

## Security Relevance
These logs are critical for detecting brute force attacks and unauthorized access attempts.
