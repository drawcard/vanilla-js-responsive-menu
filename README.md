Vanilla JS Responsive Menu
==========================

A vanilla JS responsive menu plugin.

Dependencies
------------
Apollo JS | https://github.com/toddmotto/apollo
Load apollo first

Features
========

* Accessible friendly
* compressed 4kb
* IE9+ (If the script does not run you get the regular menu)

Use
===

To make sure that menu items don't show for a split second on mobile sized screens add the following:

```
<body class="no-js">
<script type="text/javascript">function hasClass(e,t){return e.className.match(new RegExp("(\\s|^)"+t+"(\\s|$)"))}var el=document.body;var cl="no-js";if(hasClass(el,cl)){var reg=new RegExp("(\\s|^)"+cl+"(\\s|$)");el.className=el.className.replace(reg," js-enabled")}</script>
```

The basic markup:

```
<div class="navigation_container">
    <ul class="closed">
        <li><a href="#">Item</a></li>
    </ul>
</div>
```

Place following on the bottom of your document:

```
<script type="text/javascript">
    responsivemenu.init({
        wrapper: document.querySelector('.navigation_container')
    });
</script>
```

Options
=======

wrapper
---

The container that wraps the menu

default: document.getElementsByTagName('nav')[0],

initiated_class
--------------

The class to attach to the wrapper when menu is initiated

default: 'initiated',

before_element
--------------

The element where the toggle button will be put before

default: '',

toggletype
----------

HTML element of the main toggle button

default: 'button',

toggleclass
-----------

The class of the main toggle button

default: 'togglebutton',

togglecontent
-------------

The value / text / html on the main toggle button

default: 'menu',

subtoggletype
-------------

HTML element of the sub toggle buttons

default: 'button',

subtoggleclass
-----------

The class of the sub toggle buttons

default: 'subtoggle',

subtogglecontent
-------------

The value / text / html on the sub toggle buttons

default: '+',

sticky
------

Use a sticky menu?

default: 0,

absolute
--------

Make the toggling menu absolute positioned

default: 0,

hideclass
---------

The class to add to elements that need to be hidden. Hiding happens with CSS

default: 'accessible-hide',

width
-----

The window width when menu has to become a full menu. You might need to change CSS as well when changing this value

default: 600