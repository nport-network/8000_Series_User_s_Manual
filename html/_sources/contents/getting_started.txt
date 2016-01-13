Getting Started
===============

This chapter introduces the management interface of NPort WebSmart Switch.

Management Options
------------------

The NPort WebSmart Switch can be managed through any port on the device by using the Web-based Management. Each switch must be assigned its own IP Address, which is used for communication with Web-Based Management. The PC’s IP address should be in the same range as the switch. Each switch can allow only one user to access the Web-Based Management at a time. The PC should have an IP address in the same range as the switch. Each switch can allow one user to access to the Web-Based Management at a time.

Using Web-based Management
~~~~~~~~~~~~~~~~~~~~~~~~~~

After a successful physical installation, you can configure the Switch, monitor the network status, and display statistics using a web browser.

Supported Web Browsers
######################

The embedded Web-based Management currently supports the following web browsers:

- Internet Explorer 6 or later version
- Netscape 8 or later version
- Firefox 3.0 or later version
- Chrome 5.0 or later version
- Safari 4.0 or later version
- Opera 10 or later version

Connecting to the Switch
########################

You will need the following equipment to begin the web configuration of your device:
1. A PC with a RJ-45 Ethernet connection
2. A standard Ethernet cable
Connect the Ethernet cable to any of the ports on the front panel of the switch and to the Ethernet port on the PC.

.. figure:: /images/image9.png
	:align: center

	Connected Ethernet cable

Login Web-based Management
##########################

In order to login and configure the switch via an Ethernet connection, the PC must have an IP address in the same subnet as the switch. For example, if the switch has an IP address of **192.168.1.1**, the PC should have an IP address of **192.168.1.z** (where z is a number between 2 ~ 254), and a subnet mask of **255.255.255.0**. You can open the web browser and enter **192.168.1.1** (the factory-default IP address) in the address bar. Then press <Enter>.

.. figure:: /images/login_ip.png
	:align: center

	Enter the IP address 192.168.1.1 in the web browser

.. figure:: /images/login_page.png
	:align: center

	Login page

.. NOTE::
	The switch's factory default IP address is 192.168.1.1 with a subnet mask of 255.255.255.0 and a default gateway of 0.0.0.0.


Configuration
-------------

The features and functions of the NPort WebSmart Switch can be configured for optimum use through the Web-based Management Utility.

Web-based Management
~~~~~~~~~~~~~~~~~~~~

After a successful login you will see the screen below:

.. figure:: /images/web_based_management.png
	:align: center

	Web-based Management

Above is the Web-based Management screen. The three main areas are the **Tool Bar** on top, the **Function Tree**, and the Main Configuration Screen.

The **Tool Bar** provides a quick and convenient way for essential utility functions like firmware and configuration management.

By choosing different functions in the **Function Tree**, you can change all the settings in the **Main Configuration Screen**. The main configuration screen will show the current status of your Switch by clicking the model name on top of the function tree.

At the upper right corner of the screen the username and current IP address will be displayed.

Under the username is the Logout button. Click this to end this session.

.. NOTE::
	If you close the web browser without clicking the Logout button, it will be seen as an abnormal exit and the login session will still be occupied.

Finally, by clicking on the NPort logo at the upper-left corner of the screen you will be redirected to the local NPort website.

*Tool Bar > Save*
	The Save provides Save Configuration.

.. figure:: /images/save.png
	:align: center

	Save

- Save Configuration
	Select to save the entire configuration changes you have made to the device to switch’s non-volatile RAM.

.. figure:: /images/save_configuration.png
	:align: center

	Save Configuration

Function Tree
-------------

All configuration options on the switch are accessed through the Setup menu on the left side of the screen. Click on the setup item that you want to configure. The following sections provide more detailed description of each feature and function.

.. figure:: /images/function_tree.png
	:align: center

	Function Tree

Management->Maintenance
#######################

