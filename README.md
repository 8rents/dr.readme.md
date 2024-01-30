# dr.readme.md

> #### *A simple readme reader  & writer. Turns a README.md into index.html for each directory. Also has the ability to inject tags and menus into the global template.*

***

## About

*Dr.readme.md* is a simple markdown converter with a couple of extra features. 

*Dr.readme.md* will convert any README file into a index file for that directory. It does so by creating a cache or build directory and creating a web server. Page edits are live updated to the build directory.

*Dr.readme.md* also has the ability to inject menus, can have the style sheet customized (*with or without SASS*) and uses a global template.

To ensure backward compatibility, *Dr.readme.md* will only inject into and modify the global template. README files should remain just as they are and not have to be modified to add features.

## Usage

DR. README .md is a node.js app. There is an Electron version with a GUI and a Command line utility.

### Electron Version

Can be downloaded from https://github.com/8rents/dr.readme.md/releases.

**Once downloaded:**

1. Open the app
2. select a folder to start or read a project
3. Click start

This will open up a window. If there is an existing README.md in the folder it will be rendered on screen. If there is no README.md file in that directory, one will be created.	

### Command line utility Through NPM

Install through NPM, Yarn or PNPM. It should ideally be installed globally.

```bash
# Install dr.readme.md globally
npm install -g 8rents/dr.readme.md

# Navigate to a directory that will be 
# project root(if no README.md exists,
# one will be created)
cd to/root/directory

# Start dr.readme.md from this directory
# (readme & drm are the same command)
drm start
```

If no `README.md` exists in that folder a generic one will be created.

### 


***

🤍 2023 [**Brenton Holiday**](https://allmylinks.com/8rents) *(aka **8rents**)*
