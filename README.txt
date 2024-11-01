=== Simple Login Limit & Protect ===
Contributors: skymonitor, ferulisses
Donate link: https://skymonitor.com/products/simple-login-limit-protect-for-wordpress/
Tags: brute force, authentication, login, limit, protection, protect, security, secure, GDPR, block, botnet, lockdown, hacker, cracker, attacker
Requires at least: 5.0
Tested up to: 5.5
Stable tag: 1.0.0
Requires PHP: 7.0
License: MPL2
License URI: https://mozilla.org/MPL/2.0/

Simple Login Limit & Protect is designed to protect your WordPress from hackers, with easy configuration, automatically learns from user behaviour.

== Description ==

Simple Login Limit & Protect is a Plugin designed to protect your WordPress site from hackers, crackers and other attackers, with simple configuration and with minimum problems for legitimate users.

Using the same technology used in the most advanced Security Tools, our plugin works as soon as activated, detecting malicious behavior and automatically blocking attackers.

= Key Features =

* Behavioral Intelligent Learning, detect the behavior of users to distinguish the bad guys from good guys
* Really GDPR Compliant [(why some others plugins don’t comply)](https://skymonitor.com/why-hash-dont-anonimize-an-ip-address-and-what-this-affects-gdpr/)
* Minimum Configuration, just install and don’t mind looking for the settings, works out of the box

= Behavioral Intelligent Learning =

We expect legitimate users to behavior in a certain way. In the other side, hackers usually start with simple commoditized scripts, we studied these scripts and implemented detection rules for them.

We studied attackers techniques such as User Enumeration, Brute Force Attack, the Most Common Passwords Used and developed sensors to these behaviours, identifying the remote user as an attacker.

In the other side, legitimate users normally use the same Provider, with a common Internet browser and in an certain way, we also detect this behaviour and identify them as a good user.

= Automatically allow legitimate users to try again =

If a legitimate user is blocked due to missing his password, the plugin will inform the user how much time he have to wait before he can try again, minimising support.

On the first missed password tries, the plugin will allow the user to try again in a few minutes with a message, this removes work from the Site Administrator.

If necessary, the user can use the WordPress “Lost your password” feature to generate a new one if he forgot to not be blocked again.

But if it's a hacker that continues to try invalid passwords he will be blocked again for even increased times (limited to 24 hours).

= Full list of Features =

* Detect and block malicious users
* Detect and block Brute Force Attacks
* Detect User Enumeration Attacks
* Inform legitimate users if they are blocked
* Detect if a hacker is not using HTTPS
* Detect if a hacker is using scripts
* Detect the most commons attack tools to WordPress sites, such as Hydra, Curl, MetaSploit, Kalil
* Detect if the attacker is using a password dictionary to guess passwords
* Block the IP of the attacker
* Allow a legitimate user to try again after a few minutes
* If the attacker continues, block again for 30 minutes
* If the attacker continues, block for 24 hours
* Counts and inform the Administrator how much attacks has been blocked
* Detect and works automatically with Sucuri Web Firewall
* Detect and suggest configuration for Proxies and Load Balancers
* Detect and block attacks to XMLRPC API (not all plugins do this)
* Detect attacks to REST API for user enumeration (no other plugin do this)


== Installation Instructions ==

= On WordPress Admin Dashboard =
1. Visit `Plugins > Add New`
2. Search for `Simple Login Limit & Protect`. Find and install the plugin
3. In `Plugins > Installed Plugins`, click in Activate

= Downloading From WordPress.org =
1. Download Simple Login Limit & Protect zip file.
2. Visit `Plugins > Add New` in your WordPress Admin Dashboard
3. Click in `Upload Plugin`
4. Click in `Choose File`, find the downloaded file in your computer
5. Click in `Install Now`
6. In `Plugins > Installed Plugins`, click in Activate.

= Manually via FTP, SFTP =
1. Download Simple Login Limit & Protect zip file.
2. Unzip and upload the `simple-login-limit-protect` directory to your `/wp-content/plugins/` directory
3. Enter in your WordPress Admin Dashboard
4. In `Plugins > Installed Plugins`, click in Activate.


== Screenshots ==

1. Simple Login Limit & Protect configuration screen
2. What a user sees when it's blocked
3. The login screen released again

== Demo Video ==

https://youtu.be/J9DolDG7vU0

== Frequently Asked Questions ==

= My IP has been blocked, what should I do? =

Just wait the time indicated in WordPress login screen, the system will release your IP again automatically.

= I'm blocked and I can't wait to my IP to be released, what can I do? =

You can access from another connection from another provider, for example, using a 3G/4G Network instead of your Wifi.

If you forgot the password and has blocked by this, change the password before trying to access again.

If you can login in MySQL, you can clean the data on table wp_simple_login_limit_protect, this will give you a fresh start.

If you can only access by FTP, you can access the wp-content/plugins folder and delete the folder simple-login-limit-protect, this will uninstall the plugin, you can install the plugin again, while logged, you will not be blocked.

If you can't access by MySQL neither FTP, sorry, there is no backdoor.

= Why can't I disable GDPR protection? =

We understand that this provides a better protection, since we use Data Blurring to anonymize IP Address, like Google Analytics and other tools.

When Blurring the IP Address we will have a range of IP Address instead of the final IP, for example, if the hacker IP Address was 198.51.100.10, we will block from 198.51.100.0 to 198.51.100.255. With this, without other data sources you can't identify the original IP Address.

If a hacker tries do disconnect and reconnect to his provider, there is a chance to him to receive an IP Address in the same range, that will be already blocked.

Even if him receive an IP Address of another range, in a few tries his Internet Provider will be full blocked.

This don't prevents him to access content in your site, just to login in administrative area.

We think that this is a good idea, since we prevent more attacks from the same hacker, and, there's only a few chance that your neighbor will be trying to hack in your site.

If you think otherwise, please [fill this form](https://forms.gle/1fbSCQoyqYLrWJxd8) with your ideas.

Other reason is that some hackers will be in Europe Union, thus it's better to comply to not be at legal risk.

= How do you comply with GDPR? =

GDPR says that we can't store personal information, with include IP Address, without consent from the user.

Sure, a hacker will not consent to store his information, but we need this information stored to block attackers.

So, a method to do this is using Pseudo Anonymization with Data Blurring.

This is the [same technique used by Google Analytics](https://support.google.com/analytics/answer/2763052?hl=en), so, we think we are backed.


= Why some others plugins don't comply with GDPR? =

They use a technique called hashing to obfuscate the IP Address, normally applying a MD5 Hash Algorithm.

While this works well for unpredictable data such passwords, IP Address are high predictable (there is only 4 billions of them), and thus can be easily reversed.

We explored this theme in a Post in our website, but don't take our word, we referenced others security specialists about it:

[Why Hash Don't Anonimize an IP Address and what this affects GDPR](https://skymonitor.com/why-hash-dont-anonimize-an-ip-address-and-what-this-affects-gdpr/)

= There is only one Security Mode that is Intelligent, why can't I change it? =

We are planning other modes, we though that was a good idea keep this space reserved for options that are coming soon.

= I have an idea =

Please, [fill this form](https://forms.gle/1fbSCQoyqYLrWJxd8), we will be happy to help:


= I need support =

Mail us at <a href="mailto:support@skymonitor.com?subject=Simple Login Protect Support">support@skymonitor.com</a>

== Changelog ==

= 1.0.0 =
* Initial Public Release

