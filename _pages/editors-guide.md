---
title: "Editors Guide"
---

## Formatting

The main content uses Markdown, and here is a [Basic Syntax Guide](https://www.markdownguide.org/basic-syntax)

## Navigation Menu

The top level menu is determined by a data definition, found at [https://github.com/FAIRdom/fairdom.github.io/blob/master/_data/navigation.yml](https://github.com/FAIRdom/fairdom.github.io/blob/master/_data/navigation.yml)

## Pages

General pages should be placed in the _"_pages/"_ folder, and by default will adopt the _page_ layout.
The layout can be overridden with another layout if defined in the front-matter (the bit at the top between ---).

The front-matter for Pages should look like:

```
---
title: This is the title
---
```


e.g: - [https://raw.githubusercontent.com/FAIRdom/fairdom.github.io/master/_pages/about.md](https://raw.githubusercontent.com/FAIRdom/fairdom.github.io/master/_pages/about.md)

## News

News items should be placed in the _"news/"_ folder, with the filename prefixed with the date stamp, following [ISO 8601 Calendar Date](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) - **YYYY-MM-DD** .
This defines the date for the news item, and also helps keep the files in order.

News will automatically adopt the _news_ layout unless overridden.

You can optionally set the _date_ in the front-matter to override the date specified by the filename - useful if correcting a date in the future
without breaking the URL.

The front-matter for News could look like

```
---
title: This is the news
date: 2020-02-16
---
```

## Events

ews items should be placed in the _"events/"_ folder, with the filename prefixed with the date stamp, following [ISO 8601 Calendar Date](https://en.wikipedia.org/wiki/ISO_8601#Calendar_dates) - **YYYY-MM-DD** .
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


