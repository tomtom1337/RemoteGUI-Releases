# This software is a demonstration of the IP-Control-API capabilities available within G&D devices <br/>



<a href="https://apps.apple.com/us/app/mobilegui/id1552210719" target="_blank">
  <img src="https://beatscratch.io/assets/app_store.png" width="200" height="70">
</a>

<a href="https://testflight.apple.com/join/3QwH5VWa" target="_blank">
  <img src="https://beatscratch.io/assets/testflight-badge.png" width="200" height="80"/>
</a>

<a href="https://play.google.com/store/apps/details?id=com.mobilegui.android" target="_blank">
  <img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png" width="200" height="80"/>
</a>

<a href="https://github.com/tomvalk/RemoteGUI-Releases/releases/" target="_blank">
  <img src="https://www.yt3dl.net/images/apk-download-badge.png" width="200" height="80"/>
</a>


<a href="https://github.com/tomvalk/RemoteGUI-Releases/releases/" target="_blank">
  <img src="https://images.squarespace-cdn.com/content/v1/57eacb7e197aea92a6bb9682/1556121147198-U3JZP5DJZ7TQG9XFW4WV/ke17ZwdGBToddI8pDm48kCer5a32Hjd0zIRltAZ56MRZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpwltLZdKwhAec3545lrL2t9njB-xvxgVWJEReCmYKzSeBiwy-EsC0c1Ort17sWLgzo/bezlio-app-badges-windows-version.png?format=1500w" width="200" height="80"/>
</a>

--------------



# RemoteGUI (Windows) v5.0.0
Last Update Friday the 13th August 2021

<img src="https://raw.githubusercontent.com/tomvalk/RemoteGUI-Releases/main/Mockup_Laptop.png" height="25%" width="25%">

