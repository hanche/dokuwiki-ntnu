# Using menus #

## Global menu ##

The template looks for a page called `mainmenu` to in the site root (`http://<my site>/mainmenu`). If present, the menu will be used globally throughout the site.

## Namespace menus ##

If present, namespace menus will appear beneath the global menu. The template expects these pages to called `menu` and to be placed in the namespace/folder where they are to be displayed.

A namespace menu will be inherited until an namespace further down in the hierarchy declares a new menu. The new menu will then replace the old one in the left hand column.

_Tip: A namespace menu might contain only whitespace, if it's only purpose is to stop the previous menu from being displayed._

## Menu syntax ##

Menus are expected to contain **only** a level 2 heading and an unordered list of links. Anything else could/will break the layout. You may define multiple menus in one menu file (heading + list + heading + list etc...)

Expanding menus are created using nested levels of unordered lists, and will be expanded automatically when the page they appear beneath is active.

```
===== My menu =====

  * [[first|First menu item]]
    * [[firstsub|Sub item of the first]]
  * [[second|Second menu item]]

```

The page names `mainmenu` and `menu` are configurable in the "Template settings" section.