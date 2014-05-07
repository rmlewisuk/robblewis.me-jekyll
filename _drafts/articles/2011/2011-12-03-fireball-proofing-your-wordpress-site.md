---
title: Fireball Proofing Your Wordpress Site
permalink: /fireball-proofing-your-wordpress-site/
date: 2011-12-03 15:25:38
layout: post
---

Thanks to the amazing guys over at Panic, on the 28th of November, my blog crashed. Overloaded with traffic. The reason? [This](https://twitter.com/#!/panic/status/141261387686092800): ![Panicstatus](http://therobb.com/wp-content/uploads/2011-12-panicstatus.png) In the next two hours after this tweet, I got around 1000 visitors an hour. Specifically to [this page](http://therobb.com/2011-11-my-new-tattoo/). I was not expecting that much traffic, especially seeing as I only have 11 subscribers through RSS and about 250 Twitter followers. I had read about installing WPSuperCache in the past but I hadn't deemed it necessary. Here's how to install and setup WPSuperCache and, in turn, stop your site from getting Fireballed.  [WPSuperCache](http://wordpress.org/extend/plugins/wp-super-cache/) is a Wordpress plugin that _generates static html files from your dynamic Wordpress blog._ This means when people visit your site, they are served the static version of the page instead of using PHP scripts to generate the page. To install the plugin visit <http://wordpress.org/extend/plugins/wp-super-cache/>, download the zip file and then extract it to your Wordpress directory at _wp-content/plugins_. Alternatively, you can install it via your Wordpress dashboard under _plugins>add new_ and search for 'WPSuperCache'. Now from the dashboard plugin page, activate the plugin. ![Installsupercache](http://therobb.com/wp-content/uploads/2011-12-installsupercache.png) Once you have activated, go to the settings page (_Settings>WP Super Cache_). Depending on your setup, you may need to add this to your _wp-config.php_ file: _define('WP_CACHE', true);_. Once this is done, you may have some warnings at the top of the page mostly relating to file permissions. Make the changes mentioned in these warnings and then you should be able to press the _test cache_ button to check if you have everything setup correctly. If setup correctly, you should see a message like this: ![Cachetest](http://therobb.com/wp-content/uploads/2011-12-cachetest.png)