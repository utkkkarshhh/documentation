---
myst:
  html_meta:
    "description": "Sphinx themes and extensions"
    "property=og:description": "Sphinx themes and extensions"
    "property=og:title": "Sphinx themes and extensions"
    "keywords": "Documentation, Plone, Sphinx, reStructuredText, MyST, Markdown, themes, sphinx-book-theme, pydata_sphinx_theme, extensions"
---

(contributing-sphinx-themes-and-extensions)=

# Sphinx themes and extensions

We learned the hard way that maintaining the design and features of documentation is a lot of work.
To make all documentation maintainable, we use actively developed themes and extensions to build the documentation.

## Themes

When customizing the theme, we use [Sphinx Book Theme](https://sphinx-book-theme.readthedocs.io/en/stable/), which in turn depends on [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html).
See their documentation for features, tips, and tricks that you might want to include in your documentation.

We minimize the customizations of these themes as much as possible.
The one large customization is the search filter by part of the documentation, implemented in modifcations to the templates, {file}`_static/searchtools.js`, and the CSS file {file}`_static/custom.css`.


## Extensions

We use several Sphinx extensions to enhance the presentation of Plone documentation.

-   [`sphinx.ext.graphviz`](https://www.sphinx-doc.org/en/master/usage/extensions/graphviz.html) allows you to embed [Graphviz](https://graphviz.org/download/) graphs in your documents.
-   [`sphinx.ext.intersphinx`](https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html) provides linking between separate projects that use Sphinx for documentation.
-   [`sphinx.ext.todo`](https://www.sphinx-doc.org/en/master/usage/extensions/todo.html) adds support for todo items.
-   [`sphinx_copybutton`](https://sphinx-copybutton.readthedocs.io/en/latest/index.html)  adds a little "copy" button to the right of code blocks.
-   [`sphinx-design`](https://sphinx-design.readthedocs.io/en/latest/) adds grids, cards, icons, badges, buttons, tabs, and dropdowns.
-   [`sphinx_sitemap`](https://pypi.org/project/sphinx-sitemap/) generates multiversion and multilanguage [sitemaps.org](https://www.sitemaps.org/protocol.html) compliant sitemaps.
-   [`sphinxcontrib.httpdomain`](https://sphinxcontrib-httpdomain.readthedocs.io/en/stable/) provides a Sphinx domain for describing HTTP APIs.
    It is used by Plone's {doc}`plone.restapi/docs/source/index`.
-   [`sphinxcontrib.httpexample`](https://sphinxcontrib-httpexample.readthedocs.io/en/latest/) enhances `sphinxcontrib-httpdomain` by generating RESTful HTTP API call examples for different tools from a single HTTP request example.
    Supported tools include [curl](https://curl.se/), [wget](https://www.gnu.org/software/wget/), [httpie](https://httpie.io/), and [python-requests](https://requests.readthedocs.io/en/latest/).
    It is used by Plone's {doc}`plone.restapi/docs/source/index`.
-   [`sphinxcontrib.video`](https://pypi.org/project/sphinxcontrib-video/) allows you to embed local videos as defined by the HTML5 standard.
-   [`sphinxext.opengraph`](https://pypi.org/project/sphinxext-opengraph/) generates [OpenGraph metadata](https://ogp.me/).
-   [`sphinx.ext.viewcode`](https://www.sphinx-doc.org/en/master/usage/extensions/viewcode.html) generates pages of source code modules and links between the source and the description.
    It is used by {doc}`/plone.api/index`.
-   [`sphinx.ext.autosummary`](https://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html) generates function/method/attribute summary lists.
    It is used by {doc}`/plone.api/index`.
