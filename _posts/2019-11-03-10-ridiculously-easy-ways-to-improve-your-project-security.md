---
layout: post
title: 10 Ridiculously Easy Ways to Improve Your Project Security
date:
  'Sun Nov 03 2019 01:00:00 GMT+0100 (heure normale d’Europe centrale)': null
categories: Tips Security Help
published: true
comments: true
---

*Four months ago we asked more than 120 of our customer to fill in a form so we could know a little bit more about them. Today is the day we will review what they answered by giving 10 ridiculously easy ways to improve your project security !*

* * * * *




1 -- Use a login system
----------------------

A vast majority of our customers already implemented a login system. You should always have a login system to protect your application from hackers. How can it protect your program, you may ask ? A login system will give you natural control on whoever access your program. Not all login system are equals however, and some will give you way more control than others ⚠️

A good login system needs to inform you about :\
-- Who runs your software, and when ✅
-- With which login key they actually signed in ✅
-- The HWID of the customer ✅
-- The IP Adress of the customer ✅

All of those informations will allow counter-measurements and actions to be done to reduce the potentiality of a cracker to access your sensitive informations.

* * * * *




2 -- Only use a server-sided login system
----------------------------------------

There exist MANY different approaches on how to make a suitable login system for your project. Let's see some most-used ones and their flaws, and why you should stick with a server-sided login system. PHP-based login system is used as an example here, but any login system that validate the authenticity of the user on server-side is fine too 😉

#### [2.1] -- Do not use MySqlConnection

The main issue with MySqlConnection is that it requires you to hardcode the credentials of the database in your project source code. ⚠️ The data will be visible using decompilers or even hex editor / text editor on your compiled file, putting your security at high risk.

#### [2.2] -- Do not use Pastebin HWID check

This technique consists of downloading a string on a raw pastebin url and checking if current user's HWID is contained inside the pastebin content. While the pastebin content cannot be tampered, (⚠️) the connection can still be redirected or the link can be tampered to include a pastebin where the current user's HWID is in. This is not a good solution since anyone can alter the checked data.

#### [2.3] -- Do not use any login system that only relies on the file

That is the case of offline key system, offline HWID system and basically all offline login system. The main issue is that the login system is offline, so it can only be entirely on the customer's computer, in other words all of your important code used to check if the key is correct is on the customer's computer, and thanks to that he is able to alter the file and therefore bypass the login system implementation.

* * * * *




3 -- Download files using the login system
-----------------------------------------

You should always make it so customers need to use the login system to access any 3rd part files or link. To do so, most of the login system will allow you to create "*server variables*", "*remote variables*", "*variables*" or any other features that allow you to post data online and retrieve the data using the data ID within your project. 🤯 This way it will prevent anyone that is not an actual customer of your program to access those files. You need to send back the file only if the login credentials of your customers are valid, that is, not only correct but also only if he has an actual valid login key.  

* * * * *




4 -- Use your login system to collect informations about your customer
---------------------------------------------------------------------

🎉 Chill out, we are not telling you to become the next big-brother, and you need to comply with GDPR or any local laws regarding the collect of cyber data anyway; but it is necessary to know who your customers are to be able to offer a better service or product, and mostly to prevent crackers and hackers to use your software again.\
In a concrete example, let's say *Mister Smith* registered on my product with his own account, played with the program a few times and then charge-back on PayPal and crack the file. Now, what we want him is to calculate the cost-benefit of such action, because as soon as he charged back on PayPal you will ban his IP and HWID from the login system database. ⚔️ This way, when you will release new updates for your files, they won't be able to get them. This way you can prevent future cracked version of your program to exists.

Your login system must allow you to access all of the data* we listed bellow to monitor your program access with ease :\
- Username\
- Password\
- E-mail\
- IP Address\
- Hardware ID

* of course all sensitive data must be encrypted with secure solutions 😉

* * * * *




5 -- Always use the most of NETGuard.IO
--------------------------------------

The premium plan includes a lot more protection settings for your file, and will cover major security risks about your data being stolen statically. ⚔️ The premium plan protect your strings, the function calls inside your program, and even include a native wrapper for your .NET Framework file.   

* * * * *




6 -- Always use 'Native Shield'
------------------------------

The "*Native Shield*" protection adds a lot more security to your overall file obfuscation settings. This settings is a must-have for premium users of NETGuard.IO ! This option also allow you to use any native packer or file virtualizer on top of your protected file.   

* * * * *




7 -- Always use a Native Packer or File Virtualizer on top of your .NET Obfuscation
----------------------------------------------------------------------------------

.NET programs are MSIL-based compiled files, that means anyone can look at the MSIL code level. While if you use a Native Packer or File Virtualizer the MSIL code is hidden within the native file, and the vast majority of script skiddies will stop at this step. Adding a native packer / virtualize on top of the protected file produced by NETGuard will increase your file security a lot.

* * * * *




8 -- Re-obfuscate your project as obfuscators update are being released
----------------------------------------------------------------------

🚀 You should always re protect your file every time a NETGuard update is being release because it will allow you to increase your file security and fix some bugs it might have. Once re protected, you should delete every link of the old file from the internet / your website to prevent hackers to de-obfuscate / unpack your old files and get their hand on the source code.

* * * * *




9 -- Use online payment store system to let your customers download your product
-------------------------------------------------------------------------------

You should consider using a selling gateway system such as Shopify or Selly, they are free to use and will make your life easier. 💳 They will prevent anyone but your customers from accessing your software download link.

* * * * *




10 -- Control your online presence
---------------------------------

💻 If you are being active on online forums or communities, you have to be aware that your behaviour will influence the public's point of view on your product. Being seen as nice and professional will prevent people from willing to harm you and your project. The less drama, the better.

In all scenario :\
-- you should try to be as professional as possible, that means being gentle with nice people, and prevent yourself from being involved into any sort of drama.\
-- you should keep your online community safe from any trolls or mean people, that will lower the quality of your external image.

* * * * *
