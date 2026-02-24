===== styling.css =====
# styling.css
Created 2026-02-24


## Description

## Journal
 - [X] Backlog
    - [ ] 
 - [X] Doing
 
## css code


*make.sh*
```bash
noweb.py -Rstyling.css styling.css.md > styling.css && echo 'styling.css' && notify-send -a "Compilation of styling.css" "" "$(date +"%Y-%m-%d") fertig" 
```


```bash
chmod u+x styling.css && ln -sf $(pwd)/styling.css ~/.local/bin/styling.css && echo 'fertig'
```

*styling.css*
```css
.button {
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 30px;
  margin: 4px 2px;
  cursor: pointer;
  border-radius: 12px;
  opacity: 0.75;
}

.avatar{
 border-radius : 50%;
}

.button1 {background-color: #88c0d0;  width: 35%;}/*#a626a4 #ea6f5a #b48ead*/
.button2 {background-color: #ea6f5a;  width: 100%;} 

/* Style the video: 100% width and height to cover the entire window */
#myVideo {
  position: fixed;
  top: 0;
  min-width: 100%;
  min-height: 100%;
  z-index: -1;
}

.linktree {
  /*position: fixed;
  background: rgba(0, 0, 0, 0.5);
  padding: 20px;
  color: #f1f1f1;
  */
  top: 0;
  color: #c8c8c8;
  width: 100%;
  z-index: 1;
}
```
