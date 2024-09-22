PixelOS 14 for Samsung Galaxy A71
------------------------------------

Create directories

	$ mkdir Pixel14
	$ cd Pixel14

Init the base manifest

	$ repo init -u https://github.com/PixelOS-AOSP/manifest.git -b fourteen --git-lfs
  
Add the local manifest

  Take the xml file for your device and copy it to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync 

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch aosp_a71-ap2a-userdebug
	$ mka bacon
