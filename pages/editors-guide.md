---
title: "Editors Guide"

search_exclude: true
---

## Formatting

The main content uses Markdown, and here is a [Basic Syntax Guide](https://www.markdownguide.org/basic-syntax)

## Navigation Menu

The side bar navigation menu is determined by a data definition, found at [_data/sidebars/main.yml](https://github.com/FAIRDOM/fairdom.github.io/blob/master/_data/sidebars/main.yml)

## Pages

General pages should be placed in the _"pages/"_ folder, and by default will adopt the _page_ layout.

The layout can be overridden with another layout if defined in the _front-matter_ (the bit at the top between `---`).

The front-matter for Pages should look like:

```
---
title: This is the title
---
```

e.g: - [pages/about/about.md](https://raw.githubusercontent.com/FAIRDOM/fairdom.github.io/master/pages/about/about.md)

**Note** that the subfolder of the pages (in this case _/about/_) is discarded when created the url, so in this case points directly at [https://fair-dom.org/about](https://fair-dom.org/about)

When editing a page, take a note of and don't change any _redirect_from_ definitions in the front-matter. 
These define a redirection from a page that existed on the old site, that is linked to from another website.

## News

News items should be placed in the _"_news/"_ folder, with the filename prefixed with the date stamp, following [ISO 8601 Calendar Date](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) - **YYYY-MM-DD** .
This defines the date for the news item, and also helps keep the files in order.

News will automatically adopt the _news_ layout unless overridden.

You can optionally set the _date_ in the front-matter to override the date specified by the filename - useful if correcting a date in the future
without breaking the URL.

If you wish to provide an image then set the _image_ to the relative path of the image file.

The front-matter for News could look like

```
---
title: This is the news
date: 2020-02-16
image: "/images/news/elixir-logo.png"
---
```
An example is [_news/2018-03-28-carole-goble-presents-at-digitallife-2018.md](https://raw.githubusercontent.com/FAIRdom/fairdom.github.io/master/_news/2018-03-28-carole-goble-presents-at-digitallife-2018.md)
## Events

ews items should be placed in the _"_events/"_ folder, with the filename prefixed with the date stamp, following [ISO 8601 Calendar Date](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) - **YYYY-MM-DD** .
This defines the post date for the event item, and also helps keep the files in order.

The event front-matter is a bit more complicated and looks like:

```
---
title: FAIRDOM PALs User Meeting 2019
start_date: 2019-07-18
end_date: 2019-07-19
location: HITs
location_url: https://www.h-its.org/institute/
date: 2019-02-24
---
```
The _title_ and _start_date_ are mandatory, and both the start and end date should follow the YYYY-MM-DD format.
The _end_date_ is optional and if missing would indicate a 1 day event.

If you wish to specify a specific start time, you can put this in the body of the Event description.


The _location_ is optional, and if you wish to provide a URL for the location (also optional), you can specify the _location_url_

Like with _news_ - the _date_ is optional and overrides the post date defined by the file prefix.

An example is [/_events/2019-05-26-fairdom-pals-user-meeting-2019.md](https://raw.githubusercontent.com/FAIRdom/fairdom.github.io/master/_events/2019-05-26-fairdom-pals-user-meeting-2019.md)
