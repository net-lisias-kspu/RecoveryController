# Recovery Controller /L Unofficial

This mod allows funds to be recovered, at a reduced rate, from dropped stages so long as they have parachutes attached (not necessarily deployed).


## Installation Instructions

To install, place the GameData folder inside your Kerbal Space Program folder. Optionally, you can also do the same for the PluginData (be careful to do not overwrite your custom settings):

* **REMOVE ANY OLD VERSIONS OF THE PRODUCT BEFORE INSTALLING**, including any other fork:
	+ Delete `<KSP_ROOT>/GameData/RecoveryController` if existent
	+ Delete `<KSP_ROOT>/GameData/net-lisias-ksp/RecoveryController`
* Extract the package's `GameData` folder into your KSP's root:
	+ `<PACKAGE>/GameData` --> `<KSP_ROOT>/`
* Extract the package's `PluginData` folder (if available) into your KSP's root, taking precautions to do not overwrite your custom settings if this is not what you want to.
	+ `<PACKAGE>/PluginData` --> `<KSP_ROOT>/`
	+ You can safely ignore this step if you already had installed it previously and didn't deleted your custom configurable files.

The following file layout must be present after installation:

```
<KSP_ROOT>
	[GameData]
		[net-lisias-ksp]
			[RecoveryController]
				CHANGE_LOG.md
				LICENSE
				NOTICE
				README.md
				StageRecovery.version
				...
		000_KSPe.dll
		ModuleManager.dll
		...
	[PluginData]
		[net-lisias-ksp]
			[RecoveryController]
				...
	KSP.log
	PastDatabase.cfg
	...
```


### Dependencies

* [KSP API Extensions/L](https://github.com/net-lisias-ksp/KSPAPIExtensions)
	+ **Not Included** 
