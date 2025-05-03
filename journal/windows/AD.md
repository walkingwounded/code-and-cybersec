# Active Directory

## Windows Domain

## Active Directory Users and Computers

## Security groups

https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/understand-security-groups

## Group Policy Object (GPO)

### GPO Distribution

GPOs are distributed through a network share call **SYSVOL**, which is stored in Domain Controller. It may take 120mins to sync the GP updates to all computers. We can force gpupdates on desired computer via command *> gpupdate /force*.

## Authentication Method

**Kerberos:** A modern, secure authentication protocol using tickets to allow users to access multiple services after a single authentication.

**NetNTLM:** An older protocol using challenge-response, now considered less secure and largely replaced by Kerberos in modern systems.

## Trees and Forest

A domain can be split into sub-domains, for e.g. if a company has US and UK office with different GPO. the local.domain can be split into local.domain.uk and local.domain.us.

When a domain has sub-domains, it is termed as a *Tree*.

When 2 or more trees establish a trust relationship, it is termed as *Forest*. For e.g. company A acquires company B, company A can establish or one or two way trust relationship between domains/tree, this trust relationship will allow company A to access company B (depending on the configuration).
