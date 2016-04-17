## MS SQL Server Waterline Adapter

[![NPM version][npm-image]][npm-url]
[![Build status][ci-image]][ci-url]
[![Dependency Status][daviddm-image]][daviddm-url]

Official Microsoft SQL Server adapter for Waterline. Tested on SQL Server 2012 and 2014,
but should support any SQL Server 2005 and newer.

### 1. Install
```sh
$ npm install waterline-mssql --save
```

### 2. Configure

#### `config/models.js`
```js
{
  connection: 'sqlserver'
}
```

#### `config/connections.js`
```js
{
  sqlserver: {
    adapter: 'waterline-mssql',
    user: 'cnect',
    password: 'pass',
    host: 'abc123.database.windows.net' // azure database
    database: 'mydb',
    options: {
      encrypt: true   // use this for Azure databases
    }
  }
}
```

## License
MIT

## Maintained By
[<img src='http://i.imgur.com/Y03Jgmf.png' height='64px'>](http://langa.io)

[npm-image]: https://img.shields.io/npm/v/sails-sqlserver.svg?style=flat-square
[npm-url]: https://npmjs.org/package/sails-sqlserver
[ci-image]: https://img.shields.io/circleci/project/cnect/sails-sqlserver/master.svg?style=flat-square
[ci-url]: https://circleci.com/gh/cnect/sails-sqlserver
[daviddm-image]: http://img.shields.io/david/cnect/sails-sqlserver.svg?style=flat-square
[daviddm-url]: https://david-dm.org/cnect/sails-sqlserver
