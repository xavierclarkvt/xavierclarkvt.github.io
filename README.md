# xavierclarkvt.github.io : Portfolio Site For Xavier Clark

Will host images / videos / links / articles showcasing work done by Xavier Clark (me).

**Adding new projects requires that [pandoc](https://pandoc.org/installing.html) is installed.**

## Adding a new project:

Make a copy of `projects/temp.md` and edit it to your liking. 

When you are done, run:

```bash
pandoc -s --template=temp.html [doc].md -o [doc].html
```

and add an entry to `index.html`, ordered in terms of importance.

Format for homepage entry: 
```html
<a href="projects/[doc].html" class="project row [soft | hard | desg]">
    <h2 class="col align-self-center my-auto">
        Title (year): [description]
    </h2>
    <div class="col">
        <img src="[image link]" alt="image"/>
    </div>
    <div style="height: 5vh;"></div>
</a>
```