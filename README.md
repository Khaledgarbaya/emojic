
[![emojic](http://i.imgur.com/bflsgPt.png)](#)

# emojic

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Version](https://img.shields.io/npm/v/emojic.svg)](https://www.npmjs.com/package/emojic) [![Downloads](https://img.shields.io/npm/dt/emojic.svg)](https://www.npmjs.com/package/emojic)

> Emoji in your Node.js command line apps.

In the screenshot below I'm using a Linux terminal emulator which doesn't support *colorful* emoji (in the way like OS X does).

[![emojic](http://i.imgur.com/o0DJDca.png)](#)

## :cloud: Installation

```sh
$ npm i --save emojic
```


## :clipboard: Example



```js
// Dependencies
const emojic = require("emojic")
    , colorIt = require("color-it")
    ;

console.log(emojic.x + " Something went wrong");
// => ❌ Something went wrong

console.log(emojic.whiteCheckMark + " Success");
// => ✅ Success

// If you want to color the things a little bit
// ...using color-it (you can find it on github.com/IonicaBizau/node-color-it)
console.log(" " + colorIt(emojic.x).red() + " " + colorIt("Some red error appeared").redBg());
console.log(" " + colorIt(emojic.smiley).green() + " " + colorIt("I am a happy man!").greenBg().wetAsphalt());
// Note: On Linux, ANSI styles will be used to color the output (see the screenshot)
// => ❌ Some red error appeared
// => 😃 I am a happy man

console.log(" " + colorIt(emojic.thumbsUp).green() + " " + colorIt("Thumbs up!").greenBg().wetAsphalt());
console.log(" " + colorIt(emojic.thumbsDown).green() + " " + colorIt("Thumbs down!").yellow());
```

## :question: Get Help

There are few ways to get help:

 1. Please [post questions on Stack Overflow](https://stackoverflow.com/questions/ask). You can open issues with questions, as long you add a link to your Stack Overflow question.
 2. For bug reports and feature requests, open issues. :bug:
 3. For direct and quick help from me, you can [use Codementor](https://www.codementor.io/johnnyb). :rocket:


## :memo: Documentation

Require the library using `var emojic = require("emojic")`. Then you can use the camel case notation for the emoji names (like in the example). Visit [emoji.muan.co](http://emoji.muan.co) to search the icons.
For example, if you want to display in console `:heart_eyes:` (:heart_eyes:), you will use `console.log(emojic.heartEyes)` (notice the camelCaseStyle)

## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:


## :cake: Thanks
Thanks to [**@muan**](https://github.com/muan) for creating the [`emojilib`](https://github.com/muan/emojilib) project we use here. :sparkles:

## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:


 - [`emoji-logger`](https://github.com/IonicaBizau/emoji-logger#readme)—Logging library based on flat colors and Emoji.
 - [`ntbk`](https://michaelsoolee.com/ntbk-journal/) (by Michael Lee)—A simple command-line journaling tool.

## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
