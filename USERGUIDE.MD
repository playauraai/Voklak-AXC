VOKLAK
So, what makes AXC different?
The main idea is prevention first. We block the ways cheaters get in, rather than waiting for them to cause problems and then reacting. It runs in layers to make sure everything stays locked down without killing performance.
How it works under the hood
User-mode part
This runs alongside your game. It's super lightweight – just checks that everything is running as it should, validates what's happening, and talks securely to the deeper layer. You probably won't even notice it's there.
Kernel-mode driver
This is the heavy hitter. It sits at the system level and enforces the rules: watches for suspicious memory access, blocks unauthorized changes, and only allows legit requests from the user-mode part. It's properly signed with a real code-signing certificate so Windows trusts it and doesn't throw false alarms.
Secure channel between the two
Everything that passes between user-mode and kernel-mode gets checked and validated. No backdoors, no risky shortcuts – just tight, controlled communication.
Trust and signing
Every kernel component is digitally signed through proper channels (tied to our nummutex.com infrastructure). That means no tampering, smooth installation, and better compatibility with antivirus software.
How it fits with Nummutex
If you publish your game or app on Nummutex, you get AXC protection automatically – no extra work needed. You also get free built-in voice chat, automatic updates, centralized distribution, and a bunch of other platform perks.
As a developer, the process is dead simple:
Sign up as a dev on Nummutex
Upload your game/app
AXC is already enabled by default
Hit publish
Your users download it with full protection baked in, plus voice chat if you want to use it. You don't have to build or maintain your own anti-cheat – we handle that centrally.
The built-in voice chat bonus
It's completely free for anything published on the platform, runs on our infrastructure, stays secure, and plays nice with AXC-protected sessions. Saves you from messing with third-party services.
Our approach to security
We keep things minimal and focused:
Prevent problems upfront
Expose as little as possible
Clear separation between components
No unnecessary data collection or spying
AXC only activates when one of our platform's protected apps is running. It doesn't hang around in the background, doesn't touch unrelated stuff, and definitely doesn't abuse kernel access.
Quick disclaimer
This is strictly for protecting games and software distributed through Nummutex. Nothing shady – just fair play and solid security.

IN SHORT
With Voklak AXC you get reliable user-mode + kernel-mode protection, properly signed components, a smarter exploit-focused design, free voice chat, and way less headache for developers.
Publish once, stay protected by default. Simple as that.


Bans aren't decided by the anticheat itself – that's all server-side. AXC's job is smarter: it sniffs out anomalies in real-time. Think weird memory tweaks, funky process behavior, impossible movements, or any exploit-like red flags that scream "something's off."
How detection + banning flows
AXC spots the anomaly
User-mode checks flag odd runtime stuff, kernel driver enforces and confirms. No signatures – it's all about behavioral patterns and integrity breaks.
Secure report to the server
It bundles up the evidence (timestamps, hashes, context) and sends it over our locked-down channel to Nummutex servers. Nothing personal, just the facts needed to verify.
Server makes the call
Our backend crunches it: Is this a clear cheat? Repeated offender? Weighs against player history, game rules, etc. If it's ban-worthy, boom – server-side enforcement kicks in (kick, temp ban, permaban). False positives? We tune on the fly to keep 'em rare.
This setup keeps things fair and lightweight:
No client-side bans = Cheaters can't tamper with decisions locally.
Server oversight = Humans/AI review edge cases for accuracy.
Low latency = Detection happens instantly, reports fly fast.