The Maintenance function controls such as Reset System, Reboot Device, Firmware Upgrade and Configuration Backup & Restore.

.. figure:: /images/advanced_settings_management.png
	:align: center

	Figure – Advanced Settings > Management

- Configuration
	Provide a safe reset option for the Switch. All configuration settings in non-volatile RAM will be reset to factory default and then the Switch will reboot.

.. figure:: /images/management_maintenance_configuration.png
	:align: center

	Management > Maintenance > Configuration

- Firmware Backup & Upgrade
	| Click *Backup* to save the firmware to your disk.
	| Click *Browse* to browse your inventories for a saved firmware file.
	| Click *Upgrade* after selecting the firmware file you want to restore.

.. figure:: /images/management_maintenance_firmware.png
	:align: center

	Management > Maintenance > Firmware

.. WARNING::
		Do not disconnect the PC or remove the power cord from device until upgrade is complete. The Switch may crash if the Firmware Upgrade is incomplete.

- Reboot
	Provide a safe way to reboot the system. Click Reboot to restart the switch.

.. figure:: /images/management_maintenance_reboot.png
	:align: center

	Management > Maintenance > Reboot

System Information
------------------

The System Information provides an overview of the switch which includes essential information such as firmware, hardware and IP address. It also offers an overall status of common software features:

Port Mirroring: 
	Click Basic *Settings > Port Management > Port Mirroring*. By default this feature is disabled.
Storm Control:
	Click Advanced *Setting > Bandwidth Control > Storm Control*. By default this feature is disabled.
IGMP Snooping:
	Click Advanced *Setting > L2 Multicast Control > IGMP Snooping*. By default this feature is disabled.
Link Aggregation:
	Click *Advanced Setting > Link Aggregation*. By default this feature is disabled.
802.1Q VLAN:
	Click *Advanced Setting > VLAN > 802.1Q VLAN*. By default this feature is disabled.
Loop Detection:
	Click *Advanced Setting > Loop Detection*. By default this feature is disabled.

.. figure:: /images/system_information.png
	:align: center

	System Information

Basic Settings > General Setting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The General Setting allows the user to configure the IP address and the basic system information of the Switch.

IP Information:
	There are two ways for the switch to obtain an IP address: Static and DHCP (Dynamic Host Configuration Protocol).
When using static mode, the IP Address, Subnet Mask and Gateway can be manually configured. When using DHCP mode, the Switch will first look for a DHCP server to provide it with an IP address (including network mask and default gateway) before using the default or previously entered settings. By default the IP setting is static mode with IP address is 192.168.1.1 and subnet mask is 255.255.255.0.

System Information:
	By entering a System Name, the device can more easily be recognized on the LAN.

.. figure:: /images/basic_settings_general_settings_system.png
	:align: center

	Figure – Basic Settings > General Settings > System
 
Basic Settins > Port Management > Port Setting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the Port Management page, the status of all ports can be monitored and adjusted for optimum configuration. By selecting a range of ports (*From Port* and *To Port*), the Speed can be set for all selected ports, effective by clicking *Apply*.

.. figure:: /images/basic_settins_port_management_port_setting.png
	:align: center

	Basic Settins > Port Management > Port Setting

Speed:
	Copper connections can operate in Forced Mode settings (1000M Full, 100M Full, 100M Half, 10M Full, 10M Half), Auto, or Disabled. The default setting for all ports is Auto.

.. NOTE:: 
	Be sure to adjust port speed settings appropriately after changing connected cable media types.

Link Status:
	Reporting Down indicates the port is disconnected.
Flow Control:
	You can enable this function to mitigate the traffic congestion. Ports configured for full-duplex use 802.3x flow control, half-duplex ports use backpressure flow control. The default setting is disabled.

Basic Settings > Port Management > Port Counters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Statistics screen displays the status of each port packet count.

Click *Refresh* button to view the latest information.

Click *Clear All* button to reset the details displayed.

