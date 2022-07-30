---
layout: post
category: Log
---
## Head to Github blog now!

Recently I migrated from my wordpress blog (quite outdated though :wink:) to Jekyll. This is simple, minimal static
site generator.

Just listing out the quick procedure:

* Export the wordpress contents.

* Convert the wordpress dumped xml to markdown.

* Set up Jekyll in your system. Or fork **barryclark/jekyll-now** for easy set-up: in that repo the procedure to get your username.github.io is given.

* Spent some time to arrange your old posts in new environment.

Hurray, Your blog is up!

Wait, Do you want to create different categories of post? Then read some more :smirk:
I spent some amount of time to get these things done.

If your posts are coming from different categories, for eg., technical and non-technical contents. Instead of 
            
            --_posts
              |
              --post1.md
              --post2.md
            
you can make this structure
            
            --technical
              |
              --index.html
              --atom.xml
              --_posts
                |
                --text1.md
                --text2.md
              
            --non-technical
              |
              --index.html
              --atom.xml
              --_posts
                |
                --text1.md
                --text2.md

Please make sure to specify the tags/categories in metadata of the post.
```
 ---
 layout: post
 category: technical
 ---

```
Feel free to refer atom feed and index sample here : https://github.com/rosnikv/rosnikv.github.io/tree/master/wp-log
###### _Happy Blogging_ :thumbsup:

Reference : https://www.garron.me/en/blog/multi-blog-site-jekyll.html

P.S : post name should be of format "year-month-data-title.md"
