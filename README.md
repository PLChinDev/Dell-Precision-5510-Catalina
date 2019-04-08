# Dell-Precision-5510-Mojave
* i7-6820HQ  
* Crucial 32GB-DDR4 2667 MHz 
* Samsung SSD 970 EVO 1TB
* HD530 
* DELL-DW1830  
* This repo is based on [soulomoon repo](https://github.com/soulomoon/Dell-Precision-5510-OSX) with the exception of all third party kexts being installed to /Library/Extensions.

# HDMI
To enable hdmi output, you should add   
```
				<key>Mac-A5C67F76ED83108C</key>
				<string>none</string>
```  
under `ConfigMap->dict` in `/System/Library/Extensions/AppleGraphicsControl.kext/Contents/PlugIns/AppleGraphicsDevicePolicy.kext/Contents/Info.plist`  
and rebuild kext cache using 
`sudo kextcache -i /`  
