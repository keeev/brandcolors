Brandcolors (LESS & Sass Variables)
===========

LESS and SASS variables for all known brands. Inspired by [Brandcolors](http://brandcolors.net/) and
some selfbuilt buttons in a sideproject a few days ago I thought it would be useful to have some brandcolors
as variable for LESS and Sass in every project I need them.


## Import
If you start your application from scratch you just can copy&paste or use `style.less`
which automatically imports the Button-Mixin and Brandcolors Stylesheet.

 ```css
@import "buttons/buttons-mixin.less";
@import "brandcolors.less";
 ```
 of course you can get them wherever you want as long as you take care of the path.

## How to use buttons?

In your template file you just give your button the class you add to the stylesheet later on.  

```html
<button class="facebook-button">
  facebook button
</button>
```

then you have to add:

```css
.facebook-button {
  .sharing-button-small (@facebook);
}
```
where `@facebook`is the color which is imported from the `brandcolors.less`-file
to your stylesheet where you define the button.
The buttons mixin currently provides styling for "small"-buttons.

If you use LESS or SASS and if you're looking for a way to organize your Sass/LESS checkout [Organize that Sass!](http://alistapart.com/blog/post/organize-that-sass) on A List Apart.

Currently there are the following services/brands:


### Social Networks

* Facebook
* Twitter
* Vine
* Linkedin
* Instagram
* Foursquare
* Swarm (Foursquare)
* Yo
* Tinder
* Xing
* Google+
* Medium
* Meetup

### Music / Video / Creativity

* Rdio
* Spotify
* SoundCloud
* Vimeo
* Kickstarter

### Development & Design

* Atlassian (Jira, Bitbucket, HipChat, ...)
* Github
* Dribbble
* Behance

### Tools/Services

* Dropbox
* Kippt
* Amazon
* Airbnb
* Designer News
* Evernote


Feel free to add others!
