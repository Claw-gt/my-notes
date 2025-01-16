##### C:/
Serves as the primary storage locations
Contains *essential direcotries*

#### Essential directories

##### User directory
Stores user information and settings
Uses folder named after account *users*
Subdirectories:
- Documents
- Downloads
- Desktop
- Pictures
##### Windows directory
Serves as the operating system's backbone
Contains system files  essential for its functionality
Located in the root directory
Subdirectories:
- System32
- ...
##### Program Files directory
Central repository for all installed applications
- Program files for 64-bit applications
- Program files (x86) for 32-bit applications

##### Hidden directories and files
Prevents accidental modification or deletion
Enhances the operating system's functionality and security
Allows viewing by adjusting the *View* settings
- PerLogs
- pagefile.sys
- hiberfil.sys

# Windows Architectures

**32-bit**: processes 32 digits simultaneously
**64-bit**: handles 64 digits at once

- Impact on application handling

| Feature         | 32-bit systems                             | 64-bit systems                                         |
| --------------- | ------------------------------------------ | ------------------------------------------------------ |
| Memory handling | Limited to 4GB RAM                         | Theoreticallt, up to 18 billion GB of RAM              |
| Application     | Optimized for 32-bit processors            | Leverages enhanced capabilities of 64-bit processors   |
| Memory          | Restricted memory usage, up to 4 GB        | Can access over a billion gigabytes or exabytes of RAM |
| Performance     | Limited performance capabilities           | Enhanced performance, especially with large data sets  |
| Work per clock  | Struggle to keep pace with growing demands | More work per clock cycle                              |
#### WOW64
*Windows on Windows 64*: runs 32-bit applications on a 64-bit system
Translator within the Windows system

