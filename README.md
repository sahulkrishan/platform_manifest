[Android Open Source Cypher Project]
====================================

Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.


Initializing Repository
-----------------------

Initiate trees with Sony Xperia Z2 (Sirius) trees.

    $ repo init -u https://github.com/sahulkrishan/platform_manifest.git -b oreo-mr1-release

Sync the repository:

    $ repo sync --force-sync

***


Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    
    brunch
    
    Pick your device by typing it's number followed by enter

You can also build for specific devices (eg. sirius) like this (make sure to add the device in aoscp.devices!):

    . build/envsetup.sh

    brunch aoscp_sirius-userdebug

Remember to `make clobber` every now and then!

