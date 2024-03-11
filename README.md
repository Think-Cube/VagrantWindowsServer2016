# Vagrant Windows Server 2016

This repository contains a Vagrantfile for provisioning a Windows web server using VirtualBox

## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- [Vagrant](https://www.vagrantup.com/)
- [VirtualBox](https://www.virtualbox.org/)

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/Think-Cube/VagrantWindowsServer2016.git
   cd VagrantWindowsServer2016
   ```

2. Edit the Vagrantfile to customize the configuration if needed.

3. Bring up the virtual machine:

    ```bash
    vagrant up
    ```

4. Connect to the Windows web server using WinRM:

    ```bash
    vagrant winrm webserver01
    ```

## Configuration

### Windows Server

- **Box:** fujiiface/2012r2
- **Hostname:** windows-webserver01
- **IP Address:** 192.168.57.3 (change as needed)
- **WinRM Credentials:**
  - **Username:** vagrant
  - **Password:** vagrant

### Virtual Machine Settings

- **Memory:** 2048 MB

- **CPUs:** 2

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Contribution

Feel free to contribute by opening issues or pull requests. Your feedback and improvements are highly appreciated!
