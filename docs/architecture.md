# Architecture Overview – SecureClinic Network

## High-Level Design

Three private clinics connect to a central self-hosted hub exclusively through Zero Trust channels.

- Every clinic is untrusted by default
- All traffic goes through Zero Trust Gateway
- Anonymization happens before any further processing
- Every operation is written to an immutable audit log
- Single clinic can be isolated without affecting others

## Key Controls

- No clear-text patient data leaves the controlled environment
- Continuous verification of identity and device
- Least privilege and just-in-time access
- Full auditability
