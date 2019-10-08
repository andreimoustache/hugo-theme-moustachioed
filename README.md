# hugo-theme-moustachioed

## Homepage

Update your `config.toml` under the root directory as below. Sample config:

```toml
+++
baseURL = "http://example.org/"
languageCode = "en-us"
theme = "moustachioed"

title = "This is some theme."

[params]
fontawesome = "0000000000"
description = "This is moustachioed."
subtitle = "& these are some links"

[[params.links]]
url = "http://google.com"
name = "Google"
fa_logo = "google"

[[params.links]]
url = "http://twitter.com"
name = "Twitter"
fa_logo = "twitter"
```

### Google Analytics & Cookiebot

If you do not want to use Google Analytics and Cookiebot, just ignore this section.

If you do want to use them, just add your IDs under the `params` section of the site config (`config.toml`).

*Note*: GA won't be initialised if the cookie policy is accepted or if the browser set the `DNT` (do not track) header.

```toml
[params]
# rest of the params ...
cookiebotcbid = "xxx"
googleanalyticstrackingid = "xxx"
```

## Posts

`hugo new posts/my-first-post.md`


```toml
+++
title = "My First Post"
description = "Optional description of My First Post. Used for HTML meta tags."
summary = "Optional summary of My First Post"
date = 2019-10-04T15:43:16+07:00
draft = false
pubilshDate = 2019-10-04T15:43:16+07:00
tags = [ "blog" ]
type = "post"
+++
```