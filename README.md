astral-jekyll
=============

### Original - Astral theme by HTML5 UP / Pixelarity:


* Original: [Astral - HTML5 UP](https://html5up.net/astral)
* License: [Creative Commons Attribution 3.0 License](https://html5up.net/license)

For attribution free use, go to:
* [Astral - Pixelarity](https://pixelarity.com/astral)
* [License](https://pixelarity.com/license)

### To Do:

- Improve caching in pwa.js
- Add image / FA icon replacement to category and tag links

### Modifications:

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

-   hash handling changed to force navigation to homepage. '\#work' became
    '/\#work'. To allow for off-nav pages.

-   Browse page: filter categories and tags. Uses the same ‘articles’ layout as
    the index page.

-   CSS

    -   Links have been refactored to use the sass folder.

    -   Automatically compressed for smaller file size

    -   Added custom.scss for easy style changes

    -   Some minor changes to font awesome handling in nav links and CSS

-   Added file caching in pwa.js. cache first then network update method.
    disabled by default to allow easier development

-   handled lists of documents in the post_list include with three *basic*
    layouts: card, text, image.
