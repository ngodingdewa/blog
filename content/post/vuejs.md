+++
title = "Pengenalan awal Vue.js"
slug = "vuejs"
description = "Belajar vue.js"
tags = ["javascript","vue"]
date = 2018-06-18T16:22:40+07:00
categories = ["vue"]
draft = false
comments = true
image= "/images/vue/vue.png"
+++


Saat ini vue sangan populer dikalangan front-end. Dengan kemudahan dan kecanggihannya vue menjadi pilihan sebagai framework javascript yang wajib masuk kedalam list yang patut dipelajari selain react.

Untuk awal perkenalan dengan vue, disarankan untuk mengetahui terlebih dahulu dasar-dasar HTML, CSS dan javascript agar memudahkan kedepannya..

Cara yang mudah untuk mencoba vue, bisa pergi ke [jsfiddle.net](https://jsfiddle.net/chrisvfritz/50wL7mdz/). Atau buat file `index.html` dan iclude vue dibawah ini didalam tag `<head>`:

```html
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
```

Sebenernya ada cara untuk menginstall vue pake `vue-cli`, tetapi harus familiar dengan node js.

...setelah itu buat tag `div` dan beri id dengan nama `app` didalam tag `body`. Id `app` lah yang nantinya tempat aplikasi vue. 

```html
<div id="app">
  <h1>{{ msg }}</h1>
</div>
```

`msg` disini merefresentasikan data, yang akan kita kirim dari script vue.

Sekarang kita bikin script vue

```js
var vue = new Vue({
  el: '#app',
  data: {
    msg: 'Hello Vue!'
  }
})
```

variable `vue` akan menampung data `msg` dan akan dimasukan kedalam el/element id `app`. 

Kode utuhnya menjadi

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Hello World in Vue.js</title>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
  </head>
  <body>
    <div id="app">
      <h1>{{ msg }}</h1>
    </div>
    <script>
      var vue = new Vue({
        el: '#app',
        data: {
          msg: 'Belajar vuejs bersama ngodingdewa!'
        }
      });
    </script>
  </body>
</html>
```

![alt text](/images/vue/hello-world.PNG "vue hello world")

Itulah pengenalan awal tentan vue js. Kedepannya masih banyak hal-hal yang akan dipelajari.



