```
npm i
npx parcel watch bundle.js
```

Save the empty `test.pug` (specified in the watch list in `tailwind.config.js`'s `content` section) as is and let parcel start recompilation but it takes a very long time (about a second for this small set of files but will get slower linearly with more files) instead of an instant update.

It compiles with normal speed if the files in `style` are concatenated into a single file or the stylus files are transpiled as CSS beforehand.
