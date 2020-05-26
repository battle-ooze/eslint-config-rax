## 安装

```
npm install eslint-config-rax
```

依赖的库有：
```
  // 基础依赖
  "babel-eslint": "^10.1.0",
  "eslint": "^7.1.0",
  "eslint-plugin-import": "^2.20.2",
  // 使用Typescript时依赖
  "@typescript-eslint/eslint-plugin": "^3.0.1",
  "@typescript-eslint/parser": "^3.0.1",
  "typescript": "^3.9.3"
  // 使用React时依赖
  "eslint-plugin-react": "^7.20.0",
```

## 使用

 设置 `.eslintrc.js` 内容如下：

 * 普通JS项目设置示例见 [.eslintrc.js](https://github.com/raxjs/eslint-config-rax/blob/master/test/base/.eslintrc.js)
 * React项目设置示例见 [.eslintrc.js](https://github.com/raxjs/eslint-config-rax/blob/master/test/react/.eslintrc.js)
 * Typescript 项目设置示例见 [.eslintrc.js](https://github.com/raxjs/eslint-config-rax/blob/master/test/typescript/.eslintrc.js)
 * React Typescript 项目设置示例见 [.eslintrc.js](https://github.com/raxjs/eslint-config-rax/blob/master/test/typescript-react/.eslintrc.js)


## 规则定义说明

* [基础规则](https://github.com/raxjs/eslint-config-rax/blob/master/index.js) 基于[Rax](https://github.com/alibaba/rax) 相关项目沉淀
* [React规则](https://github.com/raxjs/eslint-config-rax/blob/master/react.js) 基于[Rax](https://github.com/alibaba/rax) 相关项目沉淀
* [Typescript规则](https://github.com/raxjs/eslint-config-rax/blob/master/typescript.js) 基于 [@typescript-eslint/eslint-plugin](https://github.com/typescript-eslint/typescript-eslint/tree/master/packages/eslint-plugin#supported-rules) 推荐规则

## 修改规则


若修改增添规则，请提供规则的用处和理由

比如:

```javascript
    /**
     * Indent is replaced by two Spaces
     * @reason Conventional convention
    */
    "indent": "off",
    '@typescript-eslint/indent': [
      'error',
      2,
      {
        SwitchCase: 1,
        flatTernaryExpressions: true
      }
    ],
```
