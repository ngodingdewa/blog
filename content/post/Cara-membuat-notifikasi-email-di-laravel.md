+++
title = "Cara Membuat Notifikasi Email Di Laravel"
description = ""
tags = ["laravel"]
date = 2018-06-17T16:05:02+07:00
categories = []
image= "https://d33wubrfki0l68.cloudfront.net/df196ebffb1eed612dd88947c0a7a8f74dd2c242/8a492/img/telegram/embed/embed.png"
comments = true
+++

## Tutorial laravel untuk pemula vol.1

Themes can enhance the Vue app that VuePress uses by exposing an `enhanceApp.js` file at the root of the theme. The file should `export default` a hook function which will receive an object containing some app level values. You can use this hook to install additional Vue plugins, register global components, or add additional router hooks:

Zombie ipsum reversus ab viral inferno, nam rick grimes malum cerebro. De carne lumbering animata corpora quaeritis. Summus brains sit​​, morbo vel maleficia? De apocalypsi gorger omero undead survivor dictum mauris. Hi mindless mortuis soulless creaturas, imo evil stalking monstra adventus resi dentevil vultus comedat cerebella viventium. Qui animated corpse, cricket bat max brucks terribilem incessu zomby. The voodoo sacerdos flesh eater, suscitat mortuos comedere carnem virus. Zonbi tattered for solum oculi eorum defunctis go lum cerebro. [`_site` mapped to a git submodule on the `gh-pages` branch](http://blog.blindgaenger.net/generate_github_pages_in_a_submodule.html) Nescio brains an Undead zombies. Sicut malus putrid voodoo horror. Nigh tofth eliv ingdead.


```bash
# install globally
yarn global add vuepress # OR npm install -g vuepress

# create a markdown file
echo '# Hello VuePress' > README.md

# start writing
vuepress dev

# build
vuepress build
```

```js{4}
import Vue from 'vue';
import App from './App.vue';

// Receives the context of the render call, returning a Promise resolution to the root Vue instance.
export default context => {
  return Promise.resolve(
    new Vue({
      render: h => h(App)
    })
  );
}
```
<iframe width="700" height="400" src="https://www.youtube.com/embed/RdmkEF161aU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

```json
{
  "title": "VuePress",
  "description": "Vue-powered Static Site Generator",
  "base": "/",
  "pages": [
    {
      "lastUpdated": 1524027677000,
      "path": "/",
      "title": "VuePress",
      "frontmatter": {}
    },
    ...
  ]
}
```

```css
.container{
  background-color: red;
  padding: 20px;
  font-size:10px;
}
```

```html
<html>
  <head>
    <title>Testing</title>
  </head>
  <body>
    <div class="container">
      <div style="color:red"></div>
    </div>
  </body>
</html>
```

```javascript
<script>
export default {
  mounted () {
    import('./lib-that-access-window-on-import').then(module => {
      // use code
    })
  }
}
</script>
```

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```

```json
{
  "path": "/using-vue.html",
  "title": "Using Vue in Markdown",
  "frontmatter": {}
}
```

```cs
$ rm -rf public
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 found taxonomies: map[string]string{"tag":"tags", "category":"categories"}
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content 
0 future content 
2 pages created 
0 tags created
0 categories created
in 4 ms
$ find public -type f -name '*.html' | xargs ls -l 
-rw-r--r--  1 quoha  staff  94 Sep 29 22:23 public/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/first/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/second/index.html
$ cat public/index.html 
<!DOCTYPE html>
<html>
<body>
  
    <h1>second</h1>
  
    <h1>first</h1>
  
</body>
</html>
$
```

```xhtml
<!DOCTYPE html>
<html>
<body>
  {{ range first 10 .Data.Pages }}
    <h1><a href="{{ .Permalink }}">{{ .Title }}</a></h1>
  {{ end }}
</body>
</html>
```