# Typescript issue with `exclude`

To see the issue:

```bash
cd a
npm ci
npm run watch
```

You get an error from `../b/data/__tests__/shouldnotbeincluded.test.ts` which should be excluded based on `tsconfig.json`

```
  "include": ["src", "../b"],
  "exclude": ["node_modules", "**/b/**", "**/*.test.ts"]
```
