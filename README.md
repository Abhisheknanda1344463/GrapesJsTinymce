# GrapesJS Tinymce Editor

This plugin replaces the default Rich Text Editor with the one from Tinymce



## Summary

* Plugin
    * Name: `grapesjs-plugin-tinymce6`

# Author Contact
Skype: maxim2356
Telegram: @MaksymMalysh
Email: support@devfuture.pro

## Usage

```html
<link href="path/to/grapes.min.css" rel="stylesheet"/>
<script src="path/to/grapes.min.js"></script>
<script src="path/to/grapesjs-plugin-tinymce6.min.js"></script>

<div id="gjs"></div>

<script type="text/javascript">
  let editor = grapesjs.init({
    container : '#gjs',
    plugins: ['grapesjs-plugin-tinymce6'],
    pluginsOpts: {
      'grapesjs-plugin-tinymce6': {
        'tinymce-module': "https://cdn.tiny.cloud/1/no-api-key/tinymce/6/tinymce.min.js",
      },
      inline: ['span','a','button','h1','h2','h3','h4','h5','label'],
      inline_toolbar: [
        'bold italic underline strikethrough forecolor backcolor',
        'fontfamily fontsize'
      ],
      toolbar: [
        'bold italic underline strikethrough fontfamily fontsize outdent indent',
        'blocks forecolor backcolor | alignleft aligncenter alignright alignfull | numlist bullist'
      ],
      plugins:  [
        'link',
        'lists',
        'autolink'
      ]
    }
  });
</script>
```

## Add your API key

Replace `no-api-key` in the `pluginsOpts['tinymce-module']` path with a Tiny Cloud API key, 
which is created when signing up to the [Tiny Cloud](https://www.tiny.cloud/auth/signup/).

## Development

Clone the repository

```sh
$ git clone https://github.com/GoodPHP/grapesjs-plugin-tinymce6.git
$ cd grapesjs-plugin-tinymce6
```

Install dependencies

```sh
$ npm i
```

Start the dev server

```sh
$ npm start
```


## License

BSD 3-Clause
