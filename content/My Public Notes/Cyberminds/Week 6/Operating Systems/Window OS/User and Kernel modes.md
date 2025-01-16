### Functions of a processor

Works in two modes: user mode and kernel mode

##### User mode
Restricted mode
Prevents direct access to hardware and system components

Initiation of application in user mode ➡ Windows generates unique process for the application ➡ Process is equipped with own virtual address space and distinct handle table ➡ Protection against unauthorized access

1. Distinct virtual address spaces
2. Isolation of the application
3. Virtual address space is limited
4. Prevents damage to OS data by user mode programs
##### Kernel mode
Reserved mode
Allows interactions between hardware and the operating system
Codes share a single virtual address space
*e.g Connecting software applications with computer's physical hardware*
Kernel and hardware communication is handled by Hardware Abstraction Layer
### Communication between modes
User and kernel modes communicate through **system calls**
- User mode operates in a secure and isolated environment
- Kernel mode acts on behalf of the application to perform hardware-related tasks

![https://learn.microsoft.com/pt-br/windows-hardware/drivers/gettingstarted/images/userandkernelmode01.png](https://learn.microsoft.com/pt-br/windows-hardware/drivers/gettingstarted/images/userandkernelmode01.png)
