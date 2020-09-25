# yarr

yet another rss reader.

![screenshot](https://github.com/nkanaev/yarr/blob/master/artwork/promo.png?raw=true)

*yarr* is a server written in Go with the frontend in Vue.js. The storage is backed by SQLite.

The goal of the project is to provide a desktop application accessible via web browser.
Longer-term plans include a self-hosted solution for individuals.

There are plans to add support for mobile & tablet resolutions.
Support for 3rd-party applications (via Fever API) is being considered.

[download](https://github.com/nkanaev/yarr/releases/latest)

## credits

[Feather](http://feathericons.com/) for icons.



## Crear contenedor (Docker)

Instala `Go >= 1.14` and `gcc`. Get the source code:

```sh
git clone https://github.com/nkanaev/yarr.git
git clone https://github.com/nkanaev/gofeed.git
mv gofeed yarr
cd yarr
```

Then:
**docker build ** y crea la imagen

```
docker create --name=yarr -p 7070:7070  ugeek/yarr:amd64
```
