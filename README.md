# Useful-Tools
Welcome to my ICT Support Engineer toolkit! As an experienced ICT Support Engineer, I've found these tools to be invaluable in enhancing my efficiency and productivity while providing Level 1 and Level 2 service desk support. Whether you're new to the field or a seasoned veteran, you may find these tools to be a beneficial addition to your technical arsenal.

## Network and Connection Management Tools
* [mRemoteNG](#mremoteng): This is an open-source, multi-protocol, tabbed remote connections manager that I use for handling and switching between multiple remote connections easily.
* [TCPView](#tcpview): A lifesaver when investigating potential security threats or connection issues. This Sysinternals utility provides real-time observation of all TCP and UDP connections, helping me pinpoint suspicious network activity and diagnose connection problems.
## Log Viewing and Management
* [BareTail](#baretail): An effective tool for viewing and monitoring log files in real time. It's especially helpful when troubleshooting as it allows me to spot errors or anomalies as they occur.

## mRemoteNG
Given the numerous connections I must manage daily, a tool that allows for seamless transitions between them is an absolute necessity. That's where mRemoteNG steps in as an invaluable part of my toolkit. This robust software streamlines my workflow by enabling quick and convenient switches between remote sessions. Its user-friendly interface further complements my work style, making the task of juggling multiple connections feel effortless and efficient. The ease of use paired with the comprehensive functionalities mRemoteNG offers truly enhances my productivity, providing comfort and fluency in my everyday operations.
### mRemoteNG vs. Remote Desktop Connection (RDC)
||mRemoteNG|RDC|
|---|---|---|
|Overview|mRemoteNG is an open-source software project for managing remote desktop connections. It is a fork of mRemote, and 'NG' stands for 'Next Generation.' This software supports multiple protocols, including RDP (Remote Desktop Protocol), VNC, ICA, SSH, Telnet, HTTP/HTTPS, rlogin, and raw socket connections.|RDC: Also known as mstsc.exe, RDC is a built-in Windows feature used to connect to remote computers using the Remote Desktop Protocol (RDP). It's a basic tool that allows a single connection at a time and is generally used by end-users.|
|User Interface|mRemoteNG provides a tabbed interface, which allows you to manage and switch between multiple remote sessions from a single window. It also supports organizing connections in a hierarchical tree structure, which can be useful for managing large numbers of connections.|RDC: RDC has a simpler interface, primarily designed for single connections. It doesn't provide an integrated view of multiple sessions, which can make managing multiple connections cumbersome.|
|Features|mRemoteNG: In addition to RDP, mRemoteNG supports multiple protocols, including SSH, Telnet, VNC, and more. It allows you to manage multiple connections, save credentials, customize appearance, and it has more advanced features like the ability to execute scripts/macros at connection events.|RDC: RDC has basic features to initiate and manage a remote desktop connection, such as defining the screen size, local resources usage, and other options. However, it does not support management of multiple sessions concurrently.|
|Security|mRemoteNG: mRemoteNG supports a variety of secure protocols including SSH and HTTPS, and it has a feature to store credentials in a password-protected format. However, as an open-source project, its security updates depend on the activity of its developer community.|RDC: The standard RDC tool benefits from the regular security updates provided by Microsoft to all their supported software. However, it should be used in combination with secure network configurations, like VPNs, and the credentials should be handled securely.|
|Comptaibility|mRemoteNG: It's a Windows-based application and isn't compatible with other operating systems.|RDC: As a part of the Windows operating system, RDC is only available on Windows. However, Microsoft provides Remote Desktop clients for MacOS, iOS, and Android, which can connect to a Remote Desktop server on a Windows machine.|

Conclustion: mRemoteNG is a more powerful tool than RDC due to its support for multiple protocols and advanced features. However, it may be overkill if you only need to connect via RDP and manage a few connections. For more complex needs, mRemoteNG is a strong choice.
### Guide to setting up mRemoteNG
1. Installation
    1. Visit the [mRemoteNG website](https://mremoteng.org/) or its [GitHub page](https://github.com/mRemoteNG/mRemoteNG) to download the latest version of mRemoteNG.
    2. Once downloaded, run the installer.
    3. Follow the prompts in the installation wizard to install mRemoteNG. This will typically involve accepting the license agreement, choosing an installation location, and deciding whether to create desktop shortcuts or not.
    4. Once installation is complete, launch mRemoteNG.
2. Creating a new connection
    1. When mRemoteNG is open, go to the "File" menu and select "New Connection".
    2. This will open a new panel on the left side of the application where you can fill in the details of the connection.
    3. Fill in the following fields:
    4. Connection Name: This is the name you want to assign to the connection. It can be any name that helps you identify the remote system.
    5. Hostname/IP: Enter the hostname or IP address of the remote system you want to connect to.
    6. Protocol: Select the protocol you want to use for the connection. If you're connecting to a Windows system, you will likely want to use RDP (Remote Desktop Protocol).
    7. Username: The username for the remote system.
    8. Password: The password for the remote system.
    9. Domain: If you are connecting to a system that is part of a domain, enter it here. This is usually relevant for business or enterprise environments.
    10. Once you've filled in the connection details, click "OK" or "Save"
3. Connecting to the remote system
    1. Now that the connection is set up, you can connect to the remote system by double-clicking the connection name in the panel on the left.
    2. If you've entered everything correctly, a new tab should open showing the desktop of the remote system.
    3. You can manage multiple connections in the same way, and each will open in a new tab in mRemoteNG.
    4. Remember that the information you need (like hostnames, usernames, and passwords) will depend on the specifics of the systems you're connecting to. 
    
Always ensure that you're following security best practices when managing remote connections, such as using strong, unique passwords, and only connecting over secure networks.
## BareTail
BareTail has become an integral part of my toolkit as it provides the versatility to monitor logs in real-time as well as review past logs. Its user-friendly interface coupled with its robust functionality makes troubleshooting an efficient and streamlined process. By offering a clear view into system activities, BareTail enables me to swiftly identify and address issues, thereby significantly enhancing my productivity and effectiveness.
### Guide to setting up BareTail
1. Installation of BareTail
    1. Download BareTail: Visit the [Bare Metal Software website](http://www.baremetalsoft.com/baretail-2.05/index.php#:~:text=BareTail%20is%20a%20real%2Dtime%20viewing%20tool%20for%20text%20files.) and navigate to the BareTail page. Click on the download link to get the latest version.
    2. Run the Installer: Once the download is complete, locate the downloaded .exe file and double-click on it to start the installation process. Follow the prompts to complete the installation.
    3. Launch BareTail: Once installed, you can launch BareTail from the Start menu or your desktop shortcut if you created one during the installation.

2. Using BareTail
    1. Open a Log File: After opening BareTail, click on "File" on the menu bar, then "Open" from the drop-down list. Navigate to the log file you want to monitor and select it. The log file will open in a new tab in the BareTail interface.
    2. View Real-Time Logs: With the log file open, BareTail will automatically update the display as new entries are added to the log. You can scroll through the log entries using the scroll bar or the arrow keys.
    3. Search in a Log File: To search for a specific text string in the log file, press Ctrl + F to open the "Find" dialog box. Type in the text string you're looking for and click "Find Next" to search for the next occurrence of that string in the log. Click "Find Previous" to search for the previous occurrence.
    4. Highlighting Text: In BareTailPro, you can highlight specific text strings in different colors. To do this, go to "Options" on the menu bar, then "Configure Highlights." Click "Add," type in the text string you want to highlight, choose a color, and click "OK."
    5. Configure Preferences: You can configure the program's preferences by clicking on "Options" in the menu bar, then "Preferences." This allows you to set options like the update speed, the number of lines to display, font size, and more.

Remember that BareTail (free version) is a rather basic real-time log viewer. If you need more advanced features like filtering, bookmarks, and regular expression searches, you might consider upgrading to BareTailPro or using a different log viewer that provides these features.
### Quick guide to User's PC logs
|Logs|Description|Location|
|---|---|---|
|Windows Event Logs|These logs record significant events on your PC, such as successful and failed login attempts, system events, and application events.|%SystemRoot%\System32\Winevt\Logs\|
|Application Logs|Many applications generate their own log files which could be stored in the application's directory in the Program Files or Program Files (x86) folders. Additionally, they might use the Windows AppData folders, typically found at:| C:\Users\[username]\AppData\Local\[application name] C:\Users\[username]\AppData\Roaming\[application name]|
|Internet Information Services (IIS) Logs|Internet Information Services (IIS) Logs are used to record detailed information about activity on an IIS web server. They are critical for diagnosing and troubleshooting issues, monitoring website performance, understanding user behavior, and improving the security of your web applications.|%SystemRoot%\System32\Logfiles\|
## TCPView
I use TCPView as a key instrument for investigating potential malware threats. It allows me to scrutinize suspicious network connections in real time, effectively serving as a live window into the system's network activity. With its detailed display of all active TCP and UDP connections, including the owning process and associated addresses, TCPView provides valuable insights into any abnormal connections that a computer may be making - a strong indicator of possible malware infection.

Furthermore, TCPView proves to be a crucial resource for troubleshooting connection issues with software. It aids in identifying whether a software is unable to establish a network connection, thereby facilitating effective diagnosis and resolution of the problem. The utility of TCPView, therefore, extends beyond just security concerns, making it a comprehensive tool for network connection management.
### Introduction to TCPView
TCPView is a Windows program that provides a detailed listing of all TCP and UDP endpoints on your system, including the local and remote addresses and state of TCP connections. This utility is developed by Microsoft's Sysinternals team. TCPView provides a more informative and conveniently presented subset of the Netstat program that ships with Windows.
### Installation
1. Download TCPView: Visit the Sysinternals section of the [Microsoft website](https://learn.microsoft.com/en-us/sysinternals/downloads/tcpview) and download the latest version of TCPView. It's a standalone program, so no installation is required.
2. Extract the Zip File: Once the download is complete, extract the .zip file to a location of your choice.
3. Run TCPView: Open the extracted folder and double click on the TCPView.exe file to run the application.
### Using TCPView
1. Once you open TCPView, it presents you with a list of all active TCP and UDP connections and the processes that own them.
2. Interpreting the Results: Each row in TCPView represents a single endpoint. You'll see the process (program) that owns the endpoint, the local and remote IP addresses and port numbers, and the connection's current state (e.g., "ESTABLISHED", "LISTENING", etc.).
3. Refreshing the View: TCPView automatically updates every second, but you can force a refresh by pressing Ctrl+R.
4. Ending a Connection: If you want to close a connection, right-click it and select "Close Connection". Please be aware that this should be done cautiously, as abruptly ending connections could cause system instability or data loss.
5. Process Properties: Right-clicking on a process gives you the option to view its properties, which will provide you with more detailed information about the process.
6. Customizing the View: From the View menu, you can customize what information is displayed and how it's presented. For example, you can choose to show unconnected endpoints, resolve IP addresses to hostnames, and more.

Remember, as with any tool that provides detailed system information, TCPView should be used responsibly. Be cautious when ending connections or killing processes, as this could potentially destabilize or harm your system.
