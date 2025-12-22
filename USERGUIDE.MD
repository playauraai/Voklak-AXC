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
