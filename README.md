*** Requiem for Kingsmouth Code Repository ***
This respository holds all the MUSHCode I've written.
I've built this game from the ground up; two months to write CharGen (Currently in Version 1.10).
Updated README on 10/9. Game currently under development since Oct 2013.

RfK Version 1.10 - 8/30/2014
Additions:
 o Damage code.(+damage)
 o Automatic donation of RP to players on the 1st of the month
 o Sendhome checking code in update handler.
 o Add punisher to mask/dirge list.
 o Healing Code (+heal #ofVitae)
	o Humans regain 1 WP at Dawn automatically
	o Humans/Ghouls heal all Bashing and reduce 1 lethal to bashing at Dawn automatically.
 o Messages to WP gain and healing @ dawn.
 o Roll to job.
 o Downtime code.
 o set_flag function.
 o Hunt chan
 o Lorekeeper to merit free text
 o Feeding from players
 
Bugfixes:
 o More alignment/display problems with csheet
 o alignment/display problems with status
 o Update CG approval to set willpower to max
 o Add contacts to merit ft list
 o Fix bug where merits were not removing correctly after reducing merit to 0. (Updates CG to v1.10)
 o Change dawn to act like Dusk and player login.
 o Cheap hack added to set_hp for bug in healing code.
 o Fix dawn/dusk so they trigger for all players.
 
Changes:
 o Trim the trailing 0 on set_hp core function.
 o change in vamp_hunger to check for cg approval.
 o update lattr in update_handler
 o Changed update_handler & update functions to only parse mwho() once
 o Removed PC_DATA`STATUS`VITAE.MAX from cg approval finalization as it is no longer needed. This is calculated by get_vitae(player,max) depending on their BP merit.
 o Add bonus to hunting dicepools from disciplines.
 o Change bloodpools to refill daily
 o Modify wizset to add /misc category, moved beats to misc and added various other items to set.
 o Add contacts to merit ft list.
 o Changed +available to also toggle unfindable flag.
 o Change producer merit to human only.
 o Move rituals & ritual themes under specialties on csheet.
 o Correct regex for roll2
 o Update CG stat selection description
 o Moved event functions in update handler.
 o Change dawn/dusk functions to trigger all related events.
 o Update roll to job to include extra dice.

Pending for release in RfK v.Next:
 o New herd code
 
RfK Version 1.06 (5/10/14)
Additions:
 o Posebreak code & related hooks
 o Chance die to current dice roller.
 o Add set_hp and set_vitae to CoreV1.01
 o New commands: +vitae, +hunt, +map, +nom, +willpower
 o Bloodpools for hunting & code to automatically fill bloodpools.
 o Dawn/Dusk times added to Cron
 o Added Tick to game, currently only checks Vamp Hunger
 o Auto-Wake code spends 1 vitae automatically when waking daily.
 o Wizset
 
Bugfixes:
 o Fixed Several +csheet bugs related to alignment of text and correcting display.
 o Fixed missing brace in Condition Code
 o Corrected attribute in condition code
 
Changes:
 o Removed allies free text as mandatory in CG Merits
 o Fixed incorrect text & description on extra dice rolls.
 o Core-1.01: Removed nasty hasattrval checks & added new attribs to PlayerParent.
 o Changed Mastermind/Minion to Hardcore/Casual.
 o Covenant-Specific checks to bboards
 
 
RfK Version 1.00 (2/13/14)
 o Initial commit to Bitbucket.
 o Opened MUSH
 
 o CharGen v 1.09
	* See changes posted on bboard.
	

** PLEASE ** Document all changes in the ChangeLog for tracking!!
Thank you!
