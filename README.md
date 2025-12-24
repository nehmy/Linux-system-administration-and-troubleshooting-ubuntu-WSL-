# Linux-system-administration-and-troubleshooting-ubuntu-WSL-
This project documents my hands on experience using ubuntu on windows subsystem for linux, focusing and command line operations on linux system administration, SSH troubleshooting and command line operations

## Key Tasks Performed
- Installed and configured Ubuntu using WSL
- Troubleshot SSH key permission issues
- Fixed SSH authentication failures caused by incorrect file permissions
- Fixed security issues by implementing the principle of least privilege for SSH private keys 
- Used Linux commands like df, free -m, ip to inspect system, memory, disk, and network status
- Troubleshot connectivity issues using ping, ssh -vv for debugging 

## Troubleshooting Experience
While attempting to SSH into an AWS EC2 instance, I encountered:
- SSH key permission errors (`permissions too open`)
- Authentication failures
- Connection timeouts

Resolution steps included:
- Creating a clean copy of the SSH key
- Correcting ownership and permissions using `chmod` because the key had permissions that were too broad(0555)
- Retesting connectivity using ls -la until a successful secure login

## Evidence
Screenshots included show:
- WSL installation
- SSH errors and debugging output
- Successful SSH login
- System, disk, memory, and network checks

## Skills Demonstrated
- Linux command line usage
- SSH troubleshooting
- File permissions and ownership
- System diagnostics
- Problem-solving and documentation
