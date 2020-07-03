astral-jekyll
=============

Original - Astral theme by Pixelarity:
--------------------------------------

-   Link: https://pixelarity.com/astral

-   License: https://pixelarity.com/license

 You should obtain the correct permission to use the original theme and files
before using this one.

To Do:
------

-   Add breadcrumb navigation as an include.

-   Add post information to individual layout (author, date, category, tags,
    etc)

Modifications:
--------------

-   Navigation links are set up in navigation.yml data file.

    -   name - required. The display name of the link.

    -   hash - optional. Override the hash that is used for internal links. The
        default is the lower case URL encoded ‘name’.

    -   url - required for external links.

    -   icon - Defaults to \`fa-link\`. A Font Awesome icon to display. See
        https://fontawesome.com/cheatsheet

    -   iconPrefix - solid/brand/etc. See
        https://fontawesome.com/v5.9.0/how-to-use/on-the-web/referencing-icons/basic-use.

    -   target - Optional. anchor target. Use ‘_blank’ to open in a new tab.

-   The index page uses documents in the index_collection folder to generate its
    content. This allows you to edit the sections as separate files, not one
    continuous block of HTML.

-   CSS

    -   Links have been refactored to use the sass folder.

    -   Automatically compressed for smaller file size

    -   Added custom.scss for easy style changes

    -   Some minor changes to font awesome handling in nav links and CSS

-   added file caching in pwa.js. cache first then network update method.
    disabled by default to allow easier development

-   using \_data/main.yml to for titles and landing content layout

-   \#hash handling changed to force navigation to homepage. '\#work' became
    '/\#work'. To allow for off-nav pages.

-   handled lists of documents in the post_list include with three *basic*
    layouts: card, text, image.