.. figure:: /images/basic_settings_port_management_port_counters.png
	:align: center

	Basic Settings > Port Management > Port Counters

EgressOK:
	Number of packets transmitted successfully.
IngressOK:
	Number of packets received successfully.
EgressError:
	Number of transmitted packets resulting in error.
IngressError:
	Number of received packets resulting in error.

Basic Settings > Port Management > Port Mirroring
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Port Mirroring is a method of monitoring network traffic that forwards a copy of each incoming and/or outgoing packet from one port of the Switch to another port where the packet can be studied. This enables network managers to better monitor network performances.

.. figure:: /images/basic_settings_port_management_port_mirroring.png
	:align: center

	Basic Settings > Port Management > Port Mirroring

Selection *Mirror Mode* for the Source Ports is as follows:

Ingress:
	Duplicates the data transmitted from the source port and forwards it to the Target Port.
Click “all” to include all ports into port mirroring.

Egress:
	Duplicates the data that received from the source port and forwards it to the Target Port.
Click “all” to include all ports into port mirroring.

Both (transmit and receive) mode:
	Duplicate both the data transmitted from and data sent to the source port, and forwards all the data to the assigned Target Port. Click “all” to include all ports into port mirroring.
.. NOTE::
	The target ports will stop mirroring packets if there are unknown tags or destination packets sent out by source ports.

Advanced Settings > Link Aggregation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The LAG function allows the switch to combine two or four ports together to increase bandwidth. Select the LAG Groups, choose the Members to be grouped together, and then click *Apply* to activate the selected LAG Groups. Up to eight LAG Groups may be created, each supporting up to four ports.

Click *Disable* button to remove all the members in this trunk group.

.. figure:: /images/advanced_settings_link_aggregation.png
	:align: center

	Advanced Settings > Link Aggregation

Advanced Settings > L2 Multicast Control > IGMP Snooping
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

With Internet Group Management Protocol (IGMP) snooping, the WebSmart Switch can make intelligent multicast forwarding decisions by examining the contents of each frame’s Layer 2 MAC header.

By default, IGMP is disabled. If enabled, the WebSmart switch can recognize IGMP queries and reports sent between network stations or devices and an IGMP host. With IGMP snooping enabled, the WebSmart switch will forward multicast traffic only to the connections that have members attached

.. figure:: /images/advanced_settings_l2_multicast_control_igmp_snooping_igmp_snooping_setting.png
	:align: center

	Advanced Settings > L2 Multicast Control > IGMP Snooping> IGMP Snooping setting

Advanced Settings > Loop Detection
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Loopback Detection function is used to detect the loop created by a specific port while Spanning Tree Protocol (STP) is not enabled in the network, especially when the down links are hubs or unmanaged switches. The Switch will automatically shut down the port. The Loopback Detection port will be unlocked when the Loopback Detection *Recover Time* times out. The Loopback Detection function can be implemented on a range of ports at a time.

.. figure:: /images/advanced_settings_loop_detection.png
	:align: center

	Advanced Settings > Loop Detection

Loop Detection:
	Enable or disable Loopback detection. The default is Disabled.
Interval (1-32767):
	Set a Loop detection Interval between 1 and 32767 seconds. The default is 1 seconds.
Recover Time (0 or 60-1000000):
	Time allowed (in seconds) for recovery when a Loopback is detected.

The Loop Detection Recover Time can be set at 0 seconds, or 60 to 1000000 seconds. Entering 0 will disable the Loop Detection Recover Time. The default is 60 seconds.
Click *Apply* to implement changes made.


Troubleshooting > Cable Diagnostics
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Cable Diagnostics is designed primarily for administrators and customer service representatives to examine of the copper cable quality. It rapidly determines the type of cable errors occurred in the cable.
Select a port and then click the Test button to start the diagnosis.

.. figure:: /images/troubleshooting_cable_diagnostics.png
	:align: center

	Troubleshooting > Cable Diagnostics

