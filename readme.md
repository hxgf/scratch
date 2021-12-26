# 𓂀

blank slate to make it a little easier to start building a static web site for apache ... from scratch

---

## WHAT'S INCLUDED?

- [index.html](https://github.com/hxgf/scratch/blob/master/index.html) - boilerplate page with necessary meta tags and all the libraries already linked

- [.htaccess "router"](https://github.com/hxgf/scratch/blob/master/.htaccess) - pretty urls, force https, gzip static assets (if available)

- [images/blank.gif](https://github.com/hxgf/scratch/blob/master/images/blank.gif) - 1x1 transparent .gif

### plus your choice of utility libraries:
- [tachyons CSS (4.12.0)](https://tachyons.io/) (default)
- [tailwind JIT via CDN](https://tailwindcss.com/) (alt)

- [jquery (3.6.0)](https://jquery.com/) (default)
- [alpine.js (2.5.0)](https://github.com/alpinejs/alpine) (alt)

- [instant.page (5.1.0)](https://instant.page/) (default)
- [turbo (latest) via CDN](https://turbo.hotwired.dev/) (alt)

---

## ALPINE BOILERPLATE EXAMPLE
- vertically centered text
- alpine.js x-data function block 
- pop-up rain spell

```
<body class="h-100 sans-serif">

  <div class="dt h-100 mw7 center" x-data="welcome()">
    <div class="dtc v-mid pink tc lh-copy">
      <div class="f-subheadline mb2 pointer" @click="rain_spell()">☼ &nbsp; ❀ &nbsp; ♡</div>
      <div class="f2">Light, Life and Love are like three glow-worms at thy feet: the whole universe of stars, the dewdrops on the grass
      whereon thou walkest!</div>
    </div>
  </div>

  <script>
    function welcome() {
      return {
        rain_spell: function () {
          alert('o Gabriel fac pluat. o poseidon, ut pluvia. ne pluat o Neptune beatitudinis. o deus, nam ego filius tuus fac pluvia. Sic fiat semper.')
        }
      }
    }
  </script>

</body>
```

---

## LICENSE
Copyright © [HXGF](https://hxgf.io). This project is MIT licensed.