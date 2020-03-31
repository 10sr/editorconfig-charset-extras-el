[![MELPA](https://melpa.org/packages/editorconfig-charset-extras-badge.svg)](https://melpa.org/#/editorconfig-charset-extras)
    

editorconfig-charset-extras.el
==============================

Extra EditorConfig Charset Support


Overview
--------


This library adds extra charset supports to editorconfig-emacs.
The list of supported charsets is taken from the result of
`coding-system-list'.

For example, add following to your `.editorconfig`
and `sjis.txt` will be opend with `sjis' encoding:

    [sjis.txt]
    charset = sjis

Alternatively, you can specify `emacs_charset` as:

    [sjis.txt]
    emacs_charset = sjis

If both `charset' and `emacs_charset' are defined, the value of
`emacs_charset' takes precedence.


To enable this editorconfig plugin, add following to your init.el:

    (add-hook 'editorconfig-custom-hooks
              'editorconfig-charset-extras)


License
-------

This software is unlicensed.
