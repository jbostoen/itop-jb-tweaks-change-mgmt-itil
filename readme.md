# jb-tweaks-change-mgmt-itil

Copyright (C) 2019-2021 Jeffrey Bostoen

[![License](https://img.shields.io/github/license/jbostoen/iTop-custom-extensions)](https://github.com/jbostoen/iTop-custom-extensions/blob/master/license.md)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/jbostoen)
🍻 ☕

Need assistance with iTop or one of its extensions?  
Need custom development?  
Please get in touch to discuss the terms: **info@jeffreybostoen.be** / https://jeffreybostoen.be

## What?

Modifies Change:
* prevents automatic computation of impacted items (computed). Often undesired: if you manually add a core switch, this could add a lot of 'computed' items which are also impacted - which makes it less obvious to see the ones that really matter (manually added). The tab 'impact analysis' still works the same.
* adds 'reminder' field (only visible for NormalChange)

Modified NormalChange:
* allows to not specify an acceptance_comment

Modifies NormalChange, RoutineChange:
* always allow 'reject', even further in the process

Modifies EmergencyChange, NormalChange and RoutineChange:
* prevent 'title' from becoming read-only when state changes to 'implemented'
* prevent 'private_log' from becoming read-only when state changes to 'closed'
* prevent 'impact' from being mandatory
* make fallback default to 'restore from backup'

## Cookbook

XML
* add field to existing class
* change default value for field
* override a method
* override a property
