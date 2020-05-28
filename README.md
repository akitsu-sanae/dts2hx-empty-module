
`tsc` can handle this code, but `dts2hx` cannot.

```
$ npm install dts2hx --save-dev
$ npx tsc
$ node index.js
Hello
$ npx dts2hx ./index --tsconfig ./tsconfig.json
> Converting module ./index
> Error: Module not found hoge (SourceFile /path/to/dts2hx-empty-module/index.ts:1)
> Saved externs for ./index into externs/
```


