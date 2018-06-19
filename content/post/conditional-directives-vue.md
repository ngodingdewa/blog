+++
title = "Conditional Directives v-if, v-else, v-else-if, v-show di vue js"
slug = "conditional-directives-vue"
description = ""
tags = ["javascript","vue"]
date = 2018-06-18T20:21:05+07:00
categories = ["vue"]
draft = false
comments = true
image= "/images/vue/vue.png"
+++

> Kerangka dasar dari front-end adalah ia bisa menampilkan atau menyembunyikan element berdasarkan `kondisi` yang dikehendaki. 

Vue juga memilika arsip directive seperti `v-if`, `v-else`, `v-else-if` dan `v-show`.

Sekarang kita akan mencoba menelaah semuanya.

Setelah memulai [perkenalan vuejs](/post/vuejs) sebelumnya. Sekarang kita tambahkan sedikit propertis nilai sebagai kondisi yang akan mengatur element.

```js
var vue = new Vue({
  el: '#app',
  data: {
    msg: 'Hello Vue!',
    isLogin: false
  }
})
```

## v-if
`v-if` directive bisa mengatur kondisi sesuai yang kita inginkan

...misal kita ingin mengatur sebuah tombol logout tidak ditampilkan kalo kondisi kita tidak login.

Kita bisa menggunakan properti `isLogin` di data model dan menampilkannya di view atau html. 

```html
<button v-if="isLogin">Logout</button>
```

Button tersebut tidak akan muncul karena nilai dari `isLogin` adalah `false`. Sebaliknya jika kita set menjadi `true` dia akan muncul.

`v-if` ini mengatur semua element yang tebungkus didalamnya apakah ingin di proses atau tidak.

```html
<div v-if="isLogin">
  <label>Form Login</label>
  <form>
    <input type="text" name="email">
    <input type="text" name="password">
    <button type="submit">Submit</button>
  </form>
</div>
```

## v-else

`v-else` digunakan jika kita memilika `dua` kondisi yang dikehendaki. Dan ini merupakan kebalikan dari `v-if`. jika kondisi `false`. Element `v-else` lah yang akan di proses/ditampikan.

```html
<button v-if="isLogged"> Logout </button>
<button v-else> Log In </button>
```

Perlu diingat `v-else` tidak memerlukan nilai. Tetatpi ia harus berada/berderetan setelah `v-if` atau `v-else-if` digunakan.

## v-else-if

`v-else-if` digunakan jika kita memiliki kondisi `lebih dari dua` misal 3 atau seterusnya yang ingin diperiksa. Sebagai contoh kita tambahkan properti `isLoginDisabled` dengan nilai `true`

```html
<button v-if="isLogged"> Logout </button>
<label v-else-if="isLoginDisabled"> Register disabled </label>
<button v-else> Log In </button>
```

## v-show
Sama seperti `v-if` bisa menyembunyikan atau menampilkan elment sesuai kondisi.

Perbedaannya

1. `v-if` dieksekusi jika bernilai `true` dan akan dilewatkan jika bernilai `false`.
2. `v-show` ia akan merender semuanya, dan hanya menggunakan css `display:none`.
3. `v-show` tidak bisa digabungkan dengan `v-else` atau `v-else-if`.

Pada dasarnya `v-show` digunakan ketika banyak interaksi seperti `on-off` biar kinerja cepat. Sedangkan `v-if` memiliki keuntungan ketika render awal.


