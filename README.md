```
npm i
npx parcel watch bundle.js
```

Save the empty `test.pug` (specified in the watch list in `tailwind.config.js`'s `content` section) as is and let parcel start recompilation but it takes a very long time (about a second for this small set of files but will get slower linearly with more files) instead of an instant update.

It compiles with normal speed if the stylus files are transpiled as CSS beforehand.
It also compiles faster (but not as fast as with CSS) if all the stylus files are concatenated into a single file.

```
npx stylus style/
```
and change `.styl` to `.css` in `bundle.js` and it works fast.
