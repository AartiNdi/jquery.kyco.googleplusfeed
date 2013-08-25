jquery.kyco.googleplusfeed
==========================

The best Google+ feed widget out there!

This is a simple Google+ feed widget which makes use of http://plusfeed.frosas.net

Take a look at the [demo](http://tr.im/49tpy).

How to install
--------------

Download the js file and include it in your head after including jquery:

    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"><script>
    <script src="jquery.kyco.googleplusfeed.min.js"><script>

Also include the css file and grab the loader.gif from the demo directory:

    <link rel="stylesheet" href="jquery.kyco.googleplusfeed.css">

Create a div to hold the feed and then pull the feed into it by calling the 
kycoGooglePlusFeed method with the specified Google+ ID:

    <script>
        $(document).ready(function() {
            $('.mydiv').kycoGooglePlusFeed('116899029375914044550');
        });
    </script>

What a customisation looks like:

    <script>
        $(document).ready(function() {
            $('.mydiv').kycoGooglePlusFeed({
                id: '116899029375914044550',
                feedPosts: 2,
                postsIncrement: 1,
                maxPosts: 5,
                profileImageSize: 150
            });
        });
    </script>


Configuration - kycoGooglePlusFeed({ <em>options</em> })
-------------------------------------------------

    id: /* Google+ ID */

The Google+ ID used to generate the feed.

    feedPosts: 3,

Feed posts to show on load.

    postsIncrement: 3,

Number of feed posts to show on "Show more" button click.

    maxPosts: 20,

Max number of posts to pull before "Show more" will go to Google+, cannot exceed 20 
because of Google API in use.

    profileImageSize: 50

Image size of the profile image, max size is 250. Also adjust css if changing the default.


Styling
-------

By default you will have to also include the loader image from the demo file if you want
a spinner to appear while the feed is loading.


Support
-------

For bugs or improvements please use the issues tab or email info@kyco.co.za.
