# BaseKit Partner Widgets

BaseKit is the world's fastest growing website builder. It is used by over 100 hosting companies around the world. Every month, tens of thousands of new BaseKit sites are created and published.

To find out more about BaseKit, please visit [basekit.com](http://basekit.com). If you are interested in becoming a BaseKit partner, and offerring a world-class website builder to your customers, you can find out more at [basekit.com/partners](http://basekit.com/partners).

## How It Works

We provide our partners with the use of simple sign-up and login widgets that can be used on any website. These can be deployed in minutes, so you can offer the BaseKit website builder to your users with minimal effort.

### Sign Up Widget

This is a widget that will create a BaseKit user and website. The user that is created will be assigned to your partner account. You will be paid comission for any users on your account who go on to subscribe to a premium BaseKit package.

### Login Widget

This widget allows an existing user to login to BaseKit.

Note that this will only allow users assigned to your partner account to login.

## Using The Widgets

The widgets require [jQuery](http://jquery.com/) or [Zepto](http://zeptojs.com/) to be available.

If you're not already using jQuery, the suggested way to include it is via Google's CDN. The following line of code can be used, and should be placed towards the end of the body tag in your HTML.

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
```

Somewhere **after** jQuery, you then need to include the BaseKit widget library. The following line of code can be used to do so:

```html
<script src="http://partners.basekit.com/embed.js"></script>
```

The widgets are available as jQuery plugins. These are methods that extend jQuery's capabilities, enabling all jQuery objects to access these methods.

The widgets need to be given a container element in which they will be rendered. This can be any block-level element, such as a div.

```html
<div id="signup"></div>
```

```javascript
$("#signup").signupWidget({
    partnerRef: 691
});
```
