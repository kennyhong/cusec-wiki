README
======

First things first
------------------

Learn [Markdown](https://help.github.com/articles/github-flavored-markdown)! Then check out MDwiki's [quick start](http://dynalon.github.io/mdwiki/#!quickstart.md).

Whenever you feel stuck, go to [MDwiki's own site](http://mdwiki.info) for further information.

Getting Started
---------------

Structure
---------

_All file references here are relative to their respective language folder._

| Name | Type | Description |
| :--- | :--- | :--- |
| `index.md` | File | Starting point (a.k.a. "home page") for your wiki. **Note this is not the `index.html`, but `index.md`**! |
| `navigation.md` | File | Various settings of your wiki (e.g., name of your wiki, items in the navigation bar at the top, etc.) |
| `config.json` | File | If you don't know what this is for, don’t touch it. |
| `pages` | Folder | Ideally, inside this folder, you create one `*.md` file for every page inside your wiki (e.g., `foo.md`, `much-longer-names-are-also-okay.md`, etc.) You can also create as many subfolders as you need, just remember to link them accordingly. |
| `uploads` | Folder | An example folder structure where you could put other files. **Although it is best to host your files somewhere else, like Dropbox, or a CDN, etc.** |

Best Practices
--------------

### Relative URLs

Instead of using absolute URLs when linking one wiki page to another, use relative URLs.

For instance if `en/pages/foo.md` page had to link to `en/pages/bar.md`, it is enough to just add `[Click here](bar.md)` in your markdown.

### Don't Host Your Uploads in Git(Hub)

Instead of hosting your uploads inside the `uploads` folder, consider using Dropbox, Google Drive, or a CDN.

### Add References to Uploads

**Whenever you can, avoid hosting your uploads using Git(Hub).**

If you _must_ add references to files hosted inside the `uploads` folder here's how to do it, for instance: `![Image Title](uploads/images/foo.png)`. Add that in your markdown and you're good to go.


How to Preview
==============

In order to preview your changes locally, prior to publishing online, you may need to take some actions. Below some starting points for each operating system, also check out MDwiki's [frequently asked questions](http://dynalon.github.io/mdwiki/#!faq.md) section for some ideas.

Mac OS
------

The easiest way to serve up static sites on a Mac is to use [Anvil](http://anvilformac.com). Go ahead and download it from their website, install and add a site using the status bar icon: simply select the folder where your wiki is located on your Mac.

If you don't want to download any apps, you can use the Terminal on your Mac and Python. To do this, go to your site folder in the Terminal app and type `python -m SimpleHTTPServer 8000`. This will start running a local server which you can navigate to by typing the URL `localhost:8000` in any web browser.

Windows
-------

You can use [Fenix](http://fenixwebserver.com) to host a static site on windows. Fenix also comes with lots of advanced functionality that you might not use. Fenix can also run on a Mac.

Linux
-----

You can use [Prax](http://ysbaddaden.github.io/prax/). Prax is a pure ruby alternative to Pow!! that runs on GNU/Linux.


