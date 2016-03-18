# Demo for different handling of symlinks in Gulp3 and Gulp4

These are the source files:
```
|-- src
|   |-- foo
|       |-- baz > ../../vendor/bar
|-- vendor
    |-- bar
```

See the [Gulpfile](gulpfile.js) for the simple Gulp task that copies the directory `./src/` to the directory `./dest/`

With Gulp 3.9.1 the directory structure in `./dest/` is as follows:
```
|-- dest
    |-- foo
        |-- baz
```
(`baz` is a copy of `vendor/bar`)

## Instructions
Try it out with
```shell
npm install
npm run build
```
