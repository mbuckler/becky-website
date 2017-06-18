# Becky's Personal Website

This is the repo containing Rebecca Smith's personal website. It was
written by Becky Smith and Mark Buckler, and uses a theme based on the
[Hugo Artist's Theme](https://github.com/digitalcraftsman/hugo-artists-theme/tree/2873e529a336f620000cb4852155cd53d93e2f8b).

To view the website go to [http://becky.gallery](http://becky.gallery)!

## How to add new pictures

You can add new pictures in `becky-website/static/img/work/`. Putting
each section in its own folder will help keep things organized.

## How to add a new work (art) category

1) Add a new markdown file in `becky-website/content/work/` named by the
new kind of category you are adding. An example could be `portraits.md`.

2) Edit your new markdown file to add descriptions and/or images. Add
images with the following format:

    `![Portraits](img/work/portraits/image_name.jpg)`

## How to update the website after making changes

1) If you haven't yet, install Hugo

    [Hugo install directions](https://gohugo.io/overview/installing/)

2) Change to the `becky-website` directory

2) Rebuild your website with Hugo

    `> hugo`


3) Add your changed files with git

    Any image files you changed:

    `> git add becky-website/static/img/work/portraits`

    Any category files you changed:

    `> git add becky-website/content/work/portraits.md`

    The files containing your rebuilt website:

    `> git add docs/`

4) Commit your changes

    `> git commit`

5) Fill out the commit form (describe what you changed). If you are
using Emacs as your text editor: type in your message, exit with
`ctrl-X`, hit `Y` to say yes to exiting and saving, and finally
finish by pressing `Enter`.

6) Push your changes to both the github repo and the web!

    `git push`
