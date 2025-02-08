![Argon](https://cdn.jsdelivr.net/gh/solstice23/cdn@master/argon_new_animate.svg)

# Hexo-Theme-Argon

Hexo port of the [Argon-Theme](https://github.com/solstice23/argon-theme)

# About

Hexo-Theme-Argon is ported from the WordPress version of the Argon theme.

## Project Status

Currently, there is no energy to maintain the ported version, only the WordPress version is maintained. New features in WordPress will not come to the Hexo version, only necessary bug fixes will be made. ~~(Haven't used Hexo for a long time)~~

Feel free to submit Pull Requests to contribute/port new features/fix bugs.

# Usage

## 1. Install and enable the theme

1. Clone this repo in the `Hexo root directory/themes` directory.

```
git clone https://github.com/solstice23/hexo-theme-argon.git
```
Install the ejs renderer.

```
npm install hexo-renderer-ejs
```

2. Rename the cloned folder to `argon`

3. Change the `theme` item to `argon` in `Hexo root directory/_config.yml`

## 2. Modify theme configuration

1. Copy `Hexo root directory/themes/argon/_config.yml` to `Hexo root directory/source/_data` folder and rename it to `argon.yml`

2. Modify the copied configuration file

## 3. Configure search functionality

1. Execute in the `Hexo root directory/themes` directory

```
npm install hexo-generator-search --save
```

2. Add options in `Hexo root directory/_config.yml`

```
search:
  path: search.xml
  field: post
  content: true
```

# Update

Execute in the `Hexo root directory/themes/argon` directory

```
git pull
```

# Post Parameters

Argon supports setting some individual parameters for posts, such as post thumbnails

| Parameter Name            | Description                          |
|---------------------------|--------------------------------------|
| thumbnail                 | Post thumbnail URL                   |
| first_image_as_thumbnail  | Use the first image in the post as the thumbnail |
| after_post                | Additional content after the post    |
| excerpt                   | Custom excerpt for the post          |

# Hexo version compared to WordPress version

+ Retains most features of the WordPress version
+ Same interface
+ Does not support multiple languages for now (PRs welcome)
+ Currently only supports Gitalk, giscus, waline comment systems (PRs welcome)

# Telegram Channel
[t.me/argontheme](https://t.me/argontheme)

Automatically push update messages and other news about Argon

> Readme to be improved...

# Changelog

## 20201031 v1.0.2
+ Added Busuanzi for counting visits and post views
+ Fixed Page generation issue again
+ Changed highlight color to red
+ Fixed Gitalk comments not loading issue
+ Fixed issue with post directory not supporting numbers + titles

## 20200908 v1.0.1
+ Fixed issue where clicking search results would not close the search
+ Fixed duplicate search button issue on mobile
+ Fixed Page generation issue

## 20200905 v1.0.0
+ Added custom excerpts for posts
+ Supported More tag
+ Fixed Gitalk margin issue

## 20200822 v1.0.0.beta
+ Initial version
