
## AJAX Enumeration (API Pentesting)
Same endpoint as in UZ801, but the Jetty server APK indicates those additional `funcNo`s:

|funcNo|Description|Arguments         |Example Req|Example Resp| Related URL/Remarks |
|------|-----------|------------------|-----------|------------|-------------|
| 2003 | Set SIM Slot ? | -       |```{"funcNo":2003,"simslot":"1","password":"abc"}```|```{"error_info":"password error!","flag":"0"}``` | Password is hard-coded to `admin8888`. This variation actually calls some function `this.mWanDataController.setSimSlot(1);`.|
| 3000 | Force Update | -          |```{"funcNo":3000}``` | | Should do a No-MD5 update on `/data/update.zip`. Saves config to `/data/mificonfig.json` before updating.|
| 3001 | Remove Update file | -          |```{"funcNo":3001}``` | ```{"flag":"0"}``` | Tries to remove `/data/update.zip`. 1 means the file does not exist anymore, 0 if it still exists (removal failed).|
| 3002 | Query device name + SW version | -          |```{"funcNo":3002}``` |  | Returns `device_name` and `sw_version`.|

