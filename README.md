# Use Case
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
