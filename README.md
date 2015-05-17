# mavlink.js

> Collection of JavaScript libraries for the MAVLink protocol


## How To Generate

1) Clone mavlink repository from https://github.com/mavlink/mavlink.git

2) Execute generator tool (it's a python script..):

```shell
python \
  -m pymavlink.tools.mavgen \
  --lang=JavaScript \
  message_definitions/v1.0/{platform}.xml
```

Replace ``{platform}`` with name of autopilot, e.g. ``pixhawk``. The tool creates javascript source files.


3) Copy ``mavlink.js`` and ``jspack.js`` to target folder.
