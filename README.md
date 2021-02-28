# cicuta_virosa
iOS\iPadOS 14.3 kernel LPE for all devices by **@ModernPwner**. Please do not follow us on twitter :)

# Current state
- Exploit works :)
- Need a lot of cleanup + more stable primitives that not relaying on memory reallocation. **Use it on your own risk**
- Exploit will take more then 2 minutes because we can't understand how to properly bypass one stupid sanity check in kernel on "Stage 3: Convert uaf into pktopts uaf" (we'll fix it soon)
- Reliability is amazing on our A13 and A10 devices

# The vuln
**CVE-2021-1782**: A race condition in user_data_get_value() leading to ivac entry uaf. This issue has been actively exploited in the wild with the WebKit exploit. We might release this RCE chain in the future.

# Writeup
Soon.

# How to build it
be pro epic hax0r like cockstar or pussy420wnd

# Credits
- Some utils (exploit_utilities.c): @Jakeashacks
- Vuln: samsuck

# License
my patches and additions on top of ModernPwner’s code are licensed under the ABSE (“Anyone But Stefan Esser”) license.
note that an additional exception to the license is added, forbidding use/redistribution of said content to his
trainees as well, but only when in a 5 mile radius from “Stefan Esser” or while holding any sort of (video)conference/chat with him.
note that this license will only be used as long as what would capstone decode / that one other arm64 ida
plugin thing by i0n1c (“Stefan Esser”) are not under the MIT license.
afterwards, all exceptions are cleared and basically WTFPL applies

# PAC bypass
For the moment we have a brand new technique to bypass PAC but we decided to not include such critical stuff here.  
**Maybe** we'll post a PAC bypass along with the iOS 14.5 exploit. This is in progress, we **may** publish 14.5 exploit after Apple patch. 
