# bec4.github.io

The [BEC4 website](https://bec4.mit.edu) is hosted through GitHub pages which forwards it to the MIT subdomain. This means that all the relevant files are contained in this repository, and that GitHub converts them into static files which it hosts. For this, it uses a static site generator called [Jekyll](https://jekyllrb.com), which is a program that converts markdown files into styled HTML files according to some style definition. It's fairly easy to make small edits to this: clone the repository, make your changes, and push the result. It's a bit more complicated if you want to *see* the results of your work before pushing it to the public repository. For that you need to install Jekyll locally -- see the instructions below.

## Files and structure
Every page is a markdown file in the root of the repo. Only edit those if you want to change the contents of the website. Some of them contain some Javascript for some of the visualizations, all of that code and other requirements are in the `/assets` folder.

### Changing layout
If you want to change some of the structure of the HTML files you need to go into the `/_layouts` folder. This contains HTML templates with special tags that are to be filled in by Jekyll.

### Changing styles
If you want to change the style you need to edit `/assets/styles.scss`, this is a style sheet that overrides the theme defaults. The rules that are configured here are used by Jekyll to generate the full set of style sheets for the final website.

## Running Jekyll locally
Setting Jekyll up locally is mildly annoying because it requires a Ruby installation. It's easiest to do this on a Mac or Linux machine, although there are [installation instructions](https://jekyllrb.com/docs/installation/) for Windows, too.

Once you've made it that far, though, running a local server with the website is easy. Just `cd` into the repo directory and do
```
bundle exec jekyll serve --livereload
```
This will run the website on `localhost:4000`. The `--livereload` option automatically reloads the web page when you change one of the files. Optionally, if you'd like to test it on another device, you can add the option `--host=0.0.0.0`, then any device with network access to you machine can load the website, which is useful if you want to test something on your phone, for instance. 

## Linking to the MIT subdomain
Connecting to MIT's subdomain requires the CNAME file that's in the repository. On MIT's side, IS&T created a CNAME record that points to [bec4.github.io](bec4.github.io), which is really all there is. 
