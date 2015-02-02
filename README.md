
This is a Jekyll plugin for Twitter Emoji. 
It is based heavily* on the work of 

[@ellekasai](https://github.com/ellekasai) 

in the case of the css file that reference the required assets;

and

[@23maverick23](https://github.com/23maverick23) 

in the case of the Jekyll source.

You can find the css file [here](https://github.com/ellekasai/twemoji-awesome). 

Just place it in your css directory;

add a line like 
```
<link rel="stylesheet" href="{{ "/css/twemoji-awesome.css" | prepend: site.baseurl }}">
```
and you should be good to go.

Install: Place in the _plugins directory. 

Usage:

{% twa twa-heart %}

It will work with any formatting from the third column on the demo page for [Twemoji Awesome](http://ellekasai.github.io/twemoji-awesome/). 

See notes there and use the [Emoji Cheatsheet](http://www.emoji-cheat-sheet.com/) for names.

Working example:
- http://ezmyrelda.com/2010/07/06/things-are-amazing/

*read: essentially lifted.

Compatibility notes:

Works under the 3.0.0 dev version recently released with "gem 'jekyll'" in the gemfile.

Likely works under 2.4.0 as well. Can't say for any other version. I never got 2.5.3 to work right.
