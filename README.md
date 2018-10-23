# tinyMCE-4-styles
tinyMCE-4 main script and styles, published as GitGub Pages as an alternative for the cdn.tinymce.com.

Chrome has recently started blocking the stylesheets if <script src="//cdn.tinymce.com/4/tinymce.min.js"></script> is used, thus breaking the editor: 
"Access to CSS stylesheet at 'http://cdn.tinymce.com/4/skins/lightgray/content.min.css' from origin 'http://127.0.0.1:8000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource."

Loading the script  like this: <script src="https://olli-suutari.github.io/tinyMCE-4-styles/tinymce.min.js"></script> and thus loading styles via: https://github.com/Olli-Suutari/tinyMCE-4-styles/tree/master/skins/lightgray seems to be working more reliably.

Code is copied from the offical tinymce repository:

https://github.com/tinymce/tinymce

License: https://github.com/tinymce/tinymce/blob/master/LICENSE.TXT

