# Angular Rust

<img align="right" width="150" height="150" src="/content/ruex.svg">

**Angular Rust** is an intuitive, elegant, and responsive Zola theme for product sites.

- Build for product sites
- Simple and intuitive structure
- Clean and elegant design 
- Responsive and mobile device compatible
- Customize and extend friendly

https://angular-rust.github.io

# Installation

First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/angular-rust/ruex.git
```

or add as a submodule
```bash
$ git submodule add https://github.com/angular-rust/ruex  themes/ruex
```

and then enable it in your `config.toml`:

```toml
theme = "ruex"
```

# Structure

### Hero

**Angular Rust** is designed for product websites, hence we let **hero** part fills whole of screen.
You can customize your **hero** by using `hero` block in the `index.html`.


### Page

Every markdown file located in `content` directory will become a **Page**. There also will display as
a navigate link on the top-right corner. 
You can change the frontmatter's `weight` value to sort the order (ascending order).

```
+++
title = "Changelog"
description = "Changelog"
weight = 2
+++

```

### CSS variables

You can override theme variable by creating a file named `_variables.html` in your `templates` directory.

```html
<style>
    :root {
        /* Primary theme color */
        --primary-color: #FED43F;
        /* Primary theme text color */
        --primary-text-color: #543631;
        /* Primary theme link color */
        --primary-link-color: #F9BB2D;
        /* Secondary color: the background body color */
        --secondary-color: #fcfaf6;
        --secondary-text-color: #303030;
        /* Highlight text color of table of content */
        --toc-highlight-text-color: #d46e13;
    }
</style>
```

# Configuration

You can customize some builtin property in `config.toml` file:

```toml
[extra]
logo_name = "Angular Rust"
logo_path = "ruex.svg"
extra_menu = [
    { title = "Github", link = "https://github.com/angular-rust/ruex"}
]
```
## Theme 

Primary #409EFF
Success #67C23A
Warning #E6A23C
Danger #F56C6C
Info #909399
Primary Text #303133
Regular Text #606266
Secondary Text #909399
Placeholder #C0C4CC
Border Base #DCDFE6
Border Light #E4E7ED
Border Lighter #EBEEF5
Border Extralight #F2F6FC
Background B #000000
Background W #FFFFFF
Background Transparent

#17212F
#152030
#0D1520
#2A4058
#12202F
#168AFD
#E55074
#1581EE
#16ADCA
#FFFFFF
#0C6291
#4D87F2
#4D87F1
#0C6291

#121A26
#40C4FF
#1C2834

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300&display=swap');

## Page front-matter
```
title = ""
description = ""
date =
weight = 0
draft = false
slug = ""
path = ""
aliases = []
in_search_index = true
template = "page.html"

[taxonomies]
tags = ["rust", "web"]

[extra]
```

## Section front-matter
```
title = ""
description = ""
sort_by = "none"
weight = 0
template = "section.html"
page_template =
paginate_by = 0
paginate_path = "page"
insert_anchor_links = "none"
in_search_index = true
render = true
redirect_to = ""
transparent = false
aliases = []

[extra]
```

# Showcases

Please see the [showcases page](/showcases).

# Contributing

Thank you very much for considering contributing to this project!

We appreciate any form of contribution:

- New issues (feature requests, bug reports, questions, ideas, ...)
- Pull requests (documentation improvements, code improvements, new features, ...)