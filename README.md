# "Cmd Trigger" Plugin

Example config.json with custom delay (in ms) to turn off the switch:

```
    "accessories": [
        {
          "accessory": "CmdTrigger",
          "name":      "My command",
          "command":   "echo Hello World",
          "delay":   "10000",
          "execAfterDelay": false
        }
    ]

```

Example config.json with stateful switch:

```
    "accessories": [
	    {
	        "accessory": "CmdTrigger",
	        "name":      "Stafeful Switch",
	        "command":   "dummy",
	        "stateful":   true,
	        "debug":      false
	    }
    ]
```

With Cmd Trigger plugin you can create any number of fake switches that will execute a CLI command when turned on or after delay (and will automatically turn off right afterward, simulating a stateless switch). This can be used to trigger command and scripts on a server running Homebridge via HomeKit. For example by telling Siri to backup your documents.

You can also use this plugin as fakeswitch with custom delay, or as a stateful switch.

This plugin was created by extending homebridge-dummy plugin: https://github.com/nfarina/homebridge-dummy.

# Installation instructions

```
$: npm -g install homebridge-cmdtrigger
```
