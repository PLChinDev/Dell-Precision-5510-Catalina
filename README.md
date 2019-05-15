# Dell-Precision-5510-Mojave
* Intel i7-6820HQ 
* Intel HD530 
* Crucial 32GB DDR4 2667 MHz
* Samsung SSD 970 EVO 1TB 
* Dell DW1830  
* macOS Mojave 10.14.5
* Clover r4928 beta
* This repo is based on
[soulomoon repo](https://github.com/soulomoon/Dell-Precision-5510-OSX) with the exception of all third party kexts being installed in /Library/Extensions

# HDMI
To enable HDMI output, add   
```
				<key>Mac-A5C67F76ED83108C</key>
				<string>none</string>
```  
under `ConfigMap->dict` in `/System/Library/Extensions/AppleGraphicsControl.kext/Contents/PlugIns/AppleGraphicsDevicePolicy.kext/Contents/Info.plist`  
and rebuild kext cache using 
`sudo kextcache -i /`.  
