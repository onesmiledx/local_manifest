PixelOS 14 QPR3 for Samsung Galaxy A71
------------------------------------

Create directories

	$ mkdir Pixel14  
	$ cd Pixel14

Init the base manifest

	$ repo init -u https://github.com/PixelOS-AOSP/manifest.git -b fourteen --git-lfs --depth=1
  
Add the local manifest

  Take the xml file and copy it to .repo/local_manifests/

Then sync up with this command:

	$ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_a71-ap2a-userdebug
	$ mka bacon
