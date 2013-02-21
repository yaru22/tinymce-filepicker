tinymce-filepicker
==================

Filepicker plugin for TinyMCE editor.


Installation
------------

Copy filepicker directory in this repository to TinyMCE's plugins directory.


Live Demo
---------

See the live demo [here](https://www.shopstarter.org/s/demo/). Click on 'Claim This Shop' (it's just a demo =) it's okay to claim it) button and you'll see TinyMCE editor in the customize page. You'll see the Filepicker icon on the editor's menu bar besides the unlink icon. Enjoy playing with the editor!

![TinyMCE-Filepicker Screenshot](https://dl.dropbox.com/u/35534880/TinyMCE-Filepicker.png "TinyMCE-Filepicker Integration")


Usage
-----

Include Filepicker's javascript

```<script src='//api.filepicker.io/v1/filepicker.js'></script>```

Include TinyMCE's javascript

e.g. ```<script src='js/tiny_mce/tiny_mce.js'></script>```

Set your Filepicker's API key

``` filepicker.setKey('YOUR-FILEPICKER-API-KEY-HERE'); ```

Initialize TinyMCE with Filepicker plugin

e.g.
```
  <script type='text/javascript'>
    tinyMCE.init({
      schema : 'html5',
      mode   : 'textareas',
      height : '500px',

      plugins : ' filepicker',  // Add filepicker plugin here.

      theme : 'advanced',
      theme_advanced_toolbar_location : 'top',
      theme_advanced_toolbar_align : 'left',
      theme_advanced_statusbar_location : 'bottom',
      theme_advanced_resizing : true,
      theme_advanced_buttons1 : 'save, bold, italic, underline, |, filepicker'  // Add filepicker button here.
    });
  </script>
```

See example/ for a working example source code.

