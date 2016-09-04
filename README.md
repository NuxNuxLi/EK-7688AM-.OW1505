# EK-7688AMx.OW1505


## How to build the firmware for EK-7688AMx?

0. [Build the firmware](http://labs.mediatek.com/fileMedia/download/87c801b5-d1e6-4227-9a29-b5421f2955ac#page=97&zoom=auto,70,239)

## How to setup AP-Client mode?

0. Rewrite /etc/config/wireless -- `vi /etc/config/wireless`
   
   ```
   +++option ssid 'RootAP_SSID'
   +++option key 'RootAP_password'
   +++option encryption 'psk2' (ps: RootAP's encryption)
   +++opton disabled '0' (ps: enabled station mode)
   ```

0. Restart network -- `/etc/init.d/network restart`
