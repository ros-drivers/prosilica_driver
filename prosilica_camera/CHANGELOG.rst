^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package prosilica_camera
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.9.5 (2021-03-23)
------------------
* Merge pull request `#19 <https://github.com/ros-drivers/prosilica_driver/issues/19>`_ from PR2-prime/noetic-devel
  updated settings for noetic compile
* updated settings for noetic compile
* Merge pull request `#15 <https://github.com/ros-drivers/prosilica_driver/issues/15>`_ from jnmacdnld/kinetic-devel
  Remove driver_base dependency as this package is deprecated
* Remove driver_base dependency as this package is deprecated
  Only the SensorLevels message is needed from this package, which is now
  provided by dynamic_reconfigure
* Merge pull request `#11 <https://github.com/ros-drivers/prosilica_driver/issues/11>`_ from athackst/nodelet
  updated prosilica driver to be a nodelet
* returned guard on frameDone in prosilica.cpp
* fixed install in CMakeLists.txt
* Update prosilica_nodelet.cpp
  updated comments
* updated prosilica driver to be a nodelet, added diagnostic messages, and autoadjust streambytespersecond when multiple cameras are connected (can be overwritten by reconfigure)
* Contributors: Allison Thackston, Austin, Dave Feil-Seifer, John Macdonald, athackst

1.9.4 (2014-07-28)
------------------
* Update maintainer email
* Merge pull request `#5 <https://github.com/ros-drivers/prosilica_driver/issues/5>`_ from mitchellwills/fixedrate
  Added support for fixedrate mode
* Moved setting framerate from start to configure so that it is set without needing to restart the stream
* added fixed rate back to dynamic reconfigure cfg
* Implemented fixed rate camera mode
* Contributors: Austin Hendrix, Mitchell Wills, trainman419

1.9.3 (2013-07-11 10:49:48)
---------------------------

1.9.2 (2013-07-11 10:49:16)
---------------------------
* Fix compile warnings.
* Contributors: Austin Hendrix

1.9.1 (2013-06-28)
------------------
* Fix include paths.
* Contributors: Austin Hendrix

1.9.0 (2013-06-27)
------------------
* Clean up.
* Install rules.
* Catkinize.
* Contributors: Austin Hendrix

1.8.2 (2012-10-15)
------------------
* prosilica_camera: fixed link time compile bug
* prosilica_camera: Fixed a boost linking error
* Adding .gitignore files
* Changed maintainer to me (William Woodall - wwoodall@willowgarage.com)
* provide option to set netmask and gateway
* prosilica_camera: Handle cameras which do not support binning. `#5407 <https://github.com/ros-drivers/prosilica_driver/issues/5407>`_
* Fix for auto-gain part of `#5407 <https://github.com/ros-drivers/prosilica_driver/issues/5407>`_. Cameras without auto-gain actually do have the GainMode attribute, but error when you set it to anything but Manual. Instead check for GainAutoMax.
* Enabled new settings from `#5092 <https://github.com/ros-drivers/prosilica_driver/issues/5092>`_ for Fuerte. Added gain_auto_max param.
* prosilica_driver: Updated manifest and stack descriptions for accuracy after AVT acquired Prosilica.
* new stack for Prosilica driver
* Contributors: Jack O'Quin, Patrick Mihelich, William Woodall, Wim Meeussen
