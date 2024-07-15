# ACL4SSR-web

A web page that provides a link generator for ACL4SSR rules subscription conversion.

[中文文档](./README_CN.md)

## Introduction

Although there is already a great project: [GitHub - CareyWang/sub-web](https://github.com/CareyWang/sub-web), it does not offer an option for [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR) in its remote configuration. Therefore, I merged some configurations from [ACL4SSR 在线订阅转换](https://acl4ssr-sub.github.io/) and rewrote a page, while removing the short link generation feature.

## About the Backend

The web page only provides parameter concatenation, which is very simple. For details on the parameters, see [subconverter Readme-cn](https://github.com/tindy2013/subconverter/blob/master/README-cn.md#%E8%B0%83%E7%94%A8%E8%AF%B4%E6%98%8E-%E8%BF%9B%E9%98%B6). After obtaining the link, the server requested by the link will vary depending on the `backend address` selected. It is recommended to use a local or personal server setup. [subconverter](https://github.com/tindy2013/subconverter) provides multi-platform releases, which are very simple to try.

## Usage

Download/clone the project code, enter the root directory, and run the following commands:

```bash
npm install
```

```bash
npm run build
```

You will get the webpack-packaged static files in the dist directory.

You can also fork the project and deploy it directly on [Vercel](https://vercel.com).

## Customization

There are many backend parameters, and the page only provides a few commonly used ones. If needed, you may need to modify the options configuration in `src/config.ts` and the `generateSubUrl` function in `src/index.ts`.
