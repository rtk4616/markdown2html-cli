# markdown2html-cli
markdown to html use gulp ,support auto toc , syntax highlight.

## How to use?
move to the root dir of project, rename your md file to index.md, run:  
```
npm install
```
then run:   
```
gulp tohtml    
```
the generated file located in  dist/index.html.

But, what if i want to real-time preview when i write markdown file,don't worry.you can use `gulp watch` like below:
1、first you should install chrome ext named livereload
2、ordered run commandline:
```sh
$ cd your_work_dir
$ http-server
$ gulp watch
```
now you can open `127.0.0.1:8080/index.html` to see it.

### Cli args:
--path : the work filepath ,it support gulp path syntax like *.md,**/*.md,etc.
--title: the file title.

example use:  
```
gulp tohtml --path **/*.md --title demo-page 
```

AnyWhere,Before you start your work for it ,now please see dist/index.html.  the source code of index.md is a demo article, the generated index.html look like below:   
![](111.png)    
