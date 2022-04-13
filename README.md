# Taxonomy issue minimal reproduction repo

Reproduces error where taxonomy index collides with content page when building with hugo.

### Usage
Clone repo and run the following script, which will run 10 consecutive builds, comparing the size of generated `properties/index.html` file.

```
./buildTest 10
```
You can check the file contents in `public/properties/index.html.alternative.html` and `public/properties/index.html.initial.html`

To play around, you can also run `hugo server`, save `layouts/_default/properties-list.html` and see that the output will evetually change.