[![Generic badge](https://img.shields.io/badge/Screenshots-RemoteGUI-orange.svg)](https://github.com/tomvalk/RemoteGUI-Releases/blob/main/Screenshot_RemoteGUI/)

<details><summary>Features</summary>
<p>
	

- Full integration of the IP-Control-API command set - connect, disconnect, login, logout etc.
- Shows the current connection status for all devices
- Automatic detection of all devices connected to a matrix incl. RemoteAccess and U2 devices
- Detection of newly connected devices during runtime
- Adjustment of states between online, ready and offline by PushEventNotfications during runtime
- PushEventNotfications can be shown as WIndows Messages for monitoring all conenctions
- Special commands like send messages to all devices or switch all devices at the same time can be executed directly
- Complete list with all connected devices incl. data like name, UID, port, features and much more
- Complete script builder with almost 200 API commands - Allows to create, test and export complete scripts with one click without XML knowledge
- Control and switching of additional KVM switches and MultiPower possible
- Locking access with a password is possible
- And much more!


</p>
</details>

<details><summary>Requirements</summary>
<p>

- Windows OS with Microsoft .net Framework 4.6 or higher
- It's recommended to use the latest G&D firmware in order to use all available functions and features
- The G&D firmware expansion IP-Control-API togehther with an activated Remote-Control-Port: 

```
Webinterface -> 'Your Device' -> Information -> Activated Features
Webinterface -> 'Your Device' -> Configuration -> Network -> Remote-Control -> TCP:xxxxx -> Enabled
```
</p>
</details>

<details><summary>Supported Devices</summary>
<p>

```
- ControlCenter-Digital
- ControlCenter-Compact
- ControlCenter-IP 2.0
- MUX-NT
- MUX-ATC
- Multipower-NT
```

</p>
</details>


<details><summary>Changelog</summary>
<p>
	
```
Changelog:
5.0.0
- New Design / Logo to match the MobileGUI
- Added the setting to show the Push-Event-Notification in the Windows Notifcation Center
- Added the option to show/hide Targets within the selected Workplace filter to the settings
- Overall improvements and bug fixes 

4.9.0
- Added the possibility to lock the RemoteGUI with a password 
	-> By default the password entry on startup is disabled and the password is 4658
- Added the setting to show only devices that are in the selected Workplace filter to the settings
- Moved RemoteMUX to the main window as a separate tab
- Moved Global Matrix Commands to the main window as a separate tab
- Added new RemoteMP tab for controlling MultiPower-NT 
	-> Requires firmware MultiPower-NT >= 1.1.000
- Overall improvements and bug fixes 

4.8.0
- Improved RemoteGUI appearance
	-> Added a Workplace Filter
	-> Added more apperance settings
	-> Added a Dark Mode (BETA)
- Added U2-LAN/U2+ device to the RemoteGUI and [Script Builder] 
- Added new IP-Control-API features for for MUX-ATC
	-> Single Signal Switching in the [Script Builder] for MUX-ATC
	-> Requires firmware MUX-ATC >= 1.1.000

4.7.0
- Added matrix overview tab to show all connected devices (can be copied to Excel etc.)
- Added lot of commands to the [Script Builder], more than 180x commands are now supported for
	-> ControlCenter-Compact, ControlCenter-Digital, ControlCenter-IP
	-> DL-MUX, MUX-NT, MUX-ATC
	-> RemoteAccess-CPU, MultiPower-NT
- Added new IP-Control-API features for ControlCenter-Compact / ControlCenter-Digital 
	-> Added <AllowTemporaryLogon> for OpenAccess-CON via the CON context menu (right click) and in the [Script Builder] 
	-> Added <selectvideostream> for DH devices via the CON context menu (right click) and in the [Script Builder]
	-> Improved <disconnectEvent> to show total connections to each CPU live now faster and can be switched off without refresh
	-> Requires firmware CC-Compact >= 1.4.000 / CC-Digital >= 2.3.000 and MTX-CON >= 1.7.000 for <selectvideostream>
- Overall speed improvements and bug fixes 

4.6.0
- Added support for [RemoteAccess-CPU] series

4.5.0
- Filter devices depending on status directly in the GUI accessable via the list icon beside the name filter options

4.4.0
- [Script Builder] XML code now in color and colorful
- Added support for [U2+CON/CPU] series

4.3.0 
- Added [Send Message] via CON context menu (again, got lost during the 4.0.0 update)
- Added [Disconnect all CONs] to CPU context menu

4.2.0
- Show total connections to each CPU live (can be switched off in the settings)
- Select [Connections] via the CPU context menu to get a list of all connected CONs 

4.1.0
- Performance improvements for large Matrix installations
- [Highlight] and pin CPUs and CONs via the context menu

4.0.0
- New and improved [RemoteGUI] design and features
- [Script Builder] improved for offline use
- Overall improvements and bug fixes

3.6.0
- New [Script Builder] layout

3.5.0
- Added a [SNMP Tester] accessable via the settings

3.4.0
- Show monitoring now supports [CON-2] and [DH] devices

3.3.0
- Added support for SNMP firmware detection

3.2.0
- [Script Builder] improvements and bug fixes

3.1.0
- Improved push notifications process

3.0.0
- Added support for [ControlCenter-IP] series

2.5.0
- [Script Builder] can now be used without active connection to the matrix

2.4.0
- Added support for [MUX-ATC] series
- Added support for [MUX-NT] series

2.3.0
- Improvements for large Matrix installations
- Added new features to [Script Builder]

2.2.0
- Added a counter for CPU and CON modules

2.1.0
- Added an option to filter CON and CPU modules by name

2.0.0
- New and improved [RemoteGUI] design and features

1.6.0
- Added [Hide] option on the right click context menu 
  -> This will hide the CON or CPU icons until you refresh or restart the [RemoteGUI]

1.5.0
- New [IP-Control-API] features added 
  -> Push Notifications <peripheral_power_on/off_event>
  -> <MatrixConnectionList> for Console and Targets

1.4.0
- Added layout options
- Added support for bridged [CATPro2] modules

1.3.0
- Added [U2-R-CPU/CON] support

1.2.0
- Push-Notifications now support live online / offline detection

1.1.0
- Newly connected devices are now added automatically to the [RemoteGUI]
- The matrix connection list can be updated by pressing the refresh button
- Login window appears if no user is logged in on a console
- Error messages when executing commands are now displayed with detailed information

1.0.0
- First release
```


</p>
</details>

--------------

# MobileGUI (iOS & Android) v2.1.0
Last Update Friday the 13th August 2021

<img src="https://raw.githubusercontent.com/tomvalk/RemoteGUI-Releases/main/Mockup_Phone.png" height="25%" width="25%">

[![Generic badge](https://img.shields.io/badge/Screenshots-MobileGUI-orange.svg)](https://github.com/tomvalk/RemoteGUI-Releases/blob/main/Screenshot_MobileGUI/)


<details><summary>Features</summary>
<p>
	
- Full integration of the IP-Control-API command set - connect, disconnect, login, logout etc.
- Automatic detection of all devices connected to a matrix incl. RemoteAccess and U2 devices
- Script builder with lot of API commands - Allows to create, test and save scripts with one click without XML knowledge
- Full customization (color, size, icon etc.) of saved scripts
- PushEventNotfications can be shown as PushNotification for monitoring all conenction without opening the App 
- And much more!
</p>

</details>

<details><summary>Requirements</summary>
<p>

- Android 4.1 or higher
- iOS 8.0 or higher
<br/><br/>
- It's recommended to use the latest G&D firmware in order to use all available functions and features
- The G&D firmware expansion IP-Control-API togehther with an activated Remote-Control-Port: 

```
Webinterface -> 'Your Device' -> Information -> Activated Features
Webinterface -> 'Your Device' -> Configuration -> Network -> Remote-Control -> TCP:xxxxx -> Enabled
```
</p>
</details>

<details><summary>Supported Devices</summary>
<p>
	
```
- ControlCenter-Digital
- ControlCenter-Compact
- ControlCenter-IP 2.0
```
	
</p>
</details>

<details><summary>Changelog</summary>
<p>
	
```
2.1.0
    - Public release
	
2.0.0         
    - Added new CP21 icons 
    - Fixed scripting from sidebar 
    - Overall improvements and bug fixes      
	
1.9.0
     - Added Overview Tab
     - Framework update (background)
     - Overall improvements and bug fixes   
	
1.8.0
    - New sidebar design including:
        - easy script access
        - easy workplace filter
        - show last matrix response
    - New Matrix overview frames with monitoring
    - Overall improvements and bug fixes   

1.7.0
    - Added complete monitoring frame 
    - Small improvements and UI fixes

1.6.0
    - Popups and GUI were visually reworked
    - Added PushNotification for G&D Event-Notifications
    - Overall speed improvements and UI fixes

1.5.0 
    - Added U2(LAN) devices to the GUI   
    - Added visual customization of saved Scripts (via long press)                       
                            
1.4.0 
    - Added Easy Scripting feature to [Script Builder]    
    - Overall improvements and UI fixes
                           
1.3.0
    - "More..." commands now available via long press 
    - Added show/hide Targets to the Workplace filter* 
    - Added haptic feedback 
                            
1.2.0                            
    - Added "More..." commands to Targets and Consoles
    - Overall improvements and UI fixes
                
1.1.0 
    - Added full Script Builder  
    - Added Workplace Filter to GUI                        
                            
1.0.0 
    - First Release                                
```

</p>
</details>

--------------
	
# More examples of how to control G&D devices?
https://github.com/tomvalk/G-D-Scripts
	
https://github.com/tomvalk/G-D-Cortana-Commands
	
--------------
	
# About
## Blog
[G&D RemoteGUI – einfaches Umschalten innerhalb eines KVM-Systems via XML](https://blog.gdsys.de/blog/2020/08/05/gd-remotegui-einfaches-umschalten-innerhalb-eines-kvm-systems-via-xml/) <br/>
[G&D RemoteGUI – easy switching of KVM systems via XML](https://blog.gdsys.de/en/2020/08/05/gd-remotegui-easy-switching-of-kvm-systems-via-xml/) <br/>

## Contributing
For changes or issues, please open an [request](https://github.com/tomvalk/RemoteGUI-Releases/issues) first to discuss what you would like to change. <br/>
	
## Author
Tom Valk   <br/>
State-certified technical engineer and business economist <br/>
Certified specialist trainer (BDVT)

<a href="mailto:valk@live.de?"><img src="https://img.shields.io/badge/Send Mail-%23DD0031.svg?&style=for-the-badge&logo=mail&logoColor=white"/></a>

<a href="https://www.buymeacoffee.com/tomtom1337" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
