Lastfm
======

This plugin will get the recent tracks from a last.fm account and it produces structured HTML with in-build CSS classes for styling.

![Screenshot](http://farm8.staticflickr.com/7186/6895754387_b8286958b1_z.jpg)

How to use
----------

First you must to include the JS files in the head of your HTML document.

        #HTML
        <script src="http://www.google.com/jsapi?key=ABQIAAAA1XbMiDxx_BTCY2_FkPh06RRaGTYH6UMl8mADNa0YKuWNNa8VNxQEerTAUcfkyrr6OwBovxn7TDAH5Q"></script>
        <script type="text/javascript">google.load("mootools", "1.4.1");</script>
        <script type="text/javascript" src="lastfm.js"></script>

Define some DIVs to inject the badge

        #HTML
        <div class="yui-u first">
          <div id="result"></div>
        </div>
        <div class="yui-u">
          <div id="result2"></div>
        </div>

Then you can apply the method.

        #JS
        <script type="text/javascript">
           window.addEvent('domready', function(){
                 $('result').lastfm({username: 'aline_e_b'});
                 $('result2').lastfm({username: 'thinkphp'});
           }); 
        </script>

Example #1: http://thinkphp.ro/apps/lastfm/mootools/getJSON/

Example #2: http://thinkphp.ro/apps/lastfm/mootools/jsonp/

Example #3: http://thinkphp.ro/apps/lastfm/mootools/jsonp2/
