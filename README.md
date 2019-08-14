# twa for Jekyll

## About

This is a [Twitter Emoji](https://twemoji.twitter.com/) (Twemoji) plugin for Jekyll.

It is based heavily on the work of:

- [@ellekasai](https://github.com/ellekasai)'s Twemoji Awesome ([demo](http://ellekasai.github.io/twemoji-awesome/) / [repo](https://github.com/ellekasai/twemoji-awesome))
- [@23maverick23](https://github.com/23maverick23) for the Jekyll source.


## Installation

1. Download `twemoji-awesome.rb` and place it in the `_plugins` directory (option #1 in the Jekyll tutorial on [installing plugins](https://jekyllrb.com/docs/plugins/installation/));
2. Download either the CSS or the SCSS ([Sass](https://sass-lang.com/)) file from [ellekasai's repository](https://github.com/ellekasai/twemoji-awesome), under the folder `v1`;
3. Place the file in your CSS directory (Jekyll will compile the file for you, at build time, in case you pick Sass);
4. Link the CSS file in your HTML. For example:
```html
<link rel="stylesheet" href="{{ "/assets/twemoji-awesome.css" | prepend: site.baseurl }}">
```
5. That's it!


## Usage

### Emoji
You can insert a Twemoji by inserting the following expression to your post:

```
{% twa twa-heart %}
```

Where `twa-heart` may be replaced by another emoji besides "heart". Checkk the [Emoji Cheat Sheet](https://www.webfx.com/tools/emoji-cheat-sheet/) for valid emoji names. Note that underscores `_` must be replaced with hyphens `-`. So, for :stuck_out_tongue: (`:stuck_out_tongue:`), you'd use:

```
{% twa twa-stuck-out-tongue %}
```

### Size
You can also define a preset size by using `twa-lg`, `twa-2x`, `twa-3x`, `twa-4x` or `twa-5x`.

For example:
```
{% twa twa-pizza twa-5x %}
```
Would render a giant pizza!


# Compatibility

Works under the 3.0.0 dev version recently released with "gem 'jekyll'" in the gemfile.

Likely works under 2.4.0 as well. Can't say for any other version. I never got 2.5.3 to work right.
