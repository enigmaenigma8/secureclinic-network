# Threat Model – SecureClinic Network

## Primary Threats Addressed

| Threat                              | Mitigation                                      |
|-------------------------------------|-------------------------------------------------|
| Clear-text patient data leakage     | Mandatory anonymization before processing       |
| Compromise of a single clinic       | Zero Trust + data and permission isolation      |
| Lateral movement                    | Continuous verification + segmentation          |
| Lack of accountability              | Immutable audit trail                           |
| Human error                         | Automated validation and reduced manual access  |
| Loss of infrastructure control      | Self-hosted design                              |

## Assumptions

- Clinics are untrusted by default
- Network perimeter is not a trust boundary
- Audit logs must be tamper-evident
