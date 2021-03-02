#Tract same issue from different activities, under one logcat filter

# Use Case

Logs from different Activities https://github.com/SanthoshMKunthe/Multiple-Logs-Android/blob/master/OUTPUT.png by using same LOGCAT FILTER key. . .
We all use debug logs. . . But I hate to type capital 'L' while typing 'Log.d' and also TAG remains same for that particular activity. . .

If I want to see Logs across different activities then filtering Logs based on TAG is not useful as TAG will only show me Log of one particular activity. . .

So I have created this that can show logs across different activities and has 10 types. . .

# How To Use

In Project level gradle-->

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
  In app level gradle-->
  
    dependencies {
            implementation 'com.github.SanthoshMKunthe:Multiple-Logs-Android:1.4.5'
    }

import live.mkunthe.simplelogging.smkl;

smkl.a("All logs related to user email,password etc. . ."); in different activities like Splash,Login,Main etc and when you filter in logcat you will get all logs accross different activities. . .

smkl.b("All logs related to database connection. . .");

smkl.c("All logs related to a particular bug. . .");

.

.

.

smkl.j("All logs related to a particular issue. . . From across different activities. . . Under one Logcat Filter. . .");

Screenshot --> https://github.com/SanthoshMKunthe/Multiple-Logs-Android/blob/master/OUTPUT.png
#Tract same issue from different activities, under one logcat filter
