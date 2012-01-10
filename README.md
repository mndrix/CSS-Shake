CSS Shake
=========

CSS Shake is a small utilty for finding unused CSS selectors in your
stylesheets.  It scans all your HTML and JavaScript files for
CSS classes and IDs and reports rules that can't possibly match.
It even handles classes and IDs **added from jQuery**.

Installing
----------

    $ cpanm CSS
    $ wget https://github.com/mndrix/css-shake/raw/master/css-shake

Running
-------

    $ ./css-shake my-styles.css
    Parsing CSS ...
    Finding HTML and JS files ...
    Finding classes and ids ...
    Unused CSS selectors:
    #foo #bar ul.baz      (no #bar)
    li.widget   (no .widget)

Status
------

CSS Shake is still in very early development.  It might not work for you at
all.
