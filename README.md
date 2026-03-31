# iam-security-incident-analysis

Access Control Security Incident Analysis
Overview

This project analyzes a security incident involving improper authorization and access control failures within an organizational system.

The investigation identified a former contractor account that retained administrative privileges years after the contract expiration. This represents a serious violation of access control policies and introduces the risk of unauthorized data access or insider threat activity.

This project demonstrates practical skills in:
Identity and Access Management (IAM)
Authorization analysis
Insider threat identification
Access control auditing
Security policy enforcement
Principle of Least Privilege (PoLP)

User Login → Authentication → Authorization → Resource Access
                │
                └── Misconfigured Privileges


Incident Summary:
During the investigation it was discovered that the account belonged to a contractor whose contract expired in 2019, yet the account remained active with administrator-level privileges.

This represents a critical access control oversight.
Identified Security Issues
1. Unauthorized Privilege Retention
The user retained administrator privileges despite no longer being authorized to access the system.
Risk:
Unauthorized data access
Privilege abuse
Potential insider threat

2. Account Lifecycle Mismanagement
The account should have been automatically disabled after the contract ended.
Failure to properly manage account lifecycle can lead to:
Dormant privileged accounts
Long-term unauthorized access
Security compliance violations
Security Recommendations

3. Implement Automatic Account Expiration
All contractor and temporary accounts should automatically expire after a predefined time period.

Recommended policy:
1.Contractor accounts expire after 30 days of inactivity
Automatic disablement when contracts end

2. Enforce Multi-Factor Authentication (MFA)
Administrator accounts should require MFA to reduce the risk of unauthorized access.
Benefits:
Stronger authentication
Protection against credential theft

3. Apply Principle of Least Privilege (PoLP)
Users should only have the minimum permissions necessary to perform their tasks.
Implementation strategies:
Role-Based Access Control (RBAC)
Periodic privilege reviews
Privileged access monitoring
Security Impact

Improper authorization management can lead to:
Insider threat incidents
Data exfiltration
Privilege escalation
Regulatory compliance violations

Implementing strong IAM policies significantly reduces these risks.
                
Potential extensions of this project:

SIEM log analysis
Automated account lifecycle management scripts
RBAC policy implementation
Privileged Access Monitoring dashboards
