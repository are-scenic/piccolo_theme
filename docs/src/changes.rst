Changes
=======

0.12.0
------

You can now specify the source code URL, and it will show in the nav bar.

.. code-block:: python

    # conf.py

    html_theme_options = {
        "source_url": 'https://github.com/piccolo-orm/piccolo_theme/'
    }

The icon is inferred automatically based on the URL (in the above example, we
show the GitHub logo). You can explicitly set the icon if you prefer:

.. code-block:: python

    # conf.py

    html_theme_options = {
        "source_url": 'https://self-hosted.foo.com/',
        "source_icon": "gitlab"
    }

-------------------------------------------------------------------------------

0.11.1
------

Minor style fix on search page.

-------------------------------------------------------------------------------

0.11.0
------

Fixed some styles in Sphinx v5.

-------------------------------------------------------------------------------

0.10.2
------

Drop Python 3.7 specific syntax.

-------------------------------------------------------------------------------

0.10.1
------

Fix typo in ``setup.py``.

-------------------------------------------------------------------------------

0.10.0
------

Added support for Python 3.6, as many Ubuntu systems will still be using that
version, and Sphinx still supports it. Thanks to @oncilla for reporting this
issue.

-------------------------------------------------------------------------------

0.9.0
-----

Improved the appearance of autodoc output for C files (when using
`breathe <https://breathe.readthedocs.io/en/latest/>`_). Courtesy @thijsmie.

-------------------------------------------------------------------------------

0.8.1
-----

Changed the arrow symbols - they didn't look great on mobile.

-------------------------------------------------------------------------------

0.8.0
-----

Added spacing between sections, so it's not necessary to add horizontal
dividers any more.

.. code-block:: rst

    My Heading
    ==========

    Section 1
    ---------

    Some content

    -------------------------------------------

    Section 2
    ---------

    Some content

We can now just do:

.. code-block:: rst

    My Heading
    ==========

    Section 1
    ---------

    Some content


    Section 2
    ---------

    Some content

Other minor changes:

* Using unicode triangle character instead of < for some links
* Plain admonitions are now styled properly:

.. code-block:: rst

  .. admonition:: A custom admonition

     This is my custom admonition!

-------------------------------------------------------------------------------

0.7.1
-----

Improvements to the notification feature - it was causing too many browser
reflow operations.

-------------------------------------------------------------------------------

0.7.0
-----

A notification can now be shown at the top of each page.

.. code-block:: python

    # conf.py
    html_theme_options = {
        "banner_text": 'Welcome to our amazing documentation!',
        "banner_hiding": "permanent"
    }

This involved quite a few CSS changes - please clear your browser cache if
anything appears broken.

-------------------------------------------------------------------------------

0.6.0
-----

If ``html_short_title`` is in ``conf.py`` then this is used in the nav bar
instead of the full project title.

-------------------------------------------------------------------------------

0.5.1
-----

Fixed dark mode styles - some elements weren't visible. Thanks to @alorence for
reporting this issue.

-------------------------------------------------------------------------------

0.5.0
-----

Added table styles.

-------------------------------------------------------------------------------

0.4.0
-----

Improved the appearance of autodoc output for C++ files (when using
`breathe <https://breathe.readthedocs.io/en/latest/>`_). Courtesy @thijsmie.

-------------------------------------------------------------------------------

0.3.0
-----

Added dark mode.

-------------------------------------------------------------------------------

0.2.5
-----

Improved search styles.

-------------------------------------------------------------------------------

0.2.4
-----

Added missing ``requirements.txt`` file to manifest. Thanks to @moorepants for
reporting this.

-------------------------------------------------------------------------------

0.2.3
-----
Make the ``page contents`` text smaller when the right hand sidebar is hidden.

-------------------------------------------------------------------------------

0.2.2
-----
Fix missing static files.

-------------------------------------------------------------------------------

0.2.1
-----
Fix missing static files.

-------------------------------------------------------------------------------

0.2.0
-----

Improved the main header on mobile - the search bar is replaced with a search
icon. Also increased the size of the touch targets for showing / hiding the
right sidebar, for easier use on mobile. See `PR 7 <https://github.com/piccolo-orm/piccolo_theme/pull/7>`_.
