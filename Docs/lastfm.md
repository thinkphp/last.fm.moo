Class: Lastfm (#Lastfm)
===============================

###Implements:

Options, Events

Lastfm Method: constructor (#Lastfm: constructor)
---------------------------------------------------------

### Syntax: 

    var lastfm = new Lastfm(options);

### Arguments:


### options:


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
