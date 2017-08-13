# UI developer demo project 

##UI Technology Stack

- HTML5
- CSS3
- [vuejs](https://vuejs.org)


##Requirement 
We need 2 page and one model popup design based on above stack. 

###Project List Page 
![](https://raw.githubusercontent.com/izinga/UI_DEMO/master/screenshot/project_list.png)
#### API
- [Project list](https://raw.githubusercontent.com/izinga/UI_DEMO/master/json/project_list.json)
```javascript
{
        "5983eb186711e9a944035408": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502392243,
            "os": "deviceOnly",
            "id": "5983eb186711e9a944035408",
            "name": "device"
        },
        "596495a89b9e46a3c497e4de": {
            "admin": [
                "595428049b9e46bb20b63b8f",
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1501750028,
            "os": "android",
            "id": "596495a89b9e46a3c497e4de",
            "name": "Citbank GA Demo"
        },
        "5958c3d49b9e46c55691688d": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1501770859,
            "os": "web",
            "id": "5958c3d49b9e46c55691688d",
            "name": "CNN"
        },
        "5958c5a89b9e46c556916891": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502526184,
            "os": "android",
            "id": "5958c5a89b9e46c556916891",
            "name": "Citibank Aish"
        },
        "596afcea6711e90efe7f5a35": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502254152,
            "os": "android",
            "id": "596afcea6711e90efe7f5a35",
            "name": "locus"
        },
        "598eae936711e9e57c8201c9": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502524561,
            "os": "android",
            "id": "598eae936711e9e57c8201c9",
            "name": "Amazon"
        },
        "595bfb9ecc42cb5504f85b83": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1500209766,
            "os": "iOS",
            "id": "595bfb9ecc42cb5504f85b83",
            "name": "ssss"
        },
        "598327096711e93b9aecd0f9": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502434079,
            "os": "deviceOnly",
            "id": "598327096711e93b9aecd0f9",
            "name": "Device Only"
        },
        "596709ac9b9e46887773751c": {
            "admin": [
                "5954c54e9b9e467b8b713fe7"
            ],
            "lastUsed": 1502254045,
            "os": "android",
            "id": "596709ac9b9e46887773751c",
            "name": "ebay"
        }
    }
```

- [Project image](https://raw.githubusercontent.com/izinga/UI_DEMO/master/json/project_image.json)
```javascript
{
    "result": "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"
}
```
###Project  Page 
![](https://raw.githubusercontent.com/izinga/UI_DEMO/master/screenshot/project_detail.png)
#### API
- [Project Detail](https://raw.githubusercontent.com/izinga/UI_DEMO/master/json/project_detail.json)

###Device Selection Model PopUp
![](https://raw.githubusercontent.com/izinga/UI_DEMO/master/screenshot/device_select.png)
#### API
- [Devcie List](https://raw.githubusercontent.com/izinga/UI_DEMO/master/json/device_list.json)
```javascript
{
    "available": [
        {
            "_id": "596244f4b996c838ffc76a57",
            "serial": "0123456789ABCDEF",
            "key": "",
            "uiid": "",
            "host": "127.0.0.1",
            "name": "Lenovo A536",
            "brand": "Lenovo",
            "model": "",
            "model_id": "Lenovo A536 - 4.4.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "4.4.2",
            "isConnected": true,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "480x854",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [
                "8951071001",
                "234353446"
            ],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": null,
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Browser",
                    "component": "com.android.browser/.BrowserActivity"
                },
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "_id": "127.0.0.1",
                "name": "Mac Mini",
                "ip": "127.0.0.1",
                "location": "Bangalore",
                "status": true,
                "version": false,
                "os": "darwin",
                "serial": "",
                "macAddress": "",
                "created": "2017-08-07T21:29:58.578+05:30",
                "updated": "2017-08-12T13:36:18.766+05:30",
                "last": 1502614637
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1502526889,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        }
    ],
    "busy": [],
    "offline": [
        {
            "_id": "59609077b996c838ffc6f692",
            "serial": "21b7a936d2cdae25bc3ecedf548b3c44c4982a38",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "iPhone 5s",
            "brand": "Apple",
            "model": "",
            "model_id": "iPhone 5s - 10.3.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "10.3.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "0x0",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "iOS",
            "port": 0,
            "screenmode": "default",
            "ratio": 1,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1499767545,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "59649127b996c838ffc8a191",
            "serial": "0255e9ff78752644",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "Nexus 5X",
            "brand": "google",
            "model": "",
            "model_id": "Nexus 5X - 7.1.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "7.1.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "1080x1920",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1499791844,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "5964a2f9b996c838ffc8fe77",
            "serial": "2002cc354587ca26bfe21c0cb36e6f6e6861b9da",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "iPhone 5c",
            "brand": "Apple",
            "model": "",
            "model_id": "iPhone 5c - 10.3.2",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "10.3.2",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "0x0",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "iOS",
            "port": 0,
            "screenmode": "default",
            "ratio": 1,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1502119321,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        },
        {
            "_id": "596debc1023f3553c0142785",
            "serial": "074536210b3008e9",
            "key": "",
            "uiid": "",
            "host": "",
            "name": "Nexus 5",
            "brand": "google",
            "model": "",
            "model_id": "Nexus 5 - 6.0.1",
            "manufacturer": "",
            "clientidbase": "",
            "countryCode": "",
            "ram": "",
            "fingerprint": "",
            "version": "6.0.1",
            "isConnected": false,
            "testSession": "",
            "simOperator": "",
            "timezone": "",
            "resolution": "1080x1920",
            "lcdDensity": "",
            "screensize": "",
            "img": "",
            "numbers": [],
            "useType": [
                "M",
                "A",
                "H"
            ],
            "projects": [],
            "user": "",
            "os": "Android",
            "port": 0,
            "screenmode": "default",
            "ratio": 2,
            "menubar": false,
            "status": false,
            "state": 0,
            "automate": false,
            "browsers": [
                {
                    "name": "Chrome",
                    "component": "com.android.chrome/com.google.android.apps.chrome.Main"
                }
            ],
            "apps": null,
            "display": {
                "width": 0,
                "height": 0,
                "xdpi": 0,
                "ydpi": 0,
                "size": 0,
                "density": 0,
                "fps": 0,
                "secure": false,
                "rotation": 0
            },
            "imei": "",
            "imsi": "",
            "iccid": "",
            "phoneNumber": "",
            "network": "",
            "reserveKey": "",
            "usage": null,
            "node": {
                "name": "",
                "ip": "",
                "location": "",
                "status": false,
                "version": false,
                "os": "",
                "serial": "",
                "macAddress": "",
                "created": "0001-01-01T00:00:00Z",
                "updated": "0001-01-01T00:00:00Z",
                "last": 0
            },
            "other": "",
            "minicap": {
                "state": 0
            },
            "minitouch": {
                "state": 0
            },
            "service": {
                "state": 0
            },
            "agent": {
                "state": 0
            },
            "nizedha": {
                "state": 0
            },
            "vnc": {
                "state": 0
            },
            "last": 1502525117,
            "created": "0001-01-01T00:00:00Z",
            "updated": "0001-01-01T00:00:00Z"
        }
    ],
    "reserved": []
}
```

### Support 
For best practices please refer [examples](https://vuejs.org/v2/examples/)

