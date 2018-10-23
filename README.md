# tinyMCE-4-styles
tinyMCE-4-styles, published as GitGub Pages.

Chrome has recently started blocking the stylesheets, thus breaking the editor: 

"Access to CSS stylesheet at 'http://cdn.tinymce.com/4/skins/lightgray/content.min.css' from origin 'http://127.0.0.1:8000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource."

This is an attempt to fix that by using: importcss plugin

```
<TinyMCE
    content={'<div class="mceNonEditable">' + this.state.feedbackList[i].toString() + '</div>'}
    config={{
        plugins: 'noneditable autoresize importcss',
        autoresize_bottom_margin: 0,
        contenteditable: false,
        noneditable_noneditable_class: 'mceNonEditable',
        width: '100%',
        menubar: false,
        statusbar: false,
        toolbar: false,
        branding: false,
        importcss_append: false,
        content_css : "css/custom_content.css",
        content_style: 'body { background: #fdfdfd; border: 2px dashed #009BB4; ' +
            'border-radius: 25px; box-shadow: none; } div { padding: 30px; ' +
            '}',
    }}
/>
```