# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for my projects

This config is intended to be used in nextjs projects.

## Install

```sh
yarn add -D @pnxdxt/tsconfig
```

_This config requires TypeScript 4.7 or later._

## Usage

`tsconfig.json`

```json
{
	"extends": "@pnxdxt/tsconfig",
	"compilerOptions": {
		"baseUrl": ".",
		"paths": {
			"@/pages/*": ["pages/*"],
			"@/api/*": ["pages/api/*"]
		}
	},
	"include": [
		"next-env.d.ts",
		"**/*.ts",
		"**/*.tsx",
		"**/*.cjs",
		"**/*.mjs",
		".next/types/**/*.ts"
	],
	"exclude": ["node_modules"]
}
```
