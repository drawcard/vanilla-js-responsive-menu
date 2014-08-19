Vanilla JS Responsive Menu
==========================

A vanilla JS responsive menu plugin

Todo
====

Split the JS into 2 or more files to be used as "plugins". For example not every site has submenus or a sticky / absolute menu.

Use
===

```
<script type="text/javascript">
    responsivemenu.init({
        wrapper: document.getElementsByClassName('navigation_container')[0],
        before_element: document.getElementsByClassName('logo_container')[0],
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