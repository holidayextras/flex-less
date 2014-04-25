Flex Less
=========

Flexbox is awesome! It's a powerful addition to CSS and you should be using it NOW!
The CSS Flexible Box Layout Module (www.w3.org/TR/css3-flexbox/) has been a Candidate Recommendation since September 2012.

> "That’s cool! But I can’t use it because XYZ doesn’t support it."

Since when has that stopped us using box-shadows or border-radius?
Use flexbox now on small page components as progressive enhancement, and with Flex Less you wont have to worry about the countless vendor prefixes for flexbox.

Flex Less is a mixin created to enable to to use all basic functions of CSS flexbox for all supported flexbox browsers.


Flexbox support
-------
2009 syntax
```display:box```
with -webkit- prefix
ANDROID
SAFARI v.3+
BLACKBERRY v.7+

2011 syntax
```display:flexbox```
with -ms- prefix
INTERNET EXPLORER v.10

Current syntax
```display:flex```
CHROME
FIREFOX
OPERA
INTERNET EXPLORER v.11
ANDROID v.4.4
SAFARI v.6+
BLACKBERRY v.10+

Flexbox
-------
@flex: flex, flex-inline
  
Flexbox Direction
-------
@type: row, column
@direction: normal, reverse

Flexbox Wrap
-------
@wrap: wrap, nowrap, wrap-reverse
  
Flexbox Justify Content
-------
@justify-content: start, end, center, space-between, space-around

**FIXME** - Creates duplicate CSS
  
Flexbox Align Items
-------
@align-items: center, baseline, stretch, start, end
  
Flexbox Align Content
-------
@align-items: start, end, center, space-between, space-around

**FIXME** - Creates duplicate CSS
