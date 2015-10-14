# Android Activity life Cycle
an explanation of android activity lifeCycle for beginners 


# Activity have six states
	1- Created
	2- Started
	3- Resumed
	4- Paused
	5- Stopped
	6- Destroyed

# Activity lifecycle have seven methods
	1- onCreate()
	2- onStart()
	3- onResume()
	4- onPause()
	5- onStopped()
	6- onRestart()
	7- onDestory()


# Situations

**When open the app**

onCreate() --> onStart() -->  onResume()

**When back button pressed and exit the app**

onPaused() -- > onStop() --> onDestory()

**When home button pressed**

onPaused() --> onStop()

**After pressed home button when again open app from recent task list or clicked on icon**

onRestart() --> onStart() --> onResume()

**When open app another app from notification bar or open settings**

onPaused() --> onStop()

**Back button pressed from another app or settings then used can see our app**

onRestart() --> onStart() --> onResume()

**When any dialog open on screen**

onPause()

**After dismiss the dialog or back button from dialog**

onResume()

**Any phone is ringing and user in the app**

onPause() --> onResume() 

**When user pressed phone's answer button**
onPause()

**After call end**

onResume()

**When phone screen off**

onPaused() --> onStop()

**Again screen on**

onRestart() --> onStart() --> onResume()
