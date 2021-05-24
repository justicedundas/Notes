# OpSec -> Security, Privacy, Anonymity
Notes on go-incognito	-> https://github.com/techlore/go-incognito (youtube account has videos)

Extra Resources (temp):
* *IF* you have time and legit care, please follow -> https://anonymousplanet.org/guide.html#introduction 
* No, seriously ... work on the above guide, it's top notch
* seriously make your life easier and go here for tools ... https://www.privacytools.io/


Contents:
	1. Permissions and Settings
	2. Passwords
	3. Two-Factor Authentication
	4. Search Engines
	5. Browser
	6. Hardening Browser
	7. Browsing Habits
	8. Proxies and VPNs
	9. Antivirus and Malware
	10. File Deletion
	11. Storage and Encryption
		- HDD
		- SSD
	12. Safe Communication
		- Mobile
		- Email



Why OpSec?
* lol... do i really need to explain you don't wnat all your crap stolen
* privacy and anonymity should not be overlooked... 5 eyes especially, literally wiretapping the whole world haha 
	- "but I don't do anything wrong who cares?" -> https://www.youtube.com/watch?v=M5N51k0o_8A




## 1. Privacy and Settings;
* Windows 
	* Win10Privacy
	* Grant minimum permissions to all apps

## Password;
Password -> Hash on signup, if hash is like john the ripper, etc 
Other major issues from weak or stole passwords

Avoid by using;
* Long passwords based on entropy in information theory ... use dice trik for random dictionary terms  
* Use a password manager - don't use cloud based if possible ... if you use then use difficult major password 
	* USE FOSS -> Keypass or bitwarden, best is masterpss if possible it's more secure 
	* Other way, compartmentalize passwords based off function (school, work, etc.) and store in different password managers
	* Change passwords regularly 

* BIOMETRICS ARE NOT MORE SECURE -> FACE AND FINGERPRINT ARE HACKABLE
	* CANDA ENFORCES PASSWORD TO BE HANDED OVER BY LAW************

## 2. Security Questions;

* Don't be honest... enter fake info, use passwrd manager to store answers


## Two-Factor Authentication;
* SMS - text verification;
	* SMS 2-step is not secure... cell-phone providers have weak social engineering protections
		* Still better then nothing

* Private keys -> app generated 
	* Generate keys every 30 seconds for identifcation after qr code scan
		* FOSS option that is popular -> Authy, but updates on cloud and don't allow for cloud 
	* ex; Duo or Symantec VIP Acces need internet... beware MITM Attacks	
	* Best options; 
		* FreeOTP for iOS
		* AndOTP for Android

* Best is physicl 2FA;
	* Use USB or other memory deice to access, use it for operating systems or full disk encryption
	* YubiKey
	* Use TPM module so OS can only be booted on certain systems

## 3. Search Engines;

* Google, Yahoo, Bing, etc. build profiles of you for advertising based on very one of your searches

* Best to Use;
	* DuckDuckGo, 
		* onion variant, and tags to seearch other sites
		* Not best bet to use based on USA location and prop software

	* Startpage;
		* basically google proxy, provides their results
		* doesn't have tor option so need to access clearnet
	
	* searx.me
		* best priacy wise, provides tons of search engne results

## 4. Your Browser

* Google Chrome;
	* very secure, fastest
	* terrible for privacy, tracks everything you do and build profile in browser
	* got caught searching computer files for info on you

* Firefox;
	* best option for privacy and security IF HARDENED
	* search for guides and tools to "harden" browser 

* Brave;
	* best if you don't want to configure firefox properly 

* Tor;
	* learn about this... legit

## 5. Hardening your browser
** use firefox..... just for security based apps, these tips remove anonymity

* Settings;
	* first steps -> automatic updates, homepage to privacy-oriented search engine (duckduckgo, etc.)
	* Things to disable;
		* all suggestions
		* password management
		* never remember history 
		* clear history and cache on exit
		* block pop-ups
		* send do-not-track signal 	
		* disable all tracking and telemtry data 

* about:config 
	* USE THIS AN FOLLOW ALL STEPS;
		- https://www.privacytools.io/browsers/

* extensions;
	* https everywhere -> enforce https
	* uBlock Origin -> add/tracker blocker
	* privacy badger -> block web rtc leaks, trackin crap
	* decentralytes -> block third party trackers
	* cookie autodelete -> automatically delete cookies and browser data 
	* CanvasBlocker -> HTML5 uses canvas fingerprinting.... google it then block it
	* NoScript -> disable javascript... this will cause issues and break website ... just llow or whitelist  site to allow
	* uMatrix -> Complex, difficult to configure but use if you want
	* User-Agent Switcher -> spoof user-agent... not for hardening but good for anonymity, see below 
		- go to "extensions" in firefox


## 6. Browsing Tips;

