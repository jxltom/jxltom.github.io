An enhanced [scribble](https://github.com/muan/scribble) Jekyll theme. [https://jxltom.github.io/scribble-enhanced/](https://jxltom.github.io/scribble-enhanced/).

## Overview

- Features

    - Customized page width

    - Enable/disable comments for each post

    - RSS feed and Sitemap using official Jekyll sitemap gem and feed gem

- Intergrations

    - [Disqus](https://disqus.com/)

    - [duoshuo](http://duoshuo.com/)

    - Google Analytics

## Usage

- Getting started

    - [Fork the repository](https://github.com/jxltom/scribble-enhanced/fork).

    - Change repository name to ```yourgithubusername.github.io```.

    - Set ```master``` branch as source of GitHub Pages. Then your website will be ```Http://yourgithubusername.github.io```.

- Configuration

    - Basic configuration of ```_config.yml```.

        - ```title```. Title of your site which will display in the header.

        - ```description```. Short bio or description which will display in the header.

        - ```url```. Your website URL (e.g. ```http://jxltom.github.io``` or http```://blog.jxltom.me```). Used for sitemap.xml and your RSS feed. If you're hosting your site at a Project repository, the url still should be ```http://yourusername.github.io```

        - ```baseurl```. If you're hosting your site at a Project repository on GitHub pages (```http://yourusername.github.io/repository-name```) and NOT your User repository (```http://yourusername.github.io```) then add in the baseurl here, like this: ```/repository-name```.

    - Optional configuration of ```_config.yml```.

        - ```signoff```. Your name for signoff. Leave empty for no name signoff.

        - ```disqus``` or ```duoshuo```. Enter your ```Disqus``` shortname (not your username) or your ```duoshuo``` ID to enable commenting on posts. You can find your shortname on the Settings page of your Disqus account. You can only set one between ```disqus``` and ```duoshuo```.

        - ```google_analytics```. Enter your Google Analytics web tracking code (e.g. ```UA-2110908-2```) to activate tracking.

        - ```links```. A list of links which will show as navigation bar.

    - Custom ```about``` page. Update content or delete ```about.md``` for costom ```about``` page.

    - Domain. For custom domain settings, set ```CNAME``` to your domain.

- Blogging

    - Push new post with name as ```YYYY-MM-DD-post-name.md``` in ```_posts``` folder.

    - Options of a post. You can add options in metadata of a post header.

        - ```comment: y```. If ```comment``` is set to ```y```, at the end of the post there will be a ```Disqus``` or ```duoshuo``` thread. To enable comments, you also need to provide ```disqus``` or ```duoshuo``` in ```_config.yml```.

        - ```share: y```. An option for showing tweet and like button under a post.

    - GFM

        - Start header from ```##``` in your post since title of post will be considered as ```#```.

        - Hard line breaks in paragraphs are enforced by default in GFM parser of kramdown, which is the only parser of markdown in GitHub.

        - Note that following features of GFM are not supported since kramdown GFM parser, which is the only Github mardown parser, doesn't support them currently.

            - Emoji

            - Check box

## Development

Note that there are currently two branches. **All development should be pushed to ```master```**. Branch ```gh-pages``` is only for demo.

- Custom page width

    - Change ```max-width``` of ```footer``` and ```#container```.

    - Change ```margin-left``` of ```.paging .right``` to half width of desired width plus ```20px```.

    - Change ```margin-right``` of ```.paging .left``` to half width of desired width plus ```40px```.

### TODO

- SEO optimization

- Better share function

- CNZZ integration

- Tags support

### References

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown)
- [GFM mode does not support check boxes](https://github.com/gettalong/kramdown/issues/346)
- [Feature Requests](https://github.com/gettalong/kramdown/projects/1)
- [GFM input for Kramdown not working](https://github.com/jekyll/jekyll/issues/4529)
- [kramdown Parser](https://kramdown.gettalong.org/parser/kramdown.html)
- [GFM Parser](https://kramdown.gettalong.org/parser/gfm.html)
- [The Open Graph protocol](http://ogp.me/)
- [truncatewords is unsafe](https://github.com/barryclark/jekyll-now/issues/117)
- [Do not include 404 page in sitemap.xml](https://github.com/barryclark/jekyll-now/pull/356)
- [Adding permalink to 404.html](https://github.com/muan/scribble/pull/42)
- [Creating a custom 404 page for your GitHub Pages site](https://help.github.com/articles/creating-a-custom-404-page-for-your-github-pages-site/)
- [Update 404 for new Jekyll 3](https://github.com/barryclark/jekyll-now/pull/404)