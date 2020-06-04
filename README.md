## eslint 的规范
> 这个是内部用的规范
---
## 使用
```bash
npm install --save-dev eslint-config-ro
```
## 然后在你自己的eslint的配置文件上引入
```javascript
"extends": [
    "ro"
]
```
---
## dependencies
```javascript
"dependencies": {
    "babel-eslint": "^10.0.1",
    "eslint": "^7.1.0",
    "eslint-plugin-react": "^7.20.0"
  }
```
---
## 完整的规则如下
```json
{
    "parser": "babel-eslint",
    "env": {
        "node": true,
        "es6": true,
        "browser": true
    },
    "extends": [
        "eslint:recommended",
        "plugin:react/recommended"
    ],
    "parserOptions": {
        "ecmaFeatures": {
            "jsx": true
        },
        "ecmaVersion": 11,
        "sourceType": "module"
    },
    "plugins": [
        "react"
    ],
    "rules": {
        "react/prop-types": "off",
        "react/no-typos": "error",
        "no-console": "off",
        "no-prototype-builtins": "off",
        "semi": ["error", "never"],
        "indent": [ "error", 2 ],
        "quotes": ["error", "single"],
        "block-spacing": "error",
        "space-before-blocks": "error",
        "object-curly-spacing": ["error", "always"],
        "no-duplicate-imports": "error",
        "no-var": "error",
        "require-await": "error",
        "computed-property-spacing": "error",
        "lines-between-class-members": "error",
        "key-spacing": "error",
        "no-nested-ternary": "error",
        "no-multiple-empty-lines": ["error", { "max": 1, "maxBOF": 1 }],
        "space-before-function-paren": "error",
        "arrow-spacing": "error",
        "rest-spread-spacing": "error",
        "no-unneeded-ternary": "error",
        "eqeqeq": "error",
        "space-infix-ops": "error",
        "switch-colon-spacing": "error",
        "no-multi-spaces": "error",
        "array-bracket-spacing": "error",
        "comma-spacing": "error",
        "space-unary-ops": "error"
    }
}
```
## license
MIT