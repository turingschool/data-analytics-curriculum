# Turing School Data Analytics Curriculum

This site is built with Jekyll. Find the docs [here](https://jekyllrb.com/docs/usage/)

## Contributing

* Clone the repo `git clone git@Github.com:turingschool/data-analytics-curriculum.git`
* run `bundle install`
* You can now begin to edit the website.
* To start the server run `jekyll serve --incremental`.
* Navigate to `localhost:4000` to see the site

* make changes on the `gh-pages` branch.
* you can push changes to production by pushing the `gh-pages` branch to Github. `git push origin gh-pages`.
* The changes may take a minute or two to be recognized on production. Please make sure you review your changes on production.

## Site Structure

You will find a module specific directory. eg `module1` and within each directory you will find a directory for `lessons` and `projects`. All files within this site can be written as either markdown or html. To link to each you just need to write the relative path to each file without the file extension. For example `lessons/lesson_on_stuff`.

The `navigation.html` file is where you will find the sidebar for the site.

The `today.html` file is where you will find the basic html page for today, and each file for the specific day will live within the `today` directory.

## Creating Content

### File Headers

Put something like this at the top of all your markdown files:

```yaml
---
title: Name of lesson
subheading: lesson is about stuff
layout: page
---
```

- `subheading` is optional
- `layout` is basically always going to be `page`

### Index.md instead of Readme.md

The system we're using to translate from Github to [data.turing.io](https://data.turing.io) uses index files instead of readme files. Where you would have created a file called `readme.md`, just use `index.md` instead.

### Links and Paths

When linking to a markdown file, drop the `.md` in your link. Instead of linking to `learning_to_pair.md`, just use `learning_to_pair`. Other files, such as PDFs and PNGs, keep the original extension.

#### Absolute vs Relative paths

Since you're editing on Github, and viewing at [data.turing.io](https://data.turing.io), use *relative* links instead of *absolute* links. You can learn more about their differences [here](http://www.boogiejack.com/server_paths.html).

### Github Markdown

Github uses a different system for translating Markdown than the engine we use for [data.turing.io](https://data.turing.io). Here are some things that you'll need to change get the correct formatting, even if it looks right on Github.

- Put a space after your `#`'s in headers
- Put a blank line between your headers and any content below
- Replace any `|` with `\|` unless you're really trying to do a table

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.