* Avoid program dwnload sites ... only install from software SOURCE WEBSITE
* IF BROWSER SAYS SITE IS INSECURE FLIPPING LISTEN
* Avoid pirating unless you can safely navigate....
* Phishing attacks;
	* Avoid phishing attacks by looking at URL in search bar... check certifacte on wbesite
	* Check email for match to real one
		* if email is suspicious then authnticate with sender to make sure they sent it
* NEVER GIVE ACCESS TO CAMERA, MIC, ETC. ... 
	* if you must... disable after use

* Other tracking methods;
	- behavioral track;
		- keystrokes are tracked across websites for cadence	 
			- use KeyboardPrivacy on chrome
			- behavioral-Keyboard-Privacy on firefox -> not that great but decent firefox option

* PUPs (potentially unwanted programs);
	* Read all checks when installing software, dont install unneeded programs

## 7. Browser Uniqueness, aka fingerprinting

*  testing browser uniqueness;
	* Panopticlick
		- https://canvastrackersimulator.org/
	* AmIUnique
		- https://www.amiunique.org/
	* BrowserSpy.dk
		- http://browserspy.dk/
	
	- these will show you are easily trackable... less unique means easier to target for hackers tho...

* Mitigation;
	* Noscript -> see above
	* UserAgent spoofer;
		- User-Agent Switcher extension on firefox, see above
	* USE PSEUDONYMS FOR FLIPS SAKE
		* password manager makes this easier... use random email addresses for different walks of life (school, social, work, etc.)

## 8. VPNs & Proxies

### Proxies;
	* Implemented on;
		- online services -> ex; Smart VPN: Proxy (windows)
		- configured directly in settings or operating system 
	* Goals;
		- hide IP address
		- Spoof by acting as middle-man, websites think you are visiting from different "address" (ip)
	* Downsides;
		- don't encrypt traffic
		- don't strip identifiable crap
		- no extra security features built in
			****** shadow-proxies do (shadowsocks)

### VPNs;
	* Implementation;
		- dont use free, unless solid free-tier (protonvpn, Windscribe) -> okay, but not great 
		- key things to look for;
			- encryption:
				- AES-256 bit encryption, 
				- 2048 bit handshake encryption, utiliing OpenVPN or Wiregurd
			- Jurisdiction;
				- AVOID THE 14 EYES ... legit look it up below, it's nuts
					- https://www.privacytools.io/providers/#ukusa
					- https://en.wikipedia.org/wiki/UKUSA_Agreement
					- WATCH THIS, LEGIT -> https://www.youtube.com/watch?v=M5N51k0o_8A&feature=youtu.be
				- AirVPN, PIA (private internet access) are solid and located in 14 eyes
					- probably compromised tho... let's be real

			- PFS (perfect forward secrecy)
				- need to continuall cycle keys
			- History;
				- check if they've ever given out user history .. (yes, this is store *sigh* I know)
			- Policies 
				- check stance on how they work with law enforcement (this is to note if they keep logs)
			- System KS;
				- system killswitch -> setting that if vpn disconnects, all internet traffic stops 
		*** list to look through -> https://www.privacytools.io/providers/vpn/

	* Goals;
		- Re-routes traffic through encrypted tunnel
		- Hide IP address with encrypted traffic...
		       - ISP, Govs, etc. can't snoop, collect, sell browsing data.... THEY DO THIS - lobbied congress for it in 2016  
		- MITM attacks are mitigated via encryption
	* Downsides;
		- Processing power;
		- Cost more then proxies
		- Captcha requests;
			- annoying as hell... 
		- Speed -> slower then norm

Payment Privacy;
* Mullvad
* NordVPN using crypto
* IVPN

****** Self-Hosting VPN -> BESTTTTTTT, use WireGuard potentially but be careful... OpenVPN still the best 	


### 9. Antiviruses & Malware 

** heavily debated, generally make software more secure but some open you up to new exploits and vulnerability 

* WORST thing to do for privacy... scans and collect LITERALLY EVERYTHING on your computer lol
* if you don't download random crap, and browse safely then don't use
* Recommend using Windows Defender if using windwos, if using mac then move along BUT stay safe 
	* Windows already collects everything anyway LOL so neg privacy crap doesn't apply
	* Please look up guides to properly set up

Operating Systems Differences;
	* Windows;
		- windows already collects ALL of your data LOL, so jst use windows defender
		- *Properly* configure it using a guide online 

	* MacOS;
		- beginners use pcbind
		- if basic guidelines used above, then don't really need it

	* Linux;
		- lol don't need jack 
		- run random ClamAV scans just incase tho

	* iOS;
		- if not rooted, then don't need jack

	* Android;
		- beginners get one if you download rndom crap

Best Practices to protect without antivirus;
	1. Follow browsing practices 
	2. Use a Firewall
		a) windows has one
		b) macOs needs to be enabled
		c) linux, check out NetGuard no-root firewall, pretty solid functionality 

	3. Prevent Keyloggers
		- virtual keyboard can help
		- GuardedID or other services for keystroke encryption
	4. Self Awareness
		- if you're an idiot and access insecure crap without proper tools, then just use it 

