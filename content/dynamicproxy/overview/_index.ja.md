---
title: "概要"
date: 2018-12-29T11:02:05+06:00
weight: 1
---

### What's this ?

Nginx をベースにしたプロキシサーバーを起動します。プロキシサーバー単体ではユーザーに対するサービスは提供しません。WordPress などのシステムをプロキシサーバーにバーチャルホストとして接続することによってサービスが提供されます。

プロキシサーバーはポート80番で待ち受け、接続されたバックエンドのバーチャルサーバーへアクセスを振り分けます。

プロキシサーバーを介す事によって、1台の物理的なサーバーで複数ドメインで複数のサービスを提供することが可能です。

例）

- コーポレートサイト: https://www.toybox.com
- ブログサイト: https://blog.toybox.com

プロキシサーバーは Let's Encrypt を利用した SSL 証明書によって、バックエンドのバーチャルサーバーへ SSL (HTTPS) 接続することが可能です。
また、プロキシサーバーはキャッシュ機能を備えているため、リバースプロキシとしても利用可能です。



### Feautures



