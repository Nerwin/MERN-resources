# My eslint config

+ .eslintignore

```shell
packages
node_modules
```

+ .eslintrc
```json
{
  "parser": "babel-eslint",
	"env": {
		"node": true,
		"es6": true
	},
	"rules": {
		"no-unused-vars": "warn",
		"no-extra-semi": "warn",
    "global-require": "warn",
    "block-spacing": "warn",
    "brace-style": ["warn", "1tbs", { "allowSingleLine": true }],
    "comma-dangle": ["warn", "always-multiline"],
    "capitalized-comments": ["warn", "always", { "ignoreConsecutiveComments": true }],
    "comma-spacing": ["warn", { "before": false, "after": true }],
    "comma-style": "warn",
    "computed-property-spacing": "warn",
    "eol-last": "warn",
    "func-call-spacing": "warn",
    "indent": ["error", 2],
    "no-mixed-spaces-and-tabs": ["error", "smart-tabs"],
		"semi": ["error", "always"],
    "react/jsx-uses-react": "error",
    "react/jsx-uses-vars": "error",
    "consistent-return": "off",
    "no-shadow": "off",
    "handle-callback-err": "off",
    "no-console": "off",
		"no-cond-assign": "off"
	},
	"extends": [
      "eslint:recommended",
      "airbnb",
      "plugin:security/recommended",
      "plugin:react/recommended"
    ], 
  "plugins": [
    "react"
  ],
	"parserOptions": {
        "ecmaVersion": 6,
        "ecmaFeatures": {
            "jsx": true
        }
	}
}
```

+ In the package.json

```json
"devDependencies": {
		"eslint": "^4.18.0",
    "eslint-config-airbnb": "^17.1.0",
    "eslint-plugin-import": "^2.14.0",
    "eslint-plugin-jsx-a11y": "^6.1.1",
    "eslint-plugin-react": "^7.11.1",
    "eslint-plugin-security": "^1.4.0",
	}
```
