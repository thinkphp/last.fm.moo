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
* (*String*)  result      - the id of the element where you'd want to put the badge.
* (*String*)  badgeid     - the id of the widget.
* (*String*)  badgeclass  - the css class of the widget.
* (*Integer*) amount      - the number of tracks to fetch.


### Returns

An `Lastfm` instance.

### Events

### Request

* (*Function*) - a function callback that is fired when the request is sent to the service last.fm API using YQL.

#### Signature
     onRequest(); 

#### Arguments

* (*void*) no arguments

### Complete

* (*Function*) - a function callback that is executed when the request is completed.

#### Signature

     onComplete(data); 

#### Arguments

* (*object*) data - the response from the service Last.fm API using Yahoo Query Language(YQL).


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
