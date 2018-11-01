pomelo-kcp-x
============

[![Build Status][1]][2]

[1]: https://api.travis-ci.org/leenjewel/node-kcp.svg?branch=master
[2]: https://travis-ci.org/leenjewel/node-kcp


[KCP Protocol](https://github.com/skywind3000/kcp) for [Pomelo](https://github.com/NetEase/pomelo)

fork 说明
============

修改了 leenjewel/pomelo-kcp

原本是所有连接共用一个 conv

改为根据客户端发来的消息的 conv 创建对应的 kcpsocket 对象

方便跟 tcp 连接相互配合着使用，参见 [skywind3000 的 wiki](https://github.com/skywind3000/kcp/wiki/Cooperate-With-Tcp-Server)

发布在 npm 上的名字是 [pomelo-kcp-x](https://www.npmjs.com/package/pomelo-kcp-x)

迁移说明
====

增加了一个 ts 版本 [pinus-kcp](https://github.com/bruce48x/pinus-kcp#readme)

配合 pinus 使用 ( typescript 版本的 pomelo )

typescript 在开发上完爆 js，强烈建议迁移到 typescript，难度不大。
