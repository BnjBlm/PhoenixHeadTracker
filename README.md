# PhoenixHeadTracker
The Phoenix Head Tracker is a program that interfaces with Nreal Air glasses to capture and analyze sensor data. By detecting changes in the user's head yaw and pitch, this program can control the movement of the computer mouse on screen (You wil need to implement), which can be used to play video games that use mouse look feature. You can also use this feature with Nreal Air 3D SBS mode


# How to use
Connect your Nreal Air glasses to your PC using the USB-Type C connector. Start Phoenix Head Tracker and click on 'Connect Nreal Air'. Wait 5+ seconds for the sensors to adjust. Then use the sliders to match the 'Raw Yaw' to 'Match Yaw' and 'Raw Pitch' to 'Match Pitch'. You want to Match Yaw and Pitch so when you turn your head with glasses on it should turn 90 degrees. This is based on your screen resolution. As an example, if the 'Raw Yaw' is saying 90 degree when you have you glasses on, then you should 'Match Yaw' to roughly 90 degree also.

![phoenixheadtracker](https://user-images.githubusercontent.com/129109589/228048186-b8acbd7c-5d1a-4be6-b215-1a3ed18b1120.png)

# How to build using Visual Studio 22
PhoenixHeadTracker is based on the AirAPI_Windows.dll :https://github.com/MSmithDev/AirAPI_Windows: You will find the AirAPI_Windows.dll and hidapi.dll in the PhoenixHeadTracker/bin/x64/Debug/ folder. These two files are required in order to connect to Nreal Air glasses.



Once you clone the project, open in Visual Studio 22 by clicking on PhoenixHeadTracker.sln. Make sure you set to build on x64 and debug.Then simply click on start.

![visualstudio22](https://user-images.githubusercontent.com/129109589/228050319-965458a1-af36-466a-8aa7-c45364bc91dd.png)


Make sure that both AirAPI_Windows.dll and hidapi.dll are in the debug folder. I have included them with project.

![Screenshot 2023-03-27 145335](https://user-images.githubusercontent.com/129109589/228051761-b6afc531-5881-4ea3-b935-c2c07860951e.png)

