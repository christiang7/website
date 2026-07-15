# index.html
Created 2026-07-15


## Description

## Journal
 - [X] Backlog
    - [ ] 
 - [X] Doing
 
## html code


 
### Compilation code

*make.sh*
```bash
noweb.py -Rindex.html index.html.md > index.html && echo 'index.html' && notify-send -a "Compilation of index.html" "" "$(date +"%Y-%m-%d") fertig" 
```


```bash
chmod u+x index.html && ln -sf $(pwd)/index.html ~/.local/bin/index.html && echo 'fertig'
```

### index.html



*index.html*
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Personal Website of Christian Gößl</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="description" content="Personal Website of Christian Gößl">
    <meta name="viewport" content="width=device-width,initial-scale=1" />
    <link rel="icon" href="favicon.ico" />
    <!--   <link      rel="stylesheet"       href="vue.css"     /> 
    
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify/themes/dark.css" />
    -->
    <link rel="stylesheet" href="nordic.css" />
    <link rel="stylesheet" href="styling.css" />
</head>
<body>

    <div id="app"></div>

</body>
<script>
window.$docsify = {
    loadNavbar: true,
    autoHeader: true,
    auto2top: true,
    subMaxLevel: 3,
    latex: {
        inlineMath   : [['%%', '%%'],['\\(', '\\)']], // default ['$', '$'],
        displayMath  : [['$$', '$$']],               // default
    },
    coverpage: true,
    search: 'auto', // default
    search: [
        '/',            // => /README.md
        '/Blog',       // => /Blog.md
        '/Physik', // => /Physik.md
        '/Coding',      // => /zh-cn/README.md
    ],
    search: {
        // insertAfter: '.app-name',
        // insertBefore: '.sidebar-nav',
        noData: { '/' : 'No Results' ,},//
        paths: [], //'auto', // or []
        //maxAge: 86400000, // Expiration time, the default one day
        placeholder: {'/': 'Search',}, // depth: 2,
        //hideOtherSidebarContent: false,
        //pathNamespaces: /^(\/(zh-cn|ru-ru))?(\/(v1|v2))?/,
        //pathNamespaces: ['/', '/Blog', '/Coding','/Physik'],
        depth: 6,
    },
    name: 'Home',
    plugins: [
    function pageFooter(hook, vm) {
        var footer = [
            '<hr/>',
            '<footer style="font-size: 13px;">',
            '<a href="https://creativecommons.org/licenses/by-sa/4.0/">CC BY-SA 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"> Website created with <a href="https://docsify.js.org/">Docsify</a> and language <a href="https://markdown.de/">Markdown</a>. Hosted on <a href="https://github.com/christiang7/website">Github</a>. Colortheme by <a href="https://github.com/nordtheme/nord">nord</a>',
            '</footer>',
        ].join('');

        hook.afterEach(function (html) {
            return html + footer;
        });
        },
    ],
};
</script>
    
<!-- load docsify script -->
<script src="//cdn.jsdelivr.net/npm/docsify@4"></script>

<!-- load latex engine -->

<script src="//cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<!-- load latex docsify script -->

<script src="//cdn.jsdelivr.net/npm/docsify-latex@0"></script>

<!-- load search docsify script -->

<!-- <script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.js"></script> -->

<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>

<!-- load code syntax highlight docsify script -->

<script src="//cdn.jsdelivr.net/npm/prismjs@1/components/prism-bash.min.js"></script>

</html>

```

