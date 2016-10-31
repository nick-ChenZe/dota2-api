# dota2-api
## steam api
### 1. getLeague
	
```json
 /**
 * `获取所有注册联赛`
 * @url:http://api.steampowered.com/IDOTA2Match_570/GetLeagueListing/v1
 * @param {Number} key
 * eg: http://api.steampowered.com/IDOTA2Match_570/GetLeagueListing/v1?key=2B58A9C96FD73EC323CCFDA5383C4BBC
 */
{
	"result":{
	"leagues":[{
		"name":"#DOTA_Item_The_Boston_Major_2016",
		"leagueid":4874,
		"description":"#DOTA_Item_Desc_The_Boston_Major_2016",
		"tournament_url":"http://www.dota2.com",
		"itemdef":17148
	}]
}
```

   
### 2. getMatch

```json
 /**
 * `获取具体比赛`
 * @url:https://api.steampowered.com/IDOTA2Match_570/GetMatchDetails/V001
 * @param {Number} key
 * @param {Number} match_id 	
 * eg: http://api.steampowered.com/IDOTA2Match_570/GetMatchDetails/v1?match_id=12345678&key=2B58A9C96FD73EC323CCFDA5383C4BBC
 */
{
"result":{
"players":[{
	"account_id":46480852,
	"player_slot":0,
	"hero_id":35,
	"item_0":0,
	"item_1":0,
	"item_2":0,
	"item_3":0,
	"item_4":0,
	"item_5":0,
	"kills":0,
	"deaths":0,
	"assists":0,
	"leaver_status":1,
	"last_hits":0,
	"denies":0,
	"gold_per_min":395,
	"xp_per_min":0,
	"level":1	
}],
"radiant_win":false,
"duration":30,
"pre_game_duration":0,
"start_time":1335020334,
"match_id":12345678,
"match_seq_num":12343901,
"tower_status_radiant":2047,
"tower_status_dire":2047,
"barracks_status_radiant":63,
"barracks_status_dire":63,
"cluster":132,
"first_blood_time":0,
"lobby_type":0,
"human_players":8,
"leagueid":0,
"positive_votes":0,
"negative_votes":0,
"game_mode":0,
"flags":0,
"engine":0,
"radiant_score":0,
"dire_score":0
}}
```

### 3. getTeamLogo

```json
 /**
 * `获取队伍logo信息`
 * @url:http://api.steampowered.com/ISteamRemoteStorage/GetUGCFileDetails/v1
 * @param {Number} key
 * @param {Number} appid
 * @param {Number} ugcid 
 * eg: http://api.steampowered.com/ISteamRemoteStorage/GetUGCFileDetails/v1?ugcid=900976537657237645&appid=570&key=2B58A9C96FD73EC323CCFDA5383C4BBC
 */
{
	"data": {
		"filename": "teams/team_logo_1349561171",
		"url": "http://cloud-3.steamusercontent.com/ugc/900976537657237645/9089149320CDED53F352E2BA4D00E8C98E8D4E13/",
		"size": 54577
	}
}
```

### 4. getAllItems

```json
 /**
 * `获取所有物品信息`
 * @url:http://api.steampowered.com/IEconDOTA2_570/GetGameItems/v1
 * @param {Number} key
 * eg: http://api.steampowered.com/IEconDOTA2_570/GetGameItems/v1?key=2B58A9C96FD73EC323CCFDA5383C4BBC
 */
{
	"result":{
	"items":[
		{
		"id":1,
		"name":"item_blink",
		"cost":2250,
		"secret_shop":0,
		"side_shop":1,
		"recipe":0
		}
	]
}
```

### 5. getAllHeros

```json
 /**
 * `获取所有英雄信息`
 * @url:http://api.steampowered.com/IEconDOTA2_570/GetHeroes/v1?
 * @param {Number} key
 * eg: http://api.steampowered.com/IEconDOTA2_570/GetHeroes/v1?key=2B58A9C96FD73EC323CCFDA5383C4BBC
 */
{
	"result":{
	"heroes":[
		{
		"name":"npc_dota_hero_antimage",
		"id":1
		}
	]
}
```