Test Result:
	The description of the cable diagnostic results.

	- OK: Means the cable is good for the connection.
	- Short in Cable: Means the wires of the RJ45 cable may be in contact somewhere.
	- Open in Cable: Means the wires of RJ45 cable may be broken or the other end of the cable is simply disconnected.
	- Test Failed: Means some other errors occurred during cable diagnostics. Please select the same port and test again.

Cable Fault Distance (meters):
	Indicates the distance of the cable fault from the Switch port, if the cable is less than 2 meters, it will show “No Cable”. The deviation of "Cable Fault Distance" is +/-2 meters.

.. NOTE::
	Cable length detection is effective at every speed of 10Mbps, 100Mbps and 1Gbps.

Advanced Settings > VLAN > 802.1Q VLAN
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A VLAN is a group of ports that can be anywhere in the network, but communicate as though they were in the same area.

VLANs can be easily organized to reflect department groups (such as R&D, Marketing), usage groups (such as e-mail), or multicast groups (multimedia applications such as video conferencing), and therefore help tosimplify network management by allowing users to move devices to a new VLAN without having to changeany physical connections.

By default, 802.1Q VLAN is disabled. With 802.1Q VLAN enabled, the VLAN VID 1 is created by default with an empty VLAN name field and all ports are configured as “Untagged” members.

The 802.1Q VLAN configuration is accomplished in following steps:
	- Creating a new VID group
	- Assigning ports as Access or Trunk.
	- Configuring the PVID of access VLAN
	- Advanced *Settings > VLAN > 802.1Q VLAN*: Click *Apply* to create a new VID group.
	- Advanced *Settings > VLAN > 802.1Q VLAN Port Setting > Edit*: Change the Port VLAN Mode act as Access or Trunk.
	- *PVID settings*: Port VLAN ID (PVID) is an identification that encompasses a particular switch port’s identification and VLAN membership. This identification is used to classify the incoming untagged frames.
	- Click *Edit* to configure the PVID of a port.

*Delete*:
	Click to delete the VLAN group.

.. figure:: /images/advanced_settings_vlan_8021q_vlan.png
	:align: center

	Advanced Settings > VLAN > 802.1Q VLAN

.. figure:: /images/advanced_settings_vlan_8021q_vlan_port_setting.png
	:align: center

	Advanced Settings > VLAN > 802.1Q VLAN Port Setting

.. figure:: /images/advanced_settings_vlan_8021q_vlan_port_setting_edit.png
	:align: center

	Advanced Settings > VLAN > 802.1Q VLAN Port Setting > Edit


.. NOTE::
	When 802.1Q VLAN is enabled, the Port- Based VLAN settings will be set to Disabled.

Basic Settings > General Settings> Management VLAN
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

802.1Q VLAN is used to decide which VLAN can access the switch.

.. figure:: /images/basic_settings_general_settings.png
	:align: center

	Basic Settings > General Settings

.. NOTE::
	When 802.1Q Management VLAN is enabled, the 802.1Q VLAN should be enabled first.

Advanced Settings > VLAN > Port-Base VLAN
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Port-Based VLANs are the simplest and most common form of VLAN. It assigns the appliance LAN ports to VLANs, effectively transforming the appliances. You can assign multiple ports to the same VLAN, or each port to a separate VLAN.

.. figure:: /images/advanced_settings_vlan_port_based_vlan_settings.png
	:align: center

	Figure – Advanced Settings > VLAN >Port-Based VLAN Settings

VLAN State:
	Choice Enabled or disable then click the *Apply* to enable or disable the feature.
*Add VLAN Index*:
	Click to create a new VLAN and to select VLAN ports. To save the members in a group, click *Apply*.
*Delete*:
	Click to delete the VLAN group.
*Delete All*:
	Click to delete all the VLAN groups.

.. NOTE::
	When **Port-Based VLAN** is enabled, the 802.1Q VLAN settings and 802.1Q management VLAN settings will be set to Disabled as default. By default, all ports are untagged.

