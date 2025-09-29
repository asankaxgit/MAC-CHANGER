<h1>MAC-CHANGER</h1>
A simple Python script to change the MAC address of a network interface on Linux systems.
<h3>Description</h3>
The mac_changer.py script allows users to modify the MAC address of a specified network interface. <br>It provides a command-line interface to input the network interface and the desired new MAC address. The script uses the ifconfig command to perform the MAC address change and displays the updated network configuration.
<h3>Features</h3>

Change the MAC address of a specified network interface.<br>
User-friendly ASCII art banner and usage instructions.<br>
Command-line argument parsing with error handling.<br>
Displays the updated network configuration after changing the MAC address.

<h3>Requirements</h3>

Python 3.x
Linux operating system<br>
Root privileges (use sudo to run the script)<br>
ifconfig command-line tool (usually available on Linux systems)<br>

<h3>Installation</h3>

Clone the repository:git clone https://github.com/your-username/MAC-CHANGER.git<br>
Navigate to the project directory:cd MAC-CHANGER



<h3>Usage</h3>
Run the script with root privileges, specifying the network interface and the new MAC address.<br>
sudo python mac_changer.py -i <interface> -m <new_mac_address>

<h3>Example</h3>
To change the MAC address of the wlan0 interface to e8:d0:fc:e8:3a:30:<br>
sudo python mac_changer.py -i wlan0 -m e8:d0:fc:e8:3a:30

<h3>Options</h3>

-i, --interface: Specify the network interface (e.g., wlan0, eth0).<br>
-m, --mac: Specify the new MAC address (e.g., e8:d0:fc:e8:3a:30).<br>
Use --help for usage information:python mac_changer.py --help



<h3>Output</h3>
The script will:

Display an ASCII art banner and usage instructions.<br>
Change the MAC address of the specified interface.<br>
Show the updated network configuration using ifconfig.

<h3>Notes</h3>

Ensure you have root privileges to run the script, as changing the MAC address requires administrative access.<br>
The script uses the ifconfig command, which may not be available on all systems (e.g., some modern Linux distributions use ip instead). <br>In such cases, you may need to modify the script to use the ip command or install ifconfig.<br>
Always verify the MAC address format (e.g., XX:XX:XX:XX:XX:XX) to avoid errors.

<h3>License</h3>
© 2025 asankaxgit. All Rights Reserved. See LICENSE for details.
<h3>Disclaimer</h3>
Changing your MAC address may disrupt network connectivity or violate network policies. Use this tool responsibly and only on devices and networks you have permission to modify.
