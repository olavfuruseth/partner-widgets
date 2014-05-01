# BaseKit Partner Widgets

BaseKit is the world's fastest growing website builder. It is used by over 100 hosting companies around the world. Every month, tens of thousands of new BaseKit sites are created and published.

To find out more about BaseKit, please visit [basekit.com](http://basekit.com). If you are interested in becoming a BaseKit partner, and offerring a world-class website builder to your customers, you can find out more at [basekit.com/partners](http://basekit.com/partners).

## How It Works

We provide our partners with the use of simple sign-up and login widgets that can be used on any website. These can be deployed in minutes, so you can offer the BaseKit website builder to your users with minimal effort.

There is a basic demo of the widgets available at [partners.basekit.com/widget-test.htm](http://partners.basekit.com/widget-test.htm). Please note that there is no styling on this page yet, this is coming soon.

### Sign Up Widget

This is a widget that will create a BaseKit user and website. The user that is created will be assigned to your partner account.

You will be paid comission for any users on your account who go on to subscribe to a premium BaseKit package.

### Login Widget

This widget allows an existing user to login to BaseKit.

Note that this will only allow users assigned to your partner account to login.

## Sample Code

Please find a sample HTML file in this repository that can be used to test both widgets.

[Sample HTML](sample.htm)

The only change that you need to make is to replace the partnerRef parameter with your partner reference. If you're not sure how to find this, please contact [partners@basekit.com](mailto:partners@basekit.com) and we will be able to provide you with this.

## Using The Widgets

The widgets require [jQuery](http://jquery.com/) or [Zepto](http://zeptojs.com/) to be available.

If you're not already using jQuery, the suggested way to include it is via Google's CDN. The following line of code can be used, and should be placed towards the end of your HTML body.

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
```

Somewhere **after** jQuery, you then need to include the BaseKit widget library. The following line of code can be used to do so:

```html
<script src="http://partners.basekit.com/embed.js"></script>
```

The widgets are available as jQuery plugins. These are methods that extend jQuery's capabilities, enabling all jQuery objects to access these methods.

The widgets need to be given a container element into which they will be rendered. This can be any block-level element, such as a div.

```html
<div id="signup"></div>
...
<div id="login"></div>
```

You can then use the jQuery plugins **signupWidget** and **loginWidget** to instantiaite the widgets. You will need to pass in your partner reference. If you're not sure how to find this, please contact [partners@basekit.com](mailto:partners@basekit.com) and we will be able to provide you with this.

```javascript
$("#signup").signupWidget({
    partnerRef: 123
}).on('success', function (event, firstName, lastName, email) {
    // your code goes here
});

$("#login").loginWidget({
    partnerRef: 123
}).on('success', function (event, userName) {
    // your code goes here
});
```

When either of the requests are successful the widget will trigger a **success** event notification with very basic details about the user signup or login details. This is ideal for hooking up with analytics. You would add your intergration code in the callback function.

## Styling The Widgets

We provide a stylesheet that can be used to give the widgets some basic layout and styling. If you're happy with the basic styles then please use this in your own projects directly. The following line of code can be used to do so, and should be placed somewhere in your HTML head.

```html
<link rel="stylesheet" href="http://partners.basekit.com/embed.css">
```

If you want to customise the widgets to match the other elements on your website, we suggest that you download the above CSS file and use it as a starting point.

## Troubleshooting

If you have any problems using the widgets then please contact [partners@basekit.com](mailto:partners@basekit.com) and we can help you to resolve them quickly.
