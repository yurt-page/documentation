## Blog
See [yurt-blog](https://github.com/yurt-page/yurt-blog) engine and [project ideas])https://github.com/orgs/yurt-page/projects/3).

Key features and ideas:
* RSS must be supported. Only it gives real freedom for readers. In fact only RSS will be enough to make life better for most peoples.
* The blog itself may be just an online RSS reader. I.e. you can read your own blog the same as any other.
* Multiple authors aren't necessary. We may have a very simple access list model.
* Friendly SEO is very wanted but not so important than everything else. I.e. not generate of pure HTML to be indexed. We may instead create some aggregator/proxy or maje our own "blog search" as Yandex.Blogs.
* Comments must be developed even better than posts: discussions are the main focus. Comments on habr.com are much valuable than post.
* But for some posts comments may be just disabled like in Telegram Channels. Such posts must have a different type like Note.
* So we must support different types of posts: articles (translatable and searchable), notes (not searchable), gists (not published in feed but searchable) etc.
* Stats must be as good as possible (countries, unique readers, read time etc.) but in the same time we must value users privacy (do not use or leak third party data). Otherwise, users may start to use Google Analytics or other even worst spying systems. But some websites like e-commerce for marketing still needs more stats. We are fine to create own tracking system (at least we are not evil yet).
* Cross posting is very important. We must allow publishing to Twitter, FB, anything else.
* We must also be friendly for cross posting and support OData.
* Subscribe via email will be very nice. XMPP/Web/Telegram push.
* To minimize space and optimize speed we may store posts directly in RSS but each post separately. We are free to extend RSS with our elements like comments.
* Support for git/markdown static generators. We may create a plugin for Jekyl/Hugo.
* Maybe we can add a versioning and send only diffs on editing.
* Very basic WYSIWYG editor and use Markdown. But on saving convert MD to HTML/RSS.
* For an API we may try to use AtomPub or even use raw WebDAV PUT.
* We must gzip post content on client before sending. Thus, we'll save resources on router.
* Spam Protection is the hardest thing to do. PoW Captcha may help https://git.sequentialread.com/forest/pow-captcha. Maybe reuse the Hashcash for email



### Another interesting solutions
Basically any static site generator may be used like [Hugo](https://gohugo.io/) and [it's alternatives](https://www.google.com/search?q=hugo+alternatives).
But they all are written in Go/Ruby/PHP and it's hard to put them on a router.
Hugo in Go, [Grav CMS](https://learn.getgrav.org/17/basics/what-is-grav): in PHP, 
[Ghost](https://github.com/TryGhost/Ghost) and 
[11ty](https://github.com/11ty/eleventy/) in NodeJS.
The https://www.htmly.com/ in PHP

Shell script based site generators:
* Luke Smith blog scripts https://github.com/LukeSmithxyz/lb
* suckless.org static generator https://git.codemadness.org/saait/file/README.html
* https://codeberg.org/vimuser/untitled uses pandoc templates. Used by libreboot.org
* https://blot.im/ allows to create a blog from DropBox. Sources https://github.com/davidmerfield/blot
* https://turtlapp.com/  collaborative notebook

WebDAV based blog engines:
* https://github.com/katomaso/webdave


* [indieforums](https://www.indieforums.net/threads/024f3f45f725dba0.html)
* https://searchmysite.net/ search by indie blogs
