# Choker

OS X Ruby command line utility for limiting up and down-stream bandwidth on a system wide basis.

Inspired by this super handy blog post by 'Chris vs. Synergy' http://weblog.bbzzdd.com/2010/11/16/throttling-bandwidth-in-mac-os-x/


Uses ipfw and ifconfig.

You must have sudo rights to use.

## Usage

To limit up and down-stream bandwidth to 10Kbps
```
	$ choker throttle --up 10 --down 10
```

To remove all throttling
```
	$ choker unthrottle
```

To remove up-stream throttling only
```
	$ choker unthrottle --down false
```

Disable all network adapters
```
	$ choker disable
```

Re-enable network adapters
```
	$ chocker enable
```

## Todo List

* Package up as a gem
* Neat way to track what rules are in effect
* Linux support