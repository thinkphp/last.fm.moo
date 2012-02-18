Class: Lastfm (#Lastfm)
===============================

###Implements:

Options, Events

Lastfm Method: constructor (#Lastfm: constructor)
---------------------------------------------------------

### Syntax: 

    var lastfm = new Lastfm(options);

### Arguments:

1. options - (*Object*) An object containing the Lastfm instance's options.

### options:

* (*String*)  username    - the Last.fm username to fetch the recent tracks of.
* (*String*)  result      - the place where you want to put the badge
* (*String*)  badgeid     - the widget's ID 
* (*String*)  badgeclass  - the badge's class
* (*Integer*) amount      - the number of tracks to fetch.


### Returns

An `Lastfm` instance.

Element Method: lastfm (#Element: lastfm)
-------------------------------------------------

`Lastfm` extends Element with this method.

### Syntax:

    myElem.lastfm(options);

### Arguments

1. options 
 
### Returns

* (element) 'This' element.

### Example

    #HTML
    <div id="tracks"></div>  
    <div id="tracks2"></div>  

    #JS
    window.addEvent('domready', function() {
        $('tracks').lastfm({username: 'aline_e_b'});
        $('tracks2').lastfm({username: 'thinkphp'});
    }); 