## 10. File Deletion

Emptying recycle bin doesn't delete your crap... it only deletes the pointer and makes slot availabler, until overwritten it's still recoverable... install Recuva to check this out

Tools to use:

Hard-Disks: 
	* Windows;
		- CCleaner -> wipes unused data, makes comp faster
			- https://www.ccleaner.com/ 
		- Blechbit also offers this
	* Mac;
		- just run this script;
			- https://www.macworld.com/article/3005796/how-to-replace-secure-empty-trash-in-os-x-el-capitan.html
	* Linux;
		- Bleachbit is best bet

Solid-State drives;
	* wiping data is more difficult... wipe from bios, but beware this uses limited "writes" to disk
	* Just use an encrypted drive...
		- see next on encryption

## 11. Storage and Encryption 
(not disk... covered later)

Good Tools;
	1. 7zip 
		* FOSS archiving tools, not technically encryption, but allows to password protect files
			- https://www.7-zip.org/
	2. VeraCrypt
		* FOSS, encrypted, free, and even offers full disk encryption **see later guide** 
		* creates encrypted "volume" to load files into,  
			- https://www.veracrypt.fr/code/VeraCrypt/	
	3. GnuPG
		* FOSS, implements PGP keys (pretty-good privacy), uses 3rd party software for GUI 
			- https://gnupg.org/



Cloud Storage;
	* top 4:
		1. iCloud
			* encrypt with 128 bit 
		2. Google Drive
			* encrypt with 128 bit 
		3. Dropbox
			* encrypts data with AES-256 bit, but hold keys so can decrypt anytime 
		4. Microsoft OneDrive
			* doesn't encrypt storage... what a joke

		* all encrypt traffic while it being uploaded, great so MITM can't see crap 

		* IF YOU MUST USE you should encrypt files before uploading... they can see it all, and share
			- cryptomator is a great tool;
				- https://cryptomator.org/

	* Other provides:
		1. MEGA:
			- https://mega.io/
		2. ProtonDrive:
			- https://protonmail.com/blog/proton-drive-early-access/

		* both seem solid, good alternatives for beginners

	* BEST OPTIONS:
		1. Nextcloud:
			* FOSS, Self-Hosted 
			* tricky setup, but worth the effort
				- https://nextcloud.com/

## 12. Safe Communication:
	
Most methods rely on you using a specific service, and the other user as well... worth convincing ppl tho 


*Background*:
- SMS messages -> tech used for standard messaging... all of it is logged by governments lol... and tons of tools to steel that crap

What to look for:
	* Messengers:
		* Off-the-Record Messaging:
			- crypto protocol, combines 128-AES, Diffie-Hellman key exchange, and SHA-1 hash function 
			- also provides:
				* forward secrecy
				* malleable encryption
		* XMPP:
			- Extensible Messaging and Presence Protocol open comms protocol is good alternative
		* Stick to FOSS
		* Look for crap you need to sign up that can identify you
	


Modern communication methods:
	- SMS
	- Common commercial crap;
		* iMessage, etc.
		* ALL i repeat ALL are crap.. everything is logged
	- Other commercial crap;
		* Whatsapp:
			- collects metadata ... like common, its facebook
		* Telegram:
			- security issues...
	- Email:
		* Protonmail	
			- encryption works for non-protonmail emails too BIG bonus
		* Disroute
		* Tips: 
			- use anonymous remailer, basically proxy for email
				- PTIO Email
			- Encryption:
				* PGP
				* GPG
				* OpenPGP	
				- NEEDED, email providers literally read all of your crap... use it
				- tough to setup, so use Mailvelope if you don't want to
		* I2P-Bote:
			- really cool decentralized encrypted SERVERLESS email service
			- https://github.com/i2p/i2p.i2p-bote
	- File Sharing:
		- Nextcloud, firefox send
		- use for larger files
		- ENCRYPT BEFORE SENDING


Recommendations:
	* Messaging/Video/Voice:
		- Signal:
			- need to use phone, but get around using burner apps listed below or experienced self-host emulators 

	* Secondary Number: 
		- Burner:
			- https://www.burnerapp.com/
		- Shuffle
			- getshuffle.com
		- MySudo:
			- https://mysudo.com/

	* Email:
		- Protonmail for beginners:
			- https://protonmail.com/
		- Self-hostig:
			- best option if you know how, 

	* Disposable Email:
		- TempMail:	
			- USE FOR BS SIGNUP OF SERVICES AT THE LEAST
			- https://temp-mail.org/
			
		** beware metadata in headers.... both email, and disposable will have OG IP in it, clear it
	
	* File-Sharing:
		- OnionShare:
			- encrypt before uploading, give password to recipient to decrypt
			-  

