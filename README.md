fancybox-rails
==============

Use [fancybox](http://www.fancyapps.com/fancybox/) with rails 3.2 asset pipeline.
Fancybox v. 2.1.3 updated

## Installation

This gem vendors jquery fancybox 2.1.3 for Rails 3.2 and greater. The files
will be added to the asset pipeline and available for you to use.

First add the following lines to your applications `Gemfile`:

``` ruby
gem 'jquery-rails'
gem 'fancybox-rails'
```

Then run `bundle install` to update your application's bundle.

Now you need to edit your `app/assets/javascripts/application.js`
file and add the following line:

``` javascript
//= require jquery
//= require fancybox
```

And then edit your `app/assets/stylesheets/application.css` file to
look something like:

``` css
/*
 *= require_self
 *= require fancybox
 *= require_tree .
 */
```

That's it!

## Usage

With the gem installed and included in your asset manifests, you can now
use fancybox as you normally would.

``` javascript
$(document).ready(function() {
  $("a.fancybox").fancybox();
});
```

## More information

* [Contributors](https://github.com/almaron/fancybox-rails/contributors)
* [DHH's RailsConf 2011 talk on the rails 3.1 asset pipeline](http://www.youtube.com/watch?v=cGdCI2HhfAU)

Copyright (c) Chris Mytton

## License

[Fancybox 2 license](http://www.fancyapps.com/fancybox/#license)