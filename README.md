# julian-hrb.github.io

Sitio de enlaces de **Indabox**. Cada etiqueta QR o tag NFC de la app lleva `https://julian-hrb.github.io/l/<id>`:

- Con la app instalada, Android abre Indabox directo (App Links verificados con `.well-known/assetlinks.json`; en los tags NFC además va un Android Application Record).
- En iPhone, `.well-known/apple-app-site-association` permite los *universal links*: al acercar un tag, se abre la app. Hay que reemplazar `TEAMID` por el Team ID de la cuenta de Apple Developer.
- Sin la app, `404.html` explica qué es e intenta abrir `indabox://open/l/<id>`.

`.nojekyll` evita que GitHub Pages ignore la carpeta `.well-known`.
