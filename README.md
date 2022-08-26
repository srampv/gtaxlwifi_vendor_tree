# gtaxlwifi_vendor_tree

you need to add below xml to your manifest file under .repo/local_manifests/roomservice.xml <br/>
<project name="srampv/gtaxlwifi_device_tree.git" path="device/samsung/gtaxlwifi" remote="github" /> <br/>
 <project name="srampv/gtaxlwifi_vendor_tree.git" path="vendor/samsung/gtaxlwifi" remote="github" /> <br/>
  <project name="srampv/gtaxl_wifi_hardware.git" path="hardware/samsung" remote="github" /> <br/>
  
  and then run below steps
  
  source build/envsetup.sh<br/>
  ~/bin/repo sync <br/>
  breakfast gtaxlwifi<br/>
  brunch gtaxlwifi<br/>
