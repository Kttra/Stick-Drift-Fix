# Stick Drift Fix
GPC script made to stop stick drift on the right analog stick. It is possible to edit the code to take into account the left stick or to lax the deadzones in place. This is just an example of stopping the right stick from drifting upwards by itself. I highly suggest replacing your controller instead of relying on this script because it may effect your accuracy in the long run.

However, this script will serve as a baseline to allow your controller to function properly until you get a replacement. The program at default is set to prevent your stick from drifting upwards because that is the most common stick drift issue. This fix is not permanent and is only active if you're connected through a TitanTwo device (and using the profile with this script) or anything that can support gpc. 

**Finding Deadzone Values**
----------------------------------------------------------------------------------------------------------------------------
First of all, it's important to know what a deadzone is on a controller. The higher the deadzone value, the larger the “dead zone” of the analog stick. When the value is set at zero, the joystick will respond to any and all joystick movement. A value higher than zero will create a zone where input will not be registered.

I have set the current deadzone to 80 on the right stick for upwards input. So on the right stick, if an upwards value of 80 or below is received, it will not be outputted. However if an output of 80 or above is received, it will be outputted. You may want to check your particular problem through the device monitor.

In the video below, the left side represents the inputs made realtime while the right side and center is what the device will output. In the video, notice that the right analog stick is being pushed upwards and how it will not be registered until it hits the -80 to -100 range. These values are set to be outside of our deadzone threshold. You can check your drift values using the monitor and adjust your deadzone thresholds accordingly. Note that your drift values may vary heavily from time to time, so take that into account.

https://user-images.githubusercontent.com/100814612/159133741-3211bb21-a764-4c35-a246-3546cea17b90.mp4
