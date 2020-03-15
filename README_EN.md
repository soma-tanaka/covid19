# Yamanashi COVID-19 Task Force website

![production deploy](https://github.com/covid19-yamanashi/covid19/workflows/production%20deploy/badge.svg)

[![Yamanashi COVID-19 Task Force website](https://user-images.githubusercontent.com/2931035/76643703-ef278380-6598-11ea-9cf1-4e3a44c93bdc.jpg)](https://stopcovid19.yamanashi.dev/)

### [日本語](./README.md) | English | [Spanish](./README_ES.md) | [Korean](./README_KO.md) | [Chinese (Taiwan)](./README_ZH_TW.md) | [Chinese (Simplified)](./README_ZH_CN.md) | [Vietnamese](./README_VI.md)

## How to Contribute

All contributions are welcome!

## License
This software is released under [the MIT License](./LICENSE.txt).

## For Developers

### How to Set Up Environments

- Required Node.js version: 10.19.0 or higher

**Use yarn**
``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**Use docker**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### How to resolve `Cannot find module ****` error

**Use yarn**
```
$ yarn install
```

**Use docker**
```bash
$ docker-compose run --rm app yarn install
```
