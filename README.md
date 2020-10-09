# Recovery Controller /L Unofficial

Better integration between FMRS and Stage Recovery.

Unofficial fork by Lisias.


## In a Hurry

* [Latest Release](https://github.com/net-lisias-kspu/RecoveryController/releases)
	+ [Binaries](https://github.com/net-lisias-kspu/RecoveryController/tree/Archive)
* [Source](https://github.com/net-lisias-kspu/RecoveryController)
* Documentation
	+ [Project's README](https://github.com/net-lisias-kspu/RecoveryController/blob/master/README.md)
	+ [Install Instructions](https://github.com/net-lisias-kspu/RecoveryController/blob/master/INSTALL.md)
	+ [Change Log](./CHANGE_LOG.md)
	+ [TODO](./TODO.md) list


## Description

In a nutshell, right-click on decouplers to show the properties, and click the Stage-Recovery button to cycle between the different available mods.

This will enable you to select which mod controls the decoupled stage.

Available settings are:

* auto - Let FMRS decide depending on it's options whether it will take control or not
* none - No mod should control this stage after staging
* FMRS - FMRS has control of this stage
* Stage Recovery - Stage Recovery has control of the stage

By definition, setting "auto" with this Add'On will do the same thing as not having it installed, which is why "auto" is the default.

**Without this/"Auto" mode**: When using the default settings of StageRecovery and FMRS, FMRS will handle all stages with parachutes, probes, or Kerbals exclusively while FMRS is active. If you close the FMRS window or make FMRS not active, then StageRecovery will handle ALL stages as if FMRS were not installed. FMRS has two settings that can affect this behaviour: one which makes FMRS not handle parachutes at all and another that defers parachute recovery to StageRecovery. If either of these are active then StageRecovery will handle stages with only parachutes (so no probe or kerbals on board) while FMRS handles probes and kerbals (again, only if FMRS is active).

**With this**: By changing the "Recovery Controller" on the decoupler it sets which Add'On will attempt to handle everything up to the next decoupler in the part list (which is also how StageRecovery tracks stages in the editor, so you can use the highlighting feature if you're not 100% positive what's included). Using this you can have StageRecovery recover something with a probe core and FMRS handle something with parachutes (even if FMRS's settings defer chute stages to SR), or you can use "none" to have neither mod attempt to handle recovery if you really don't want something recovered.

The settings you make should be saved with the craft. If you use sub-assemblies they should be saved with those as well.

There are a few cases where things might act different from expected. For instance, if you designate FMRS to handle a stage but FMRS is disabled, StageRecovery won't try to handle it. 

[This is a video ](https://www.youtube.com/watch?v=IGgyLM6ca_M)showing how the two Add'Ons interact without RecoveryController (or in "auto" mode) and how RecoveryController allows you to have substantially more control over how your stages get recovered.

([source](https://forum.kerbalspaceprogram.com/index.php?/topic/158970-19x-recoverycontroller-let-fmrs-and-stagerecovery-work-together/&do=findComment&comment=3015910))


## Installation

Detailed installation instructions are now on its own file (see the [In a Hurry](#in-a-hurry) section) and on the distribution file.

## License:

This plugin is licensed under the [MIT](https://opensource.org/licenses/MIT) license. See [here](./LICENSE).

Please note the copyrights and trademarks in [NOTICE](./NOTICE).


## UPSTREAM

* [linuxgurugamer](https://forum.kerbalspaceprogram.com/index.php?/profile/129964-linuxgurugamer/) ROOT
	+ [Forum](https://forum.kerbalspaceprogram.com/index.php?/topic/158970-*)
	+ [SpaceDock](https://spacedock.info/mod/1311/RecoveryController)
	+ [Github](https://github.com/linuxgurugamer/RecoveryController/)