Advanced Settings > QoS
~~~~~~~~~~~~~~~~~~~~~~~

QoS is an implementation of the IEEE 802.1p standard that allows network administrators to reserve bandwidth for important functions that require a larger bandwidth or that might have a higher priority, such as VoIP (voice-over Internet Protocol), web browsing applications, file server applications or video conferencing. Thus with larger bandwidth, less critical traffic is limited, and therefore excessive bandwidth can be saved.

The following figure displays the status of Quality of Service priority levels of each port, higher priority means the traffic from this port will be first handled by the switch. For packets that are untagged, the switch will assign the priority depending on your configuration.

.. figure:: /images/advanced_settings_qos.png
	:align: center

	Advanced Settings > QoS

Scheduler Method:
	Select Strict Priority to process the packets with the highest priority first. Select WRR (Weighted Round-Robin) to process packets according to the weight of each priority. When a priority level has reached its egress weight, the system will process the packets in the next level even if there are remaining packets. NPort WebSmart Switch system’s weight of priority levels are: 8 (Highest), 4 (High), 2 (Medium) and 1 (Low) packet. By default, the queuing mechanism is **Strict Priority**.

Advanced Settings > Bandwidth Control > Storm Control
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Storm Control feature provides the ability to control the receive rate of broadcast, multicast, and unknown unicast packets. Once a packet storm has been detected, the Switch will drop packets coming into the Switch until the storm has subsided.

.. figure:: /images/advanced_settings_bandwidth_control_storm_control.png
	:align: center

	Advanced Settings > Bandwidth Control > Storm Control

Storm Control Type:
	User can select the different Storm type from Broadcast Only, Multicast & Broadcast, and Multicast & Broadcast & Unknown Unicast.
Threshold (pps):
	If storm control is enabled (by default it is disabled), the threshold can be set from 1 to 1,000,000pps.
Click *Apply* for the settings to take effect.

Advanced Settings > Bandwidth Control > Rate Limit
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Bandwidth Control page allows network managers to define the bandwidth settings for a specified port’s transmitting and receiving data rates.

.. figure:: /images/advanced_settings_bandwidth_control_rate_limit.png
	:align: center

	Advanced Settings > Bandwidth Control > Rate Limit

From Port / To Port: A consecutive group of ports may be configured starting with the selected port.

Direction:
	This drop-down menu allows you to select between Inbound (receive) and Outbound (transmit). This setting will determine whether the bandwidth ceiling is applied to receiving, transmitting, or both receiving and transmitting packets.
No Limit:
	This drop-down menu allows you to specify that the selected port will have no bandwidth limit. Enabled disables the limit.
Rate:
	This drop-down menu allows you to select data rate from 64Kbps to 512Mbps.
Click *Apply* to set the bandwidth control for the selected ports.

Basic Settings > MAC Management > Static MAC Setting
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/basic_settings_mac_management_static_mac_setting.png
	:align: center

	Basic Settings > MAC Management > Static MAC Setting

The *Static MAC Address Setting* table displays the static MAC addresses connected, as well as the VID. Click *Add Mac* to add a new MAC address, you also need to select the assigned Port number, enter both the Mac Address and VID and Click *Apply*. Click *Delete* to remove one entry or click *Delete all* to clear the list. You can also copy a learned MAC address from *Dynamic Forwarding Table* (please refer to *Security > MAC Address Table > Dynamic Forwarding Table* for details).

By disabling Auto Learning capability and specify the static MAC addresses, the network is protected from potential threats like hackers because traffic from illegal MAC addresses will not be forwarded by the Switch.

.. NOTE::
	N1-8016/N1-8024/N1-8074 support 128 Static MAC Address entries.

Basic Settings > MAC Management > MAC Address Table
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For each port, this table displays the MAC address learned by the Switch.

