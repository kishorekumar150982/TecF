# TecF
Track touches and swipes and store the corresponding coordinates and timestamps. 
Track keystrokes and store the all typed words and timestamps.
Track screen-size and orientation.
Record the current screen image.
Process several screen images into a space optimized format by taking into account screen size and orientation
Provide application hooks to trigger a screenshot in a current state
 Provide application hooks to add custom events
Send information back to the tracking server. Either immediately or only when connected to
a WIFI network depending on configuration.
Capture metadata about the device, os and screen size

        This  application is useful for getting screenshots information , and video , device information, touch on the screen.

TouchVk.h     class has touches like single touch and taps count, if you want get this , by using   the following methods 
            we call the methods 
                   -(void)swipAction  // 
                   -(void)tapAction  //
                   -(void)distanceSwipe 

DeviceVC      calss contains device information, device id, device os, if you want get this by using the following method getDeviceInfo in our xcode project.
                           we get the following 
                             Deviceid
                             Application Id
                             Device Name
                             Device Resolution
                             App Version
                             Os Version
NetworkVC  :  class checks the device internetconnection, if there is no internet then it will show alert also , we get this by sending information to server.
LaunchTime   : class indicates launch time of the application,if you want get this we are using the following method launchTimerMethod.

ScreenSharing : class has collection of screenshots and that screenshots will convert into videos,if you want get     this by using createScreenshotAndSaveInACustomAlbum

                  we get the following 
                             The screenshot itself in a space efficient format
                             The capture time relative to the session start

SizeVC.h class has collection of orientations like width/height,landscape/portrait
                   we get the following 
                              The Current screen-size(width/height)
                              The Current Orientation (landscape/portrait)


