# đ react-component-template

A template for rapid development of React components, which satisfies component development, testing, packaging, release, document development, document packaging, and document deployment.

English | [įŽäŊä¸­æ](./README.zh-CN.md)

## đ How to use?

![](./assets/1.png)

## đ Catalog Introduction

```
âââ assets                 Store fixed resources
âââ docs                   Component documentation
â   âââ example            Demo tsx
â   âââ changelog.md       Used to display component history
â   âââ demo.md            Used to display component Demo
âââ src                    Component home directory
â   âââ index.ts           Component registration
â   âââ template.tsx       Component implementation code
âââ tests                  Component test code
â   âââ __snapshots__      Snapshot test file output without manual modification
â   âââ setup.ts           Init jest script
â   âââ index.spec.tsx     Test file
âââ .eslintrc.js           eslint config
âââ .fatherrc.ts           father config
âââ .umirc.ts              dumi config
âââ jest.config.js         jest config
âââ tsconfig.json          typescript config
```

The rest of the documents can be consulted by yourself.

## đ¤ Command introduction

| Name                     | Description              | Remarks                                                                                                            |
| ------------------------ | ------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `npm run start`          | Component development    | Document usage [dumi](https://github.com/umijs/dumi), component development and documentation development together |
| `npm run test`           | Component test           | -                                                                                                                  |
| `npm run lint`           | eslint verify            | -                                                                                                                  |
| `npm run build`          | Component packaging      | Use [father](https://github.com/umijs/father)                                                                      |
| `npm run coverage`       | Code coverage review     | -                                                                                                                  |
| `npm publish`            | Component release        | It is recommended to remove prepublishOnly for the first time                                                      |
| `npm run docs:build`     | Document packaging       | -                                                                                                                  |
| `npm run docs-dev:build` | Document packaging       | Use dumi dev environment                                                                                           |
| `npm run docs:deploy`    | Document release         | The default is to use GitHub Pages                                                                                 |
| `npm run deploy`         | Document package release | -                                                                                                                  |

## đ­ Component

### Development

```bash
npm i
npm run start
# http://localhost:8080/
```

### Test

```
npm run test
```

### Unpack

```bash
npm run build
```

- Use [father](https://github.com/umijs/father)
- More view official website configuration
- The package file is generated in the dist file by default

### Release

> `package.json` introduction

1. If you want to publish npm, `private` needs to be set to `false`.
2. The build command can be modified according to actual conditions.
3. After main decides to install the component, import points to it.
4. files Contains the files at the time of publishing, and includes README.md by default.
5. Others can be understood according to the meaning of the word.

## đ Documentation

### Start

```bash
npm run start
```

### Online preview

https://one-template.github.io/react-component-template/

### Description

- Use [dumi](https://github.com/umijs/dumi)
- Use basic layout, please add more by yourself
- Because the document is deployed on GitHub Pages, the `base` and `publicPath` of `.umirc.ts` are set to the project name
- One đ° : [ant-design-colorful](https://ant-design-colorful.github.io/ant-design-colorful/)

## đ Aide

- [Quickly modify the project name](./rename.ts)
- [Issue template](https://github.com/one-template/issue-template)
- [PR template](https://github.com/one-template/pr-template)
- [Actions use](https://github.com/github-actions-workflows/.github)

## đ Who are usingīŧ

- [image-component/react-image-shadow](https://github.com/image-component/react-image-shadow)
- [image-component/react-image-dangling](https://github.com/image-component/react-image-dangling)
- [image-component/react-image-follow](https://github.com/image-component/react-image-follow)

## License

[MIT](https://github.com/one-template/react-component-template/blob/main/LICENSE)
