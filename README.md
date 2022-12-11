# gtaxlwifi_vendor_tree

you need to add below xml to your manifest file under .repo/local_manifests/roomservice.xml <br/>
<project name="srampv/gtaxlwifi_device_tree.git" path="device/samsung/gtaxlwifi" remote="github" /> <br/>
 <project name="srampv/gtaxlwifi_vendor_tree.git" path="vendor/samsung/gtaxlwifi" remote="github" /> <br/>
  <project name="srampv/gtaxl_wifi_hardware.git" path="hardware/samsung" remote="github" /> <br/>
  
  and then run below steps
  
     26  git clone https://github.com/srampv/android_device_samsung_gtaxlwifi.git
   27  cd android_device_samsung_gtaxlwifi/
   28  ls -lrt
   29  cd ..
   30  cp -r android_device_samsung_gtaxlwifi/* ~/android/lineage/device/samsung/gtaxlwifi/
   31  git clone https://github.com/srampv/android_kernel_samsung_exynos7870.git
   32  git clone https://github.com/srampv/gtaxl_wifi_hardware.git
   33  mkdir -p ~/android/lineage/kernel/samsung/exynos7870

   35  git clone https://github.com/srampv/gtaxlwifi_vendor_tree.git
   36  cp -r gtaxlwifi_vendor_tree/* ~/android/lineage/vendor/samsung/gtaxlwifi/
   37  cp -r gtaxl_wifi_hardware/*  ~/android/lineage/hardware/samsung/
   38  git clone https://github.com/srampv/gtaxlwifi_device_tree.git
   39  cp -r gtaxlwifi_device_tree/* ~/android/lineage/kernel/samsung/exynos7870/

  source build/envsetup.sh<br/>
  ~/bin/repo sync <br/>
  breakfast gtaxlwifi<br/>
  brunch gtaxlwifi<br/>
