Specific for servers

### Features

##### Active Directory
Offers a centralized system for:
- Authentication
- Directory services
- Policy enforcement
- Streamline user account creation
- Access control
- Group policy implementation
##### File and Storage Services
##### Web and application platform
- Needs support of IIS
- Allows hosting and running critical web-based applications
##### Remote Desktop Services
- Helps businesses to embrace remote work models
- Facilitates secure remote access
- Enables increased flexibility and productivity
##### PowerShell
Is a scripting and automation framework
Helps streamline workflows and manage server configurations
##### Hyper-V
Allows running multiple virtual machines on a single physical server
Maximizes hardware efficiency
Reduces costs
##### Storage spaces direct (S2D)
##### Network services
- DNS
- DHCP
- VPN
- RDS

---
#### User account control (UAC)
MS Windows security feature
Prevents unauthorized changes
#### Group policy
Manage setting on a network
`gpupdate`
`gpresult`
#### Drive letters
Identifies storage devices with unique letter: A-Z
**C:** main hard drive
**D:** and **E:** may be other partitions drive, and networks
`vol`
`chdir`
`cd`
#### System maintenance and information
Commands:
`shutdown`
`sc`
`chkdsk`: check disk for error and tries to fix them if found
`diskpart`: diskpart utility
`winver`: check Windows version
`format`: format disks or drives. *e.g. format c:/FS:NTFS*
#### Managing files and directories
`dir`: lists directories. Same as `ls`
`md`: Creates directory. Same as `mkdir`
`rd`: delete directories or `rmdir`
`ren` : rename
`del`: delete files
#### File copying and backup
`copy`: copy file between directories.
*/v* verifies integrity
*/y* supresses confirmation prompts

`xcopy`: advanced copying tool
*/s* copy subdirectories
*/e* copy empty directories
*/a* preserve file attributes and timestamps
*/h* copy hidden files and system files

`robocopy`: handles complex file copying scenarios
*/MIR* copies the contents of the source folder to the destination folder
#### Hostname and network
`hostname`
`ipconfig`
`ping`

---

# Active Directory

Designed to manage:
- User accounts
- Computer systems
- Network resources

#### Organizational Units (OUs)
Used to manage resources
Delegate admin tasks
Apply group policy
Manage permissions

More in [[Day 15 - Active Directory]]