.. figure:: /images/basic_settings_mac_management_mac_address_table.png
	:align: center

	Basic Settings > MAC Management > MAC Address Table

Advanced Settings > LLDP
~~~~~~~~~~~~~~~~~~~~~~~~

Link Layer Discovery Protocol (LLDP) allows the switch to advertise major capabilities and physical descriptions to adjacent devices. This information can help you identify system topology and detect bad configurations on the LAN. 
Select Enabled and click *Apply* to enable LLDP.

.. figure:: /images/advanced_settings_lldp.png
	:align: center

	Figure – Advanced Settings > LLDP

Advanced Settings > Multicast Address
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Multicast is a limited broadcast that allows one-to-many and many-to-many connections. In Layer 2 multicast, a single frame addressed to a specific multicast address is received, and copies of the frame to be transmitted on each relevant port are created.

.. figure:: /images/advanced_settings_multicast_address.png
	:align: center

	Figure – Advanced Settings > Multicast Address

Advanced Settings > DoS Prevention
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The switch supports configurable Denial of Service (DoS) attack protection for many different types of attacks.

.. figure:: /images/advanced_settings_dos_prevention.png
	:align: center

	Figure – Advanced Settings > DoS Prevention

Advanced Settings > STP
~~~~~~~~~~~~~~~~~~~~~~~

Spanning Tree Protocol (STP) provides a tree topology for switches on a bridged LAN.  STP allows a network to have redundant paths without the risk of network loops.

Rapid Spinning Tree Protocol (RSTP) detects and uses network topologies to enable faster convergence after a topology change, without creating forwarding loops. 

.. figure:: /images/advanced_settings_stp.png
	:align: center

	Figure – Advanced Settings > STP

Managemenet > User Accounts
~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can modify the username and password in order to refuse unauthorized users. 

.. figure:: /images/management_user_accounts.png
	:align: center

	Figure – Management > User Accounts


Advanced > PoE > PoE Setting (N1-8074 only)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

N1-8074 supports Power over Ethernet (PoE) as defined by the IEEE Specification.  It supplies power to PD device up to 30W for PoE ports (1 – 12), meeting IEEE802.3at standards.  
This page allows user to configure the global PoE settings of the device.  

.. figure:: /images/advanced_settings_poe_poe_setting.png
	:align: center

	Figure – Advanced Settings > PoE > PoE Setting

From Port/To Port:
	Specifies the PoE function of a port or ports.
Priority:
	Configure the power supply priority as “Low”, “Normal”, or “High” on designated port(s). Default is Normal.

State:
	Select “Enabled” or “Disabled” to configure PoE function for designated port(s). Default is Enabled.
Power Limit:
	This function allows you to manually set the port power current limitation to be given to the PD. To protect the N1-8074 and the connected devices, the power limit function will disable the PoE function of the port when the power is overloaded. Select from "Class 1", "Class 2", "Class 3", “Class 4” and "Auto" for the power limit. "Auto" will negotiate and follow the classification from the PD power current based on the 802.3at standard.
Max Wattage:
	Check the box and input the power budget (from 10000 to 30000 milliwatts) to manually assign an upper limit of port power budget on designated port(s).

Click *Apply* to make the configurations take effects or click Refresh to redisplay the table.



Advaned > PoE > PoE Status (N1-8074only)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

PoE System Status:
	Displays the system power status of device.

	- Delivered (W): Displays the current used PoE power. 
	- Power Budget (Total PoE Power Budget): Displays the total PoE power budget of this switch.

The PoE port table also displays status including, Port, Port State, Class, Max watts, and watts Used.  

Class (power limit)
The maximum power used by power devices is defined by the following classification

.. table::

   ===== ========== ==========================
   Class   Usage     Output power limit by PSE
   ===== ========== ==========================
   0       Default   15.4 W
   1       Optional  4 W
   2       Optional  7 W
   3       Optional  15.4W
   4       Optional  30 W
   ===== ========== ==========================
