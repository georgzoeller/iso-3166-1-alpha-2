#Iso-3155-1-alpha-2  [![](https://travis-ci.org/georgzoeller/iso-3166-1-alpha-2.svg?branch=master)](https://travis-ci.org/georgzoeller/iso-3166-1-alpha-2) [![](https://img.shields.io/npm/v/iso-3166-1-alpha-2.svg?style=flat)](https://www.npmjs.com/package/iso-3166-1-alpha-2)

Simple lookup interface for iso country codes to countries and reverse.

Notes
- This package mirros an ISO spec and is used by a large number of packages who implement it expecting ISO adherence. Please direct requests for changes to country names or codes to the International Standards Organisation.
- This package is maintained but feature frozen, no new features will be added. Only changes to the ISO spec will be implemented.
- This package works browser and server side. The only dependency is mout.

## Installation

    npm install iso-3166-1-alpha-2

## Usage

    var iso3311a2 = require('./iso-3166-1-alpha-2')

    // Lookup country by code
    console.log iso3311a2.getCountry("DE")    // "Germany"

    // Lookup code by country
    console.log iso3311a2.getCode("Germany")  // "DE"

    // Get array of all country codes
    console.log iso3311a2.getCodes()          // ["AF","AX","AL",...]

    // Get array of all country names
    console.log iso3311a2.getCountries()      // ["Afghanistan","Åland Islands","Albania",...]

    // Get Object with code (key) to country (value) mappings
    console.log iso3311a2.getData()           // { "AF" : "Afghanistan", .... }


## Documentation

    Docco annotated source is found here: (docs/index.html)

