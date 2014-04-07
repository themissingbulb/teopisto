jQuery Teopisto
========

jQuery Teopisto is an effect sequencer which apply reveal effect to DOM objects in a order.

-----------
### What's Teopisto and why does it need?
With jQuery Teopisto, you can easily apply sequenced reveal effects to groups of objects. The effects are made possible with CSS transform, opacity and transition, that's why we highly recommend you to use Modernizr to check if the mentioned features are available in the user's browser. 

jQuery Teopisto is dependent to [jQuery Waypoints][1] and of course [jQuery] [2].

-----------
### How do you prepare Teopisto?
1. Simply put `jquery.teopisto.js` and the other dependencies inside your Javascript directory.
2. All the effects are created with css, so just in case you want to do fine tunes with the transition, you can edit the `teopisto.scss` file (Sorry LESS users).
3. Put `teopisto.css` inside your css folder.
4. Add this line of code to your website, `<script src="path/to/js/jquery.teopisto.js"></script>`
5. This one also, `<link rel="stylesheet" href="css/teopisto.css">`

-----------
### How to use Teopisto?
#### Basic usage
```
$('#container').teopisto();
```

#### Advanced usage
```
$('#container').teopisto({
    child: '*',
    interval: '380',
    offset: '68%',
    effect: 'zoom',
    random: false
});
```

-----------
### What are the options in the advanced usage?

#### child

With this option, you can choose to apply the effects only to the specific child of the container

*Default*: ```'*'```

#### interval

This option is for you to customize the sequence effect interval.

*Default*: ```'380'```

#### offset

This option is used to set the scrolling offset of the sequence, it can be in percentage or in pixels

*Default*: ```'68%'```

#### effect

There are a total of 10 sequence animation preset, they are ``zoom``, ``fade``, ``slideTop``, ``slideRight``, ``slideBottom``, ``slideLeft``, ``slideTop3d``, ``slideRight3d``, ``slideBottom3d``, ``slideLeft3d``

*Default*: ```'zoom'```

#### random

This option is used to shuffle the order of the animation sequence.

*Default*: ```'false'```

-----------
### Is this project usable?

To be honest with you, no, not really. 

The current build of this plugin is still very buggy in terms of targeting objects.

However if you are willing to repeat the initiation code several times, I'd say this plugin will work in no problem at all.

-----------
  [1]: http://imakewebthings.com/jquery-waypoints/
  [2]: http://jquery.com/