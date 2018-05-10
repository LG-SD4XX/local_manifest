LineageOS 14.1 for LG-SD4XX Devices
------------------------------------

Create directories

	$ mkdir cm-14.1
	$ cd cm-14.1

Init lineage:

	$ repo init -u git://github.com/LineageOS/android.git -b cm-14.1
  

Pick your device:

ph2n = Lg Stylo 2 Plus

sf340n = Lg Stylo 3 Plus

lv517 = Lg K20 Plus

Download and move the manifest xml for the device you want to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync -q

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_DEVICENAME-userdebug
	$ mka bacon
