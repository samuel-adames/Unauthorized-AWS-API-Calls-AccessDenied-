## MITRE ATT&CK Mapping

### Technique: T1078 – Valid Accounts
**Tactic:** Initial Access / Persistence

Repeated AWS API calls resulting in AccessDenied errors may indicate the use of
valid credentials attempting to access unauthorized resources.

### Technique: T1087 – Account Discovery
**Tactic:** Discovery

The attacker may be enumerating permissions or available services by observing
which API calls fail.

### Detection Coverage
This detection helps identify suspicious cloud activity related to misuse of IAM
credentials and permission enumeration attempts.
