# *DR. README md*

> #### *A simple readme reader. Turns a README.md into index.html for each directory. Also has the ability to inject tags and menus into the global template.*

***

## About

*DR. README md* is a simple markdown converter with a couple of extra features. 

*DR. README md* will convert any README file into a index file for that directory. 

*DR. README md* also has the ability to inject menus, can have the style sheet customized (*with or without SASS*) and uses a global template.

To ensure backward compatibility, *DR. README md* will only inject into and modify the global template. README files should remain just as they are and not have to be modified to add features.


## Installation 

DR. README .md is a node.js app. It requires nodejs > 6.1. It can be pulled via npm, yarn or pnpm.

```basic
npm install -g dr.readme.md
```

Once installed open your browser and drop a README.md into it. File locations are fine.

```c
file:///C:/Users/sfplinternet/Dropbox/Settings/Devices/Windows%2010%20Public%20Library/README.md
```

### Configuration per Project

```npm
cd root/dir/of/project

doc new
```

This will create the `.doc` folder in the root of the project.

### **Inside the `.doc` folder**

```bash
.doc # Per project hidden folder to customize dr.readme with
    scss/ # (if) this folder exists (then) use scss.
          # Otherwise, just write in the styles.css file
        styles.scss # The global style sheet. styles.css        
                    #  will be generated from this.
        0.scss # A sub (included) scss file.
    styles.css # The stylesheet to render the md files with
    js/ # Folder to hold js files
        app.js # The main app javascript file
    bundle.js # The compiled/bundled production javascript file
    template.html # The Global HTML template
    media/ # Folder to hold any assets used in theming
        logo.png # A hypothetical logo file
```

## Chrome Plugin

There's a cool Chrome plugin called [*"Markdown Reader"*](https://chrome.google.com/webstore/detail/md-reader/medapdbncneneejhbgcjceippjlfkmkg/related). It's got a bit of extensibility to it :)


***

🤍 2023 [**Brenton Holiday**](https://allmylinks.com/8rents) *(aka **8rents**)*
