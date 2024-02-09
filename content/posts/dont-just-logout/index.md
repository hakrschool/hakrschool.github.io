---
title: "Don’t just logout from your online account"
date: February 8 2024
draft: false
description: "A post to help prevent password leak"
summary: "A post to help prevent password leak"
slug: "dont-just-logout"
---
{{< figure src="searchsecret.png" >}}

> ### KEY TAKEAWAYS:
> - Just logging out from your online account is not sufficient to prevent your password leak.

Do you use public computers to access any of your online accounts? (Email, social media, Banking etc.)

 - May be at Airport? Your mobile data is not available, and you need to do something online. Sending an important message to family. <br>
 - How about Hotels where you stay? Maybe you wanted to take some printouts from your email OR access some online account.
 - Then at your friend’s place? Using their laptop to access your banking or other online accounts.
 
This article is NOT about, do not use public Wi-Fi, use VPN etc., NO. <br>

This is much more basic than that.

I am pretty sure after you are done with your online account work, you will log out from the application. <br>
What if I say, even after you log out, your account password could still be leaked? <br>
Unfortunately, that is possible. 

A small additional step (often overlooked) could prevent your password from getting leaked. 

And that step simply is, **closing the Browser (recommended)** OR just that **browser tab**.

Yes, closing the browser after you log out from an application will remove all the information from the browser’s memory as well.

Do you want to see how the password could be leaked/extracted, if you just log out, but not close the browser? <br> 
Continue reading… :right_arrow:

### Deep Dive:
Creating the browser memory dump is straight forward.

Once we have the browser memory dump, then it’s simply a :mag_right: search game looking for sensitive information in the dump including passwords. <br>

There are tools (Ex: *WinDBG*) using which you could load the memory dump file and start searching.

Let’s look at some **real application** examples: 

*Here is my browser dump file loaded in WinDBG **after** I logged out from a dummy `Facebook account`.*
{{< figure src="facebook.png" caption=" Don't get excited! Its a dummy password." >}}

*Here is my browser dump file loaded in WinDBG **after** I logged out from a dummy `Gmail account`.*

{{< figure src="gmail.png" caption=" Don't get excited! Its a dummy password." >}}


This was tested on Firefox browser, but the behavior would be same in other browsers too.

As you can see, the passwords are visible in clear text. Not just passwords, depending on the online account you access, additional sensitive information could be leaked as well. For example, your email contents, bank account details etc.

So DO NOT forget to close the browser (or the tab) next time.

Before I end this article, few quick key points: 
-	These are not vulnerabilities in the browser OR the applications you accessed.
-	The communication between the browser and the application is generally over TLS, encrypted channel, meaning passwords and sensitive data are not visible during the transit.




