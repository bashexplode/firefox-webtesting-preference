These are helpful settings to use if you are testing web applications that disable telemetry and other unnecessary settings.

This was based off of a privacy profile by /u/alphabetcereal on Reddit. The privacy profile had a few things that would make web application testing more difficult like geo tracking and cookie tracking, so those were removed or commented out.


The local-settings.js file should be saved to:
| Operating System | Directory Path                                               | 
| ---------------- |:------------------------------------------------------------:|
| Windows          | C:\Program Files (x86)\Mozilla Firefox\defaults\pref         |
| macOS            | /Applications/Firefox.app/Contents/Resources/defaults/pref   |



The mozilla.cfg file should then be placed in the follow directory:
| Operating System | Directory Path                                 | 
| ---------------- |:----------------------------------------------:|
| Windows          | C:\Program Files (x86)\Mozilla Firefox         |
| macOS            | /Applications/Firefox.app/Contents/Resources   |


Remove annoying "Update available" pop up box via Windows Registry:  
`HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Mozilla\Firefox` -> Add new DWORD (32-bit) Value of `DisableAppUpdate` -> Set value data to `1`  


---

### References:

Original Reddit post on privacy profile: https://www.reddit.com/r/privacytoolsIO/comments/d3of43/firefox_privacy_guide/

Privacy profile: https://zerobin.net/?d500be36ece372ff#GNhUiCDf9orkCpL2Pgta6CuocE/eNCnmVs2by28Kx6s=
