Android Broadcast Receiver Sample APP
==============

This sample code will help developer to quick integrate your app to work with Qmote app by simply receiving the broadcast intent sent from Qblinks Qmote Android App.

Since Qmote Android App **version 5.0.3**, it sends broadcast message for every Qmote activities. You can implement broadcast message receiver in your app, and your app will work with Qmote nicely.


###Broadcast Intent Format

Action Name: “QmoteCommand”
Key:   “QmoteClick”
Value:
       “lss”   as long-short-short-short “lsss” 
       “lls”   as long-long-short
       “sls”   as short-long-short
Value:
      Standtard Address such as “54:4A:16:77:C9:2F”

1. Function getQmote() will get Qmote addresses in Bluetooth system.
Then you can know the addresses you expected to see in your receiver.

2. Include a BroadcastReceiver to receive Qmote click.