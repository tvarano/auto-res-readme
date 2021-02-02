# How to sign up for the bot
For you to use the bot, I need these items
- UID
- Weekly Preferences (Monday 12:30 richie, Tuesday 3:30 Eppley, etc)
- Token

Send me these items and I can get you put on the list for the bot.

## How to get your login token
1. Download the IMLeagues app and log into your account
2. Download the [Stream Network Debug Tool](https://apps.apple.com/us/app/stream-network-debug-tool/id1312141691) on the app store. It's a little sketch but the other option is $10. 
3. Open Stream
4. Click "HTTPS Sniffing" Under Settings. 
5. Install the CA Certificate
	1. Allow VPN Configurations
	* NOTE: The CA MUST be installed using Safari. You might need to change your default browser.
	* You must also not use a private browsing session.`
	2. Go To Settings > General > Profiles
	3. Click on Stream Generated CA
	4. Click Install
	5. Go to Settings > General > About > Certificate Trust Settings
	6. Turn on the Stream CA

6. Go back to Stream. Click "Sniff Now"
	* You might have to click "I've trusted"

7. Go to IMLeagues app. Log out of your account. Log back in. Open reservations.
	* You might not be able to do a Duo push. Just have it call you. 
8. Go back to Stream. Stop Sniffing.
9. Click on Sniff History and go into your most recent session.
10. Look through the requests for api.imleagues.com/members/verifylogintoken. Click on this request.
	* You can search for this in the top right using the search button.
11. Click on response (next to overview). 
12. Click on preview response body. 
13. There's a bunch of json. I need the refresh_token and the access_token. Copy them both and send them. 
	* KEEP THE KEYS WHEN YOU COPY PASTE
	* If you don't know what to do, just copy paste everything.
14. I recommend uninstalling Stream and its profile and certificate after you're done just to be safe.
	

## Other things to remember
- Do not log out of your imleagues app or login somewhere else (desktop is ok) after you give me your token. 
