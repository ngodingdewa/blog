+++
title = "Tutorial laravel untuk pemula"
description = ""
tags = [
    "go",
    "golang",
    "hugo",
    "development",
]
date = "2014-06-02"
categories = [
    "Development",
    "golang",
]
nomenu = "main"
image= "https://d33wubrfki0l68.cloudfront.net/7e6ec3b647e1735c94a1ed519d824a6b5ea618f2/cd1df/img/nodejs/npm/npm.png"
+++

## Tutorial laravel untuk pemula vol.1

Zombie ipsum reversus ab viral inferno, nam rick grimes malum cerebro. De carne lumbering animata corpora quaeritis. Summus brains sit​​, morbo vel maleficia? De apocalypsi gorger omero undead survivor dictum mauris. Hi mindless mortuis soulless creaturas, imo evil stalking monstra adventus resi dentevil vultus comedat cerebella viventium. Qui animated corpse, cricket bat max brucks terribilem incessu zomby. The voodoo sacerdos flesh eater, suscitat mortuos comedere carnem virus. Zonbi tattered for solum oculi eorum defunctis go lum cerebro. Nescio brains an Undead zombies. Sicut malus putrid voodoo horror. Nigh tofth eliv ingdead.

```CSS
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

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3


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