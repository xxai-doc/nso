<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Ho kgothaletswa ho kenya nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) pele, 'me joale `direnv allow` ka mor'a ho kena directory ( [le .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) tla bolaoa ka tsela e iketsang ka mor'a ho kena directory).

Moelelo ke: Phetolelo ya Setšhaena go Sejapane, Sekorea, Seisemane, Phetolelo ya Seisemane go maleme a mangwe ka moka. Ge o nyaka go thekga Setšhaena le Seisemane fela, o ka no ngwala `zh: en` .

Moelelo ke: Phetolelo ya Setšhaena go Sejapane, Sekorea, Seisemane, Phetolelo ya Seisemane go maleme a mangwe ka moka. Ge o nyaka go thekga Setšhaena le Seisemane fela, o ka no ngwala `zh: en` .

* [khoutu ya pele-qetellong](https://github.com/xxai-art/web)
* [Diphuthelwana tša polelo tša sebaka ka kakaretšo](https://github.com/xxai-art/web/tree/main/i18n)
* [Diphuthelwana tša polelo tša dimmojule tša go tsena](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Webosaete Ditokomane tša Maleme a Mantši](https://github.com/xxai-doc)

Polelo ya mananeo a ka pele ke [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , yeo e oketšago dikarolo tše dingwe tše di theilwego godimo ga polelo ya go ngwala ya coffeescript, bona [./coffee_plus.md](./coffee_plus.md) .

## Internationalization ya diwepesaete le ditokomane

Aga godimo ga diprotšeke tše 3 tše di latelago

* [@ w5 / mdt](https://www.npmjs.com/package/@w5/mdt)

  Moselana ke `.mdt` , o ka šomiša polelo ya go swana le `<+ ./coffee_plus/import.js>` go šupa difaele tša ka ntle, gomme wa tšweletša markdown ka moselana `.md` .

* [@ w5 / trmd](https://www.npmjs.com/package/@w5/trmd)

  Phetolelo ya Markdown e ka se fetolele dikhoutu le dikgokagano, gomme e tla boloka dipolelo tše di fetoletšwego. Ge phetolelo e fetotšwe eupša mongwalo wa mathomo ga se wa fetošwa, go e phethagatša gape go ka se ngwale godimo ga phetošo ya phetolelo.

* [@ w 5 / i 18n](https://www.npmjs.com/package/@w5/i18n)

  Difaele tša polelo tša go fetolela diwepesaete tšeo di tšweleditšwego ke `yaml` .

### Ditaelo tša go Itiriša tša Phetolelo ya Tokomane

Bona polokelo ya khoutu [xxai-art/doc](https://github.com/xxai-art/doc)

Ho kgothaletswa ho kenya nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) pele, 'me joale `direnv allow` ka mor'a ho kena directory ( [le .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) tla bolaoa ka tsela e iketsang ka mor'a ho kena directory).

E le gore ke pheme motheo o mogolo wa khoutu wo o fetoletšwego malemeng a makgolo, ke ile ka hlama motheo wa khoutu wo o arogilego bakeng sa leleme le lengwe le le lengwe gomme ka hlama mokgatlo wa go boloka motheo wa khoutu

Go beakanya phetogo ya tikologo `GITHUB_ACCESS_TOKEN` gomme ka morago o sepele [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) go tla hlama ka go iketla polokelo ya khoutu.

Ke therešo gore o ka e bea gape motheong wa khoutu.

Tšhupetšo ya sengwalwa sa phetolelo [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Khoutu ya sengwalwa e hlathollwa ka tsela ye e latelago:

[bunx](https://bun.sh/docs/cli/bunx) ke legato la npx, yeo e lego ka lebelo. Ke nnete, ge o se na bun ye e tsentšwego, o ka šomiša `npx` go e na le moo.

`bunx mdt zh` e tšweletša `.mdt` ka gare ga tšhupetšo ya zh bjalo ka `.md` , bona difaele tše 2 tše di kgokagantšwego ka mo tlase

* [kofi_gotee le.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kofi_gotee le.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` ke khoutu ya motheo bakeng sa phetolelo (haeba u na le `nodejs` feela hlomamisa, empa `bun` le `direnv` ha ba hlomamisa, u ka boela matha `npx i18n` ho fetolela).

E tla parse [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , peakanyo ya `i18n.yml` ka tokomane ena ke ka tsela e latelang:

```
en:
zh: ja ko en
```

Moelelo ke: Phetolelo ya Setšhaena go Sejapane, Sekorea, Seisemane, Phetolelo ya Seisemane go maleme a mangwe ka moka. Ge o nyaka go thekga Setšhaena le Seisemane fela, o ka no ngwala `zh: en` .

Ya mafelelo ke [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , yeo e ntšhago diteng magareng ga thaetlele ye kgolo le thaetlele ya mathomo ya `README.md` ya polelo ye nngwe le ye nngwe go tšweletša tsenyo `README.md` . Khoutu e bonolo kudu, o ka e lebelela ka bowena.

Google API e šomišwa bakeng sa phetolelo ya mahala. Ge e ba o sa kgone go fihlelela Google, hle beakanya le go beakanya moemedi, go swana le:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Sengwalwa sa phetolelo se tla tšweletša cache ye e fetoletšwego ka gare ga `.i18n` directory, hle e hlahlobje ka `git status` gomme o e oketše polokelong ya khoutu go efoga diphetolelo tše di boeletšwago.

Hle sepetša `bunx i18n` nako le nako ge o fetoša phetolelo go mpshafatša cache.

Ge e le gore sengwalwa sa mathomo le phetolelo di fetotšwe ka nako e tee, cache e tla gakantšhwa, ka fao ge o nyaka go fetoša, o ka fetoša e tee fela, gomme wa sepetša `bunx i18n` go mpshafatša cache.
