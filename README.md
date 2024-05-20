# Hackintosh-Config-Lenovo-IdeaPad-3I_10110U

# <br/>**Remembering that the intention is to help and not steal someone else’s project!! All credits go to the original author.**<br>

## <br/>This configuration was adapted for the Lenovo Ideapad 3I with the 10100U processor so that some things work well.<br>

<br>Opencore was updated to 1.0.0 and all kexts too, CPUFriendFriend was used to fix the temperature and high battery consumption<br/>

<br>**Things that work with the original author's default configuration:**<br/>

  - *Webcam (Lenovo UVC Camera)*
  - *Touchpad (ELAN I2C)*
  - *HDMI (Audio + Video)*
  - *Brightness Control (F11/F12 Keys)*
<br/><br/>

**Things that work in my setup:**

  - *CPU (Intel Core i3-10110U)*
  - *Audio (Realtek ALC257)*
  - *USB (Comet Lake PCH-LP USB 3.1)*
  - *Sleep*
<br/><br/>
 
*CPU (Intel Core i3-10110U)*
> *Now power management works perfectly, even allowing the user to see the CPU temperature and also having low power consumption*

*Audio (Realtek ALC257)*
> *Only the layout-id was corrected*

*USB (Comet Lake PCH-LP USB 3.1)*
> *It worked in the default configuration, however, it caused problems with sleep*

*Sleep*
> *Now works perfectly*

<br/>Command to fix sleep in Monterey:<br/>
`sudo pmset -a tcpkeepalive O standby O hibernatemode 25 womp 0`

> [!IMPORTANT]
> It is recommended that you reset NVRAM only once after configuring sleep.

ACPI patches I made:
 - *SSDT-DATA*
 - *SSDT-USBX*
 - *SSDT-RHUB (Just redone to avoid hardware problems)*
 - *SSDT-AWAC*
 - *SSDT-HPET*
 - *SSDT-UIAC*
 - *SSDT-RTCAWAC*
