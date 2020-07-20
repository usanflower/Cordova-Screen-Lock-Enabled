ABarak64/Cordova-Screen-Lock-Enabled 
api level 23+ error 

## Cordova-Screen-Lock-Enabled
--

This is a Cordova plugin to determine if a device has a screen lock set for getting in. The majority of the code was cribbed from various platform-specific StackOverflow questions.

#### Supported Platforms

* iOS > 8.0
* Android > 4.1

#### Installing

Install with Cordova cli

    $ cordova plugin add https://github.com/usanflower/cordova-screen-lock-enabled.git
	
#### Usage

* After getting deviceReady event;

```javascript
screenLock.isScreenLockEnabled(success, failure);

function success(result) {
	if (result) {
		console.log('this device has screen lock enabled.');
	} else {
		console.log('this device does not have screen lock enabled.');
	}
};

function failure(err) {
	console.log("Error " + err);
};
```
