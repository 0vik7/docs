Remote Desktop Protocol (RDP) is enabled for images of all versions and editions of the Windows operating system prepared for Yandex.Cloud. You can connect to a VM using the RDP protocol when it is running (with the "RUNNING" status).

To connect using RDP, specify the public IP address or the FQDN of the VM. Access via FQDN is possible from another Yandex.Cloud VM, if it is connected to the same network. You can find out the IP address and FQDN in the management console. Go to the **Network** section on the virtual machine's page.

To connect to a VM:

---

**[!TAB Windows]**

1. Click **Start**.
1. In the search box, enter <q>remote desktop connection</q> and choose **Remote Desktop Connection**.
1. In the window **Remote Desktop Connection** enter the public IP address of the virtual machine to connect to in the **Computer** field.
1. Click **Connect**.
1. Specify the account settings:
    - **User name**: `Administrator`.
    - **Password**: the password that you set when you created the virtual machine.
1. Press **OK**.

#### See also
- [Remote Desktop Connection](https://support.microsoft.com/en-us/help/17463/windows-7-connect-to-another-computer-remote-desktop-connection)

**[!TAB macOS]**

1. Install and run [Microsoft Remote Desktop](https://itunes.apple.com/app/microsoft-remote-desktop/id1295203466) (free official RDP client for Mac).
1. Press ![](../_assets/plus.svg) → **Desktop**.
1. In the **Add Desktop** dialog enter the public IP address of the virtual machine to connect to in the field **PC Name**.
1. In the **User Account** field select **Add User Account**.
1. In the **Add User Account** dialog specify the account settings:
    - **User Name**: `Administrator`.
    - **Password**: the password that you set when you created the virtual machine.
1. Press **Save** twice.
1. Connect to the remote machine by double-clicking the connection you created in the main Microsoft Remote Desktop window.

#### See also
- [Getting started with Remote Desktop on Mac](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/remote-desktop-mac)

**[!TAB Linux]**

1. Install Remmina (a free RDP client for Linux) using the commands:

    ```
    $ sudo apt-add-repository ppa:remmina-ppa-team/remmina-next
    $ sudo apt-get update
    $ sudo apt-get install remmina remmina-plugin-rdp
    ```

1. Start Remmina.
1. Click ![](../_assets/plus.svg).
1. Fill in the **Profile** block as follows:
    - **Name**: a name for the connection.
    - **Protocol**: **RDP - Remote Desktop Protocol**.
1. In the **Basic** tab specify the details for connection and authorization:
    - **Server**: the public IP address of the virtual machine to connect to.
    - **User Name**: `Administrator`.
    - **Password**: the password that you set when you created the virtual machine.
1. Press **Save**.
1. Connect to the remote machine by double-clicking the connection you created in the quick access connection list.

#### See also
- [Installing Remmina on Linux distributions other than Ubuntu](https://remmina.org/how-to-install-remmina/)

---
