# Dell-Precision-5510-Mojave
- i7-6820HQ 
- HD530 
- 32GB DDR4 2667 MHz 
- Samsung SSD 970 EVO 1TB 
- DELL-DW1830  
- Currently using Clover r4919 beta
- This repo is based on [soulmoon repo](https://github.com/soulomoon/Dell-Precision-5510-OSX) with the exception of all third party kexts being installed to /Library/Extensions

# HDMI
To enable HDMI output, add the key/string to location below:  
```
/System/Library/Extensions/AppleGraphicsControl.kext/Contents/PlugIns/AppleGraphicsDevicePolicy.kext/Contents/Info.plist:
        ConfigMap:
            Dictionary:
                <key>Mac-A5C67F76ED83108C</key>
                <string>none</string>
```   
and rebuild kext cache using 
`sudo kextcache -i /` or [Kext Utility](http://cvad-mac.narod.ru/index/0-4). 

# Credits
- <a class="bbc_url" href="http://cvad-mac.narod.ru/" rel="nofollow external" sl-processed="1" style="color: rgb(15, 114, 218);" title="External link">© cVad 2008-2016</a> for Kext Utility.
