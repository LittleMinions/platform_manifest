The Little Minions Vacation
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Repo initialization:

    $ repo init -u https://github.com/LittleMinions/platform_manifest.git -b lp5.0
    
Repo initialization for specific device:

    $ repo init -u https://github.com/LittleMinions/platform_manifest.git -b lp5.0 -g all,-notdefault,<devicename>,<vendorname>

 
sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    brunch


You can also build (and see how long it took) for specific devices like this:

    . build/envsetup.sh
    time brunch <device>

Remember to `make clobber` every now and then!
