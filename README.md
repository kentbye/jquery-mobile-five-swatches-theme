jquery-mobile-five-swatches-theme
=================================

The default theme for jQuery mobile 1.4 only has two swatches, and it eliminates the blue, yellow, and additional grey swatch from the default theme.

This five swatches theme maintains the improvements of the new default 1.4 theme, but adds back the three deprecated swatches using the ThemeRoller.

## Usage
Copy all of the files in the themes directory into your CSS folder, and then be sure to add the following two lines:

    <link rel="stylesheet" href="css/themes/jquery-mobile-five-swatches.min.css" />
    <link rel="stylesheet" href="css/themes/jquery.mobile.icons.min.css" />

These can go before the other jQuery CSS and JavaScript files of

    <link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.0/jquery.mobile.structure-1.4.0.min.css" /> 
    <script src="http://code.jquery.com/jquery-1.10.2.min.js"></script> 
    <script src="http://code.jquery.com/mobile/1.4.0/jquery.mobile-1.4.0.min.js"></script> 

## Usage
I wanted to have some more color options like is shown in this [JSfiddle example](http://jsfiddle.net/Sgrve/20/) using the default jQuery mobile theme from version 1.3.

However, three swatches from the default jQuery Mobile theme that were deprecated, and according to the [jQuery Mobile 1.4 Upgrade guide](https://github.com/jquery/jquery-mobile/wiki/1.4-Upgrade-Guide):

> The default theme has been replaced and the new theme has two swatches, A (light) and B (dark)… If you were using the blue or yellow style from the B and E swatch you have to create a custom swatch for which you can use the [ThemeRoller](http://themeroller.jquerymobile.com/).

This means that the C & D swatches were folded into A, the default dark background was moved to theme B, and the yellow E swatch was eliminated all together.

They state that "For convenience we updated the 1.3 default theme to 1.4 and added it as ["classic" theme](http://view.jquerymobile.com/master/demos/theme-classic/) to the demos."

However, this specific theme has dark as the default A theme, and doesn't include the new and improved A and B swatch designs from the new 1.4 default jQuery mobile theme. I wanted to have the new default light theme as swatch A, but also have access to the legacy colors, so I merged the two with the ThemeRoller.

## ThemeRoller Creation Process

I first copied the latest [1.4 jQuery mobile css theme](https://raw.github.com/jquery/jquery-mobile/master/css/themes/default/jquery.mobile.theme.css) from the master branch and then pasted that code into the "Import or Upgrade" tab on the [ThemeRoller](http://themeroller.jquerymobile.com/).

I then opened another window, and copied the [jQuery 1.3 mobile default CSS](https://raw.github.com/jquery/jquery-mobile/1.3-stable/css/themes/default/jquery.mobile.theme.css) into another [ThemeRoller](http://themeroller.jquerymobile.com/).

* I then ported the swatch B from classic 1.3 to swatch C in the 1.4 five-swatches-theme
* Swatch D from classic 1.3 into swatch D in the 1.4 five-swatches-theme
* Swatch E from classic 1.3 into swatch E in the 1.4 five-swatches-theme
* The default A & B swatches in 1.4 were maintained.

## Making further modifications to this theme.
You can make further modifications to this theme by uploading the uncompressed `jquery-mobile-five-swatches.css` file to the [ThemeRoller](http://themeroller.jquerymobile.com/), making your desired modifications, and then downloading the file and following the same usage instructions above.


