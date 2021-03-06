=== Socialauth-WordPress ===
Contributors: labs@3pillarglobal.com
Donate link: http://www.3pillarglobal.com
Tags: socialauth wordpress, social login integration, hybridauth, authentication, contacts, friendlist, providers, openid, providers
Requires at least: 3.0.0
Tested up to: 3.4.2
Stable tag: 3.11.13
License: MIT License
License URI: http://www.opensource.org/licenses/MIT

SocialAuth-WordPress a WordPress 3.0+ plugin which enables social login integration through different providers (eg. Facebook, Twitter).

== Description ==

SocialAuth-WordPress a WordPress 3.0+ plugin derived from popular PHP based HybridAuth library. Inspired from other WordPress social login plugins, this plugin seamlessly integrates into any WordPress 3.0+ application and enables social login integration through different service providers. All you have to do is to configure the plugin from settings page before you can start using it. SocialAuth-WordPress hides all the intricacies of generating signatures and token, doing security handshakes and provides an out of the box a simple solution to interact with providers.

[Click Here](http://labs.3pillarglobal.com/socialauth-wp-demo/wp-login.php) to see Socialauth-WordPress in action.

Please check out [Developer Notes](http://wordpress.org/extend/plugins/socialauth-wp/other_notes/) for more information on this plugin.

You can also check [labs.3pillarglobal.com](http://labs.3pillarglobal.com/) to get similar libraries in other technologies under SocialAuth umbrella.

What's new in latest release?

*  Introduced plugin short code [SocialAuth-WP-Short-Code]. Use in pages/posts.
*  If new registrations are disabled, new users can not login to your WordPress site.
*  New option in plugin settings to hide 'My Contacts' option from left navigation bar of dashboard.
*  Post login redirect capability to get user back to the page from where you initiated login process.

== Installation ==

* Login to your WordPress site as admin, go to plugins menu and search for "SocialAuth-WordPress".
* Add the plugin to you plugins directory.
* From the plugin administration, enable the plugin.
* Go to Settings > SocialAuth-WordPress from left side menu.
* Configure plugin settings such as enabling one or more providers and providing your application keys.
* Go to login page and see the magic.

== Frequently Asked Questions ==

= Where can I find more information? =

Please check out [Developer Notes](http://wordpress.org/extend/plugins/socialauth-wp/other_notes/) for more information on this plugin or feel free to email us.

= Where will I get the application keys? =

Application keys need to be generated for each provider you want to enable. For example, to enable your WordPress users to login with their Facebook account, register your blog as a Facebook application. You will be provided with application keys, which you can use in the settings page for SocialAuth-WordPress.

= Which providers are supported by the plugin? =

The plugin supports all providers supported by HybridAuth library. All major providers such as Facebook, Google, Twitter, LinkedIn, Yahoo are supported. Please check out the [HybridAuth page](http://hybridauth.sourceforge.net/userguide.html) for the complete list. 

= I downloaded and enabled the plugin, but no providers appear on login page. What's wrong? =

Once you have downloaded and enabled the plugin, you need to go to the settings page and enable one or providers.

== Screenshots ==

1. Login screen with enabled providers
2. Twitter authentication screen
3. Twitter redirecting back to your application
4. Profile of the authenticated user showing user data from Twitter

== Changelog ==

= 3.11.13 =
* Introduced short code [SocialAuth-WP-Short-Code] to get social-auth-wp working from pages and posts along with login page.
* Added compliance for registrations settings; if registration is disabled new users can not login to your WordPress site.
* Added a new option to settings to hide 'My Contacts' option if you do not need that.
* Introduced post login redirect capability to get back to page from where you initiated login process.
* Started to use user's first name when username not available from login provider, this will fallback to user profile identifier if first-name and username both are not available.
* Added link for 'Back to Login' (close pop up window) when authentication fails and user is prompted with error message.
* Other minor improvements for consistency and user friendly interface
* Added some ground work to satisfy AOL openID authentication using XRDS document.

= 2.7.11 =
* Upgraded HybridAuth library to 2.1.1
* Added an option to admin-settings to not to show complete logout warning on logout.
* Added Curl-SSL support check to requirements.
* Fixed Twitter multiple profiles issue.
* User is automatically logged in after email verification.
* Some minor changes to messages and code quality.

= 1.5.5 =
* Added admin controlled email verification for new users. This is quite useful where login provider do no validate user e-mail, enabling this will allow only users with active email account to register with you WordPress site.
* Added an option in admin-settings to enable showing on login provider icons on comment and registration page, this is will help users to directly logon from there without going to login page.
* Fixed a bug on admin-settings page where 'provider ordering' block was throwing error on new setup.
* Updated some code blocks to get more quality and made changes to some messages to make them more meaningful.
 
= 1.3.2 =
* Logged -in user profile picture/avatar source can be controlled from plugin settings. By default WordPress tries to fetch avatar from Http://gravatar.com using email address in you profile, you can override that setting from plugin settings page and force WordPress to get profile picture/avatar from social media provider user is currently logged-in with.

= 1.2.2 =
* Added functionality to set display order of providers on login page
* Added new option in settings page to set how authentication will open (There are 2 options - In page itself and In a pop-up window) 
* Fixed a bug related to "Not all Google contacts are shown" thread raised by some user on support.

= 1.0.1 =
* Fix 'file not found error' when authenticating with a provider.

= 1.0 =
* First stable release

== Upgrade Notice ==

= 3.11.13 =
There has been addition of 4 new features and 3 bug fixes since last release. Update to get latest and enjoy more features.

= 2.7.11 =
There has been addition of 3 new features and 5 bug fixes since last release. Update to get latest and enjoy more features.

= 1.5.5 =
There has been addition of 2 new features and 3 bug fixes since last release. Update to get latest and enjoy more features.

= 1.3.2 =
There has been addition of 1 new feature since last release. Update to get latest and enjoy more features.

= 1.2.2 =
There has been 1 bug fix and addition of 2 new features since last release. Update to get latest.

= 1.0.1 =
There has been 1 bug fix since last release. Update to get latest.

== Live Demo ==

See the [live demo](http://labs.3pillarglobal.com/socialauth-wp-demo/wp-login.php) now!

== Features == 

* Authenticate users with Facebook, Yahoo, Google, MSN, Twitter, MySpace and LinkedIn etc (Provider support depends on provider supported by HybridAuth library).
* Access profile of logged in user (Email, First name, Last name, Profile picture)
* See contacts/friends of logged in user. Friend information contains information such as email, profile URL and name.
* More control over logout from application as well as authenticating provider.
* Administrator can control the default role for users who register via SocialAuth-WordPress.
* Administrator can set display order of providers for login page.
* Added new option in settings page to set how authentication will open (There are 2 options - In page itself and In a pop-up window) 

== Benefits ==

* Your blog users - Instead of creating new account on website, users can use their existing accounts from popular providers like Facebook etc. making it easier for them to access/contribute content.
* Blog administrators/owners - With no registration requirement, users can quickly login to the site and use its features. Further, users trust big providers (like Facebook etc.) making them comfortable in login process. This fast and trusted login process definitely attracts potential users and increase site popularity. Site administrator can set the permission for users who will login with external login provider.

== Plugin Settings ==

* SocialAuth-WordPress provides a nice settings interface to make it easy to use and configurable for your users and administrators out of the box.
* You can configure the default role which will be given to users which will connect to your app with help of this plugin.
* You can also set up a default landing page for the users using logon features of this plugin.
* Setting interface allows you to enable disable individual provider.
* When registering with Logon provider to get app_key and app_secret, some case you require you to supply a redirect_uri; you can get that from settings page.
* Administrator can also control how logon prompts appear to users. It can be either on same window or a pop up window.
* Administrator can control showing on login provider icons on comment and registration page, this is will help users to directly logon from there without going to login page.
* Administrator can enable optional e-mail verification for new users to force email verification when a new user first time comes to your site. This will only applied to users coming through providers which do not share user email in open-auth/social-auth
* Administrator can control whether or not to show complete session end message on logout or not.

== Credits ==

* HybridAuth Library - A open source social sign on php library residing in core of plugin and providing interface to connect to various login providers.
* A lot many thanks to Viruthagiri Thirumavalavan (one of most active plugin users) for using, raising bugs and suggesting enhancements to make this plugin better. 
