---
layout: page
title: Tools
permalink: /tools/
---

Links for tools and software info ideas

Jump to : [intalling jekyll](#jekyll)

### Transcription
I came across [this article](https://medium.com/@valdolyon/google-speech-to-text-work-on-your-timestamps-78abf7805fe2) which turned me on to CMUSphinx for transcription purposes. I cannot access Google Cloud API because they don't accept "prepaid" cards (lol) even when those prepaid cards are linked to bank accounts. So I am working with [CMUSphinx](CMUsphinx.github.io/) in the mean-time and who knows... maybe I'll just make *my own cloud api* :stuck_out_tongue:

### Installing Jekyll
{: #jekyyl}
I installed jekyll so I can view and develop the 'site' locally and then publish when necessay using git. I followed information on these pages to build this site, note that the macOS instructions require homebrew be installed:

- Installing jekyll [offical jekyll docs](https://jekyllrb.com/docs/installation/macos/)
- Edit Gemfile as follows
```
# gem "jekyll", "~> 4.1.1" <--commented out this line
# This is the default theme for new Jekyll sites. You may change this to anything you like.
gem "minima", "~> 2.5"
# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
 gem "github-pages", group: :jekyll_plugins <-- uncommented this line
```
- I also edited the _config.yml file as per [these instructions](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_publishing_github_pages.html)
```
baseurl: "/open-courses" # the subpath of your site, e.g. /blog
url: "val-storm.github.io" 
```
- When pushed to github all the links worked and I didn't have to do aynthing special
- [This video](https://youtu.be/SWVjQsvQocA) was a bit slow, but very helpful to get going