# Active Directory

## Windows Domain

## Active Directory Users and Computers

## Security groups

https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/understand-security-groups

## Group Policy Object (GPO)

### GPO Distribution

GPOs are distributed through a network share call **SYSVOL**, which is stored in Domain Controller. It may take 120mins to sync the GP updates to all computers. We can force gpupdates on desired computer via command *> gpupdate /force*.

