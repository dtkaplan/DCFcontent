---
layout: page
tagline: Materials and Content for DCF
title: Instructor site
---
{% include JB/setup %}

## To-Do List

1. Move this site to a new directory and connect to Github.  Deploy in
   gh-pages.
2. Get Discus ID and set up comments.
3. Look for a better theme.

## How to Modify Content

1. Edit or create the appropriate files.
2. Run `jekyll build --destination "~/Dropbox/Public/DCFcontent"`
2. Run `jekyll serve` and go to <http://0.0.0.0:4000/>.

## How to Modify the Form

* See <http://jekyllbootstrap.com/usage/jekyll-quick-start.html>.
* Some themes <http://jekyllthemes.org/>
* Once a theme is installed, run this, replacing `twitter` with the
    theme you want from the assets/themes directory.
	
        rake theme:switch name="twitter"
        jekyll build

## And now back to the original

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

## Update Author Attributes

In `_config.yml` remember to specify your own data:
    
    title : My Blog =)
    
    author :
      name : Name Lastname
      email : blah@email.test
      github : username
      twitter : username

The theme should reference these variables whenever needed.
    
## Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

    $ rm -rf _posts/core-samples

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

This theme is still unfinished. If you'd like to be added as a contributor, [please fork](http://github.com/plusjade/jekyll-bootstrap)!
We need to clean up the themes, make theme usage guides with theme-specific markup examples.


