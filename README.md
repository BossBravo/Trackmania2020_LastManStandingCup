# Trackmania 2020 : Last Man Standing Cup
Last man standing gamemode for Trackmania 2020. Original idea by https://twitter.com/LuckersTurbo

The Last Man Standing cup mode consists of a series of races on multiple maps. When you finish a race in a bad position, you lose points substracted from your total. Servers might propose warmup races to get familiar with a map first. The more you have a bad position, the more points you lose. To win, you must be the last player with points. Once you are a finalist, if you finish a race last you will be eliminated. The cup mode ends once there is one player left.

Settings are same than a cup mode, exept the _S_PointsLimit_ that became _S_PointsStartup_ :


***Default settings :***

_S_PointsStartup_ 50 => "Points at start"

_S_FinishTimeout_ -1 => "Finish timeout"

_S_RoundsPerMap_ 5 => "Number of rounds per map, Number of round to play on one map before going to the next one"

_S_NbOfWinners_ 1 => "Number of winners"

_S_WarmUpNb_ 0	=> "Number of warm up"

_S_WarmUpDuration_ 20 => "Duration of one warm up"

_S_WarmUpTimeout_ -1 => "Warm up timeout"

_S_PointsRepartition_ "1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20"

_S_DNF_LossPoints_ 20 => "Number of points for player that give up a round"



# How to Use
***Install***

Download the LastManStandingCup.Script.txt file and put it on the dedicated server inside UserData/Scripts/Modes/Trackmania/

***MatchSetting Example***
```
<?xml version="1.0" encoding="utf-8" ?>
<playlist>
	<gameinfos>
		<game_mode>0</game_mode>
		<script_name>Modes/Trackmania/LastManStandingCup</script_name>
	</gameinfos>

	<mode_script_settings>
		<setting name="S_PointsStartup" type="integer" value="50"/>
		<setting name="S_FinishTimeout" type="integer" value="-1"/>
		<setting name="S_RoundsPerMap" type="integer" value="5"/>
		<setting name="S_NbOfWinners" type="integer" value="1"/>
		<setting name="S_WarmUpNb" type="integer" value="0"/>
		<setting name="S_WarmUpDuration" type="integer" value="20"/>
		<setting name="S_WarmUpTimeout" type="integer" value="-1"/>
		<setting name="S_PointsRepartition" type="text" value="1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20"/>
		<setting name="S_DNF_LossPoints" type="integer" value="20"/>
	</mode_script_settings>

	<startindex>0</startindex>
	<map><file>Campaigns/CurrentQuarterly/Summer 2021 - 01.Map.Gbx</file></map>
	<map><file>Campaigns/CurrentQuarterly/Summer 2021 - 02.Map.Gbx</file></map>
	<map><file>Campaigns/CurrentQuarterly/Summer 2021 - 03.Map.Gbx</file></map>
	<map><file>Campaigns/CurrentQuarterly/Summer 2021 - 04.Map.Gbx</file></map>
	<map><file>Campaigns/CurrentQuarterly/Summer 2021 - 05.Map.Gbx</file></map>
</playlist>
```
