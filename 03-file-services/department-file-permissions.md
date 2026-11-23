# Department File Services & Access Control

## Project
Sentinel Defense Technologies — Enterprise IT & Security Homelab

## Objective
Configure centralized departmental file storage using Windows Server 2025, Active Directory security groups, and NTFS permissions.

## Environment
- Server: SDT-DC01
- Operating System: Windows Server 2025 Standard Evaluation
- Domain: ad.sentineldefense.test
- File Server Path: C:\CompanyShares
- Network Share: \\SDT-DC01\CompanyShares

## Folder Structure

- IT
- HR
- Finance
- Engineering

## Access Control Configuration

Configured department-specific Active Directory security groups to control access to departmental folders.

| Department | Security Group | NTFS Permission |
|---|---|---|
| IT | GG_IT_Users | Modify |
| HR | GG_HR_Users | Modify |
| Finance | GG_Finance_Users | Modify |
| Engineering | GG_Engineering_Users | Modify |

Each departmental folder uses explicit NTFS permissions. Existing SYSTEM and Administrators permissions were preserved.

## Share Configuration

- Share Name: CompanyShares
- Share Permission: Everyone — Change and Read
- NTFS permissions provide department-level access restrictions.

## Security Considerations

- Departmental access is controlled through Active Directory security groups.
- Users receive permissions through group membership rather than individual account assignments.
- SYSTEM and Administrators retain their required permissions.
- This is a simulated enterprise environment and contains no company data or credentials.

## Testing Status

- [x] Created departmental folders
- [x] Configured NTFS permissions
- [x] Configured network share permissions
- [ ] Test departmental access from a domain-joined Windows client

## Next Steps

Deploy a Windows 11 workstation, join it to the Active Directory domain, and validate departmental file access using employee accounts.
