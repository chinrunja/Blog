# npm 的使用

## 关于 npm

`npm` is the world's largest software registry. Open source developers from every continent use `npm` to share and borrow packages, and many organizations use `npm` to manage private development as well.[^1]

`npm` is the standard package manager for `Node.js`.[^2]

> `npm` 是世界上最大的软件注册中心（包管理软件）。 各大洲的开源开发者使用 `npm` 来分享和使用软件包，也有许多组织使用 `npm` 来管理私人开发。
>
> `npm` 是 `node.js` 标配的包管理器。

## 安装 npm

使用网站 <https://nodejs.org/en/download/> 下载并安装 `node`，打开终端，输入 `npm -v` 即可显示 `npm` 版本号。

因不同的包或项目依赖不同的 `node` 版本，建议使用 [nvm](https://github.com/nvm-sh/nvm) 管理 `node` 版本号。

## 初始化包管理文件 `package.json`

```sh
npm init <-y>
```

一个 package.json 文件的作用：

- 列出项目依赖的包
- 使用版本控制，指定项目的包版本
- 使构建可重现，易与其他开发人员共享

## 安装包、删除包

使用 `npm` 可以管理和下载项目的包依赖。项目的依赖会下载到当前 `node_modules` 目录下。

```
# 安装包
npm install <package_name>
# 或
npm i <package_name>

# 删除包
npm uninstall <package_name>
# 或
npm un <package_name>
```

附加安装指令：

- --save`[-S]`, 安装并添加文件到 `package.json` 的 `dependencies`。
- --save-dav`[-D]`, 安装并添加文件到 `package.json` 的 `devDependencies`。

## 更新和安装指定版本的包

```bash
# 更新
npm update

# 指定版本
npm install <package_name>@<version>
```

## 运行指令任务

```bash
npm run <task_name>
```

例如

```json
{
  "scripts": {
    "start-dev": "node lib/server-development",
    "start": "node lib/server-production"
  }
}
```

可以使用以下指令运行

```bash
npm run start-dev
npm run start

# start 指令可以简写
npm start
```

## 关于包版本的说明

示例 `package.json`:

```json
{
  "dependencies": {
    "cross-env": "^7.0.3",
    "dotenv": "^16.0.1",
    "express": "^4.17.3"
  }
}
```

- 若版本号前有 `^` 符号，则下载依赖包时，固定最大版本号，即版本的第一位数不变，后两位至最新；
- 若版本号前有 `~` 符号，则下载依赖包时，固定前两位版本号，即版本的最后一位至最新；
- 若版本号前有 `*` 符号，则版本不固定，下载至最新。

References

[^1]: [About npm](https://docs.npmjs.com/about-npm)
[^2]: [An introduction to the NPM package manager](https://nodejs.dev/en/learn/an-introduction-to-the-npm-package-manager/)
