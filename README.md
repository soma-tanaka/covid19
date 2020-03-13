# 山梨県 新型コロナウイルス感染症対策サイト

[![山梨県 新型コロナウイルス感染症対策サイト](https://user-images.githubusercontent.com/2931035/76643703-ef278380-6598-11ea-9cf1-4e3a44c93bdc.jpg)](https://stopcovid19.yamanashi.dev/)

### 日本語 | [English](./README_EN.md) | [Spanish](./README_ES.md) | [Korean](./README_KO.md) | [Chinese (Taiwan)](./README_ZH_TW.md) | [Chinese (Simplified)](./README_ZH_CN.md) | [Vietnamese](./README_VI.md)

## 貢献の仕方
Issues にあるいろいろな修正にご協力いただけると嬉しいです。

## ライセンス
本ソフトウェアは、[MITライセンス](./LICENSE.txt)の元提供されています。

## 開発者向け情報

### 環境構築の手順

- 必要となるNode.jsのバージョン: 10.19.0以上

**yarn を使う場合**
``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**docker compose を使う場合**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### `Cannot find module ****` と怒られた時

**yarn を使う場合**
```
$ yarn install
```

**docker compose を使う場合**
```bash
$ docker-compose run --rm app yarn install
```
