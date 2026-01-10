## Analysis Notes

- Most failed login attempts were caused by insufficient IAM permissions
- Several requests originated from the same IP address
- Events were classified as AWS API calls rather than console logins

Potential risks:
- Misconfigured IAM policies
- Possible credential misuse

Recommended actions:
- Review IAM permissions
- Enable alerts for repeated AccessDenied events

## Alert Configuration

A scheduled alert was created to detect multiple AWS API authentication failures.
The alert triggers when at least one result is returned, indicating five or more
AccessDenied events from the same source IP or user within the execution window.
