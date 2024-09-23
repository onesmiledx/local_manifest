RisingOS for Samsung Galaxy A71
------------------------------------

Create directories

	$ mkdir Rising14
	$ cd Rising14

Init the base manifest

	$ repo init -u https://github.com/RisingTechOSS/android -b fourteen --git-lfs
  
Add the local manifest

  Take the xml file for your device and copy it to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync 

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ riseup a71 userdebug
	$ rise b
