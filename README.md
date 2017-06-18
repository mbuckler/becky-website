# Becky's Personal Website

This is the repo containing Rebecca Smith's personal website. It was
written by Becky Smith and Mark Buckler, and uses a theme based on the
[Hugo Artist's Theme](https://github.com/digitalcraftsman/hugo-artists-theme/tree/2873e529a336f620000cb4852155cd53d93e2f8b).

To view the website go to [http://becky.gallery](http://becky.gallery)!

## How to add new pictures

1) Make a new folder for a new work category. This directory's name must
be lower case, and in `becky-website/static/img/work/`. 

2) Copy in your image files into the directory you just made.

3) Copy one of the images and rename the copy to `thumb.jpg`. This will
be the thumbnail displayed on the main page.

## How to add a new work (art) category

1) Add a new markdown file in `becky-website/content/work/` named by the
new kind of category you are adding. An example could be `portraits.md`.

2) Edit your new markdown file to add descriptions and/or images. Add
images with the following format:

    `![Portraits](img/work/portraits/image_name.jpg)`

3) Edit the work section description file
(becky-website/data/work.toml). Add a section for your new work section.

    ```
    [[projects]]                                                             
        name = "Portraits"                                                
        folder = "portraits"
    ```

## How to update the website after making changes

1) If you haven't yet, install Hugo

    [Hugo install directions](https://gohugo.io/overview/installing/)

2) Change to the `becky-website` directory

3) Rebuild your website with Hugo

    `> hugo`

4) Add your changed files with git

    Any image files you changed:

    `> git add static/img/work/portraits`

    Any category files you changed:

    `> git add content/work/portraits.md`

    The work description if you changed it:

    `> git add data/work.toml`

    The files containing your rebuilt website:

    `> git add docs/`

5) Commit your changes

    `> git commit`

6) Fill out the commit form (describe what you changed). If you are
using Emacs as your text editor: type in your message, exit with
`ctrl-X`, hit `Y` to say yes to exiting and saving, and finally
finish by pressing `Enter`.

7) Push your changes to both the github repo and the web!

    `git push`

## If you are using Bash on Windows

Bash on Windows doesn't allow you to make new files with Windows in the
directories associated with Bash. To make new files in Windows and then
transfer them to Bash, copy them from Windows to a Bash directory with
Bash. Windows files can be found in Bash within /mnt/c.

## List of things that might be worth changing

1) Each work section as a separate page might ease viewing

2) New "artist" symbols by user image

3) Remove or change icon at top and bottom of page
