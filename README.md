# api documentation for  [is_js (v0.9.0)](http://is.js.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-is_js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-is_js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-is_js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-is_js)
#### micro check library

[![NPM](https://nodei.co/npm/is_js.png?downloads=true)](https://www.npmjs.com/package/is_js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-is_js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-is_js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-is_js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/arasatasaygin/is.js/issues"
    },
    "dependencies": {},
    "description": "micro check library",
    "devDependencies": {
        "chai": "^3.4.0",
        "eslint": "^2.13.1",
        "lodash": "^4.15.0",
        "mocha": "^2.2.1",
        "mocha-phantomjs": "^4.1.0",
        "pre-commit": "^1.1.3",
        "uglify-js": "^2.7.3"
    },
    "directories": {},
    "dist": {
        "shasum": "0ab94540502ba7afa24c856aa985561669e9c52d",
        "tarball": "https://registry.npmjs.org/is_js/-/is_js-0.9.0.tgz"
    },
    "files": [
        "is.js",
        "is.min.js"
    ],
    "homepage": "http://is.js.org/",
    "license": "MIT",
    "main": "is.js",
    "maintainers": [
        {
            "name": "arasatasaygin",
            "email": "arasatasaygin@gmail.com"
        },
        {
            "name": "jdalton",
            "email": "john.david.dalton@gmail.com"
        }
    ],
    "name": "is_js",
    "optionalDependencies": {},
    "pre-commit": [
        "lint"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/arasatasaygin/is.js.git"
    },
    "scripts": {
        "build": "npm run lint && npm run min",
        "lint": "eslint .",
        "min": "uglifyjs is.js -m --comments \"/^!/\" -o is.min.js",
        "test": "mocha --check-leaks -R dot",
        "test:phantom": "mocha-phantomjs -R dot test/index.html"
    },
    "version": "0.9.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module is_js](#apidoc.module.is_js)
1.  [function <span class="apidocSignatureSpan">is_js.</span>above (n, min)](#apidoc.element.is_js.above)
1.  [function <span class="apidocSignatureSpan">is_js.</span>affirmative (value)](#apidoc.element.is_js.affirmative)
1.  [function <span class="apidocSignatureSpan">is_js.</span>alphaNumeric (value)](#apidoc.element.is_js.alphaNumeric)
1.  [function <span class="apidocSignatureSpan">is_js.</span>android ()](#apidoc.element.is_js.android)
1.  [function <span class="apidocSignatureSpan">is_js.</span>androidPhone ()](#apidoc.element.is_js.androidPhone)
1.  [function <span class="apidocSignatureSpan">is_js.</span>androidTablet ()](#apidoc.element.is_js.androidTablet)
1.  [function <span class="apidocSignatureSpan">is_js.</span>arguments (value)](#apidoc.element.is_js.arguments)
1.  [function <span class="apidocSignatureSpan">is_js.</span>array ()](#apidoc.element.is_js.array)
1.  [function <span class="apidocSignatureSpan">is_js.</span>blackberry ()](#apidoc.element.is_js.blackberry)
1.  [function <span class="apidocSignatureSpan">is_js.</span>boolean (value)](#apidoc.element.is_js.boolean)
1.  [function <span class="apidocSignatureSpan">is_js.</span>caPostalCode (value)](#apidoc.element.is_js.caPostalCode)
1.  [function <span class="apidocSignatureSpan">is_js.</span>capitalized (string)](#apidoc.element.is_js.capitalized)
1.  [function <span class="apidocSignatureSpan">is_js.</span>char (value)](#apidoc.element.is_js.char)
1.  [function <span class="apidocSignatureSpan">is_js.</span>chrome (range)](#apidoc.element.is_js.chrome)
1.  [function <span class="apidocSignatureSpan">is_js.</span>creditCard (value)](#apidoc.element.is_js.creditCard)
1.  [function <span class="apidocSignatureSpan">is_js.</span>date (value)](#apidoc.element.is_js.date)
1.  [function <span class="apidocSignatureSpan">is_js.</span>dateString (value)](#apidoc.element.is_js.dateString)
1.  [function <span class="apidocSignatureSpan">is_js.</span>day (date, day)](#apidoc.element.is_js.day)
1.  [function <span class="apidocSignatureSpan">is_js.</span>dayLightSavingTime (date)](#apidoc.element.is_js.dayLightSavingTime)
1.  [function <span class="apidocSignatureSpan">is_js.</span>decimal (n)](#apidoc.element.is_js.decimal)
1.  [function <span class="apidocSignatureSpan">is_js.</span>desktop ()](#apidoc.element.is_js.desktop)
1.  [function <span class="apidocSignatureSpan">is_js.</span>domNode (object)](#apidoc.element.is_js.domNode)
1.  [function <span class="apidocSignatureSpan">is_js.</span>edge (range)](#apidoc.element.is_js.edge)
1.  [function <span class="apidocSignatureSpan">is_js.</span>email (value)](#apidoc.element.is_js.email)
1.  [function <span class="apidocSignatureSpan">is_js.</span>empty (value)](#apidoc.element.is_js.empty)
1.  [function <span class="apidocSignatureSpan">is_js.</span>endWith (string, target)](#apidoc.element.is_js.endWith)
1.  [function <span class="apidocSignatureSpan">is_js.</span>eppPhone (value)](#apidoc.element.is_js.eppPhone)
1.  [function <span class="apidocSignatureSpan">is_js.</span>equal (value, other)](#apidoc.element.is_js.equal)
1.  [function <span class="apidocSignatureSpan">is_js.</span>error (value)](#apidoc.element.is_js.error)
1.  [function <span class="apidocSignatureSpan">is_js.</span>even (n)](#apidoc.element.is_js.even)
1.  [function <span class="apidocSignatureSpan">is_js.</span>existy (value)](#apidoc.element.is_js.existy)
1.  [function <span class="apidocSignatureSpan">is_js.</span>falsy (value)](#apidoc.element.is_js.falsy)
1.  [function <span class="apidocSignatureSpan">is_js.</span>finite ()](#apidoc.element.is_js.finite)
1.  [function <span class="apidocSignatureSpan">is_js.</span>firefox (range)](#apidoc.element.is_js.firefox)
1.  [function <span class="apidocSignatureSpan">is_js.</span>function (value)](#apidoc.element.is_js.function)
1.  [function <span class="apidocSignatureSpan">is_js.</span>future (date)](#apidoc.element.is_js.future)
1.  [function <span class="apidocSignatureSpan">is_js.</span>hexColor (value)](#apidoc.element.is_js.hexColor)
1.  [function <span class="apidocSignatureSpan">is_js.</span>hexadecimal (value)](#apidoc.element.is_js.hexadecimal)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ie (range)](#apidoc.element.is_js.ie)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inArray (value, array)](#apidoc.element.is_js.inArray)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inDateRange (date, start, end)](#apidoc.element.is_js.inDateRange)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inLastMonth (date)](#apidoc.element.is_js.inLastMonth)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inLastWeek (date)](#apidoc.element.is_js.inLastWeek)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inLastYear (date)](#apidoc.element.is_js.inLastYear)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inNextMonth (date)](#apidoc.element.is_js.inNextMonth)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inNextWeek (date)](#apidoc.element.is_js.inNextWeek)
1.  [function <span class="apidocSignatureSpan">is_js.</span>inNextYear (date)](#apidoc.element.is_js.inNextYear)
1.  [function <span class="apidocSignatureSpan">is_js.</span>include (string, target)](#apidoc.element.is_js.include)
1.  [function <span class="apidocSignatureSpan">is_js.</span>infinite (n)](#apidoc.element.is_js.infinite)
1.  [function <span class="apidocSignatureSpan">is_js.</span>integer (n)](#apidoc.element.is_js.integer)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ios ()](#apidoc.element.is_js.ios)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ip (value)](#apidoc.element.is_js.ip)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ipad (range)](#apidoc.element.is_js.ipad)
1.  [function <span class="apidocSignatureSpan">is_js.</span>iphone (range)](#apidoc.element.is_js.iphone)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ipod (range)](#apidoc.element.is_js.ipod)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ipv4 (value)](#apidoc.element.is_js.ipv4)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ipv6 (value)](#apidoc.element.is_js.ipv6)
1.  [function <span class="apidocSignatureSpan">is_js.</span>json (value)](#apidoc.element.is_js.json)
1.  [function <span class="apidocSignatureSpan">is_js.</span>leapYear (year)](#apidoc.element.is_js.leapYear)
1.  [function <span class="apidocSignatureSpan">is_js.</span>linux ()](#apidoc.element.is_js.linux)
1.  [function <span class="apidocSignatureSpan">is_js.</span>lowerCase (string)](#apidoc.element.is_js.lowerCase)
1.  [function <span class="apidocSignatureSpan">is_js.</span>mac ()](#apidoc.element.is_js.mac)
1.  [function <span class="apidocSignatureSpan">is_js.</span>mobile ()](#apidoc.element.is_js.mobile)
1.  [function <span class="apidocSignatureSpan">is_js.</span>month (date, month)](#apidoc.element.is_js.month)
1.  [function <span class="apidocSignatureSpan">is_js.</span>nan (value)](#apidoc.element.is_js.nan)
1.  [function <span class="apidocSignatureSpan">is_js.</span>nanpPhone (value)](#apidoc.element.is_js.nanpPhone)
1.  [function <span class="apidocSignatureSpan">is_js.</span>negative (n)](#apidoc.element.is_js.negative)
1.  [function <span class="apidocSignatureSpan">is_js.</span>null (value)](#apidoc.element.is_js.null)
1.  [function <span class="apidocSignatureSpan">is_js.</span>number (value)](#apidoc.element.is_js.number)
1.  [function <span class="apidocSignatureSpan">is_js.</span>object (value)](#apidoc.element.is_js.object)
1.  [function <span class="apidocSignatureSpan">is_js.</span>odd (n)](#apidoc.element.is_js.odd)
1.  [function <span class="apidocSignatureSpan">is_js.</span>offline ()](#apidoc.element.is_js.offline)
1.  [function <span class="apidocSignatureSpan">is_js.</span>online ()](#apidoc.element.is_js.online)
1.  [function <span class="apidocSignatureSpan">is_js.</span>opera (range)](#apidoc.element.is_js.opera)
1.  [function <span class="apidocSignatureSpan">is_js.</span>palindrome (string)](#apidoc.element.is_js.palindrome)
1.  [function <span class="apidocSignatureSpan">is_js.</span>past (date)](#apidoc.element.is_js.past)
1.  [function <span class="apidocSignatureSpan">is_js.</span>phantom (range)](#apidoc.element.is_js.phantom)
1.  [function <span class="apidocSignatureSpan">is_js.</span>positive (n)](#apidoc.element.is_js.positive)
1.  [function <span class="apidocSignatureSpan">is_js.</span>propertyCount (object, count)](#apidoc.element.is_js.propertyCount)
1.  [function <span class="apidocSignatureSpan">is_js.</span>propertyDefined (object, property)](#apidoc.element.is_js.propertyDefined)
1.  [function <span class="apidocSignatureSpan">is_js.</span>quarterOfYear (date, quarter)](#apidoc.element.is_js.quarterOfYear)
1.  [function <span class="apidocSignatureSpan">is_js.</span>regexp (value)](#apidoc.element.is_js.regexp)
1.  [function <span class="apidocSignatureSpan">is_js.</span>safari (range)](#apidoc.element.is_js.safari)
1.  [function <span class="apidocSignatureSpan">is_js.</span>sameType (value, other)](#apidoc.element.is_js.sameType)
1.  [function <span class="apidocSignatureSpan">is_js.</span>setNamespace ()](#apidoc.element.is_js.setNamespace)
1.  [function <span class="apidocSignatureSpan">is_js.</span>setRegexp (regexp, name)](#apidoc.element.is_js.setRegexp)
1.  [function <span class="apidocSignatureSpan">is_js.</span>socialSecurityNumber (value)](#apidoc.element.is_js.socialSecurityNumber)
1.  [function <span class="apidocSignatureSpan">is_js.</span>sorted (array, sign)](#apidoc.element.is_js.sorted)
1.  [function <span class="apidocSignatureSpan">is_js.</span>space (value)](#apidoc.element.is_js.space)
1.  [function <span class="apidocSignatureSpan">is_js.</span>startWith (string, target)](#apidoc.element.is_js.startWith)
1.  [function <span class="apidocSignatureSpan">is_js.</span>string (value)](#apidoc.element.is_js.string)
1.  [function <span class="apidocSignatureSpan">is_js.</span>tablet ()](#apidoc.element.is_js.tablet)
1.  [function <span class="apidocSignatureSpan">is_js.</span>timeString (value)](#apidoc.element.is_js.timeString)
1.  [function <span class="apidocSignatureSpan">is_js.</span>today (date)](#apidoc.element.is_js.today)
1.  [function <span class="apidocSignatureSpan">is_js.</span>tomorrow (date)](#apidoc.element.is_js.tomorrow)
1.  [function <span class="apidocSignatureSpan">is_js.</span>touchDevice ()](#apidoc.element.is_js.touchDevice)
1.  [function <span class="apidocSignatureSpan">is_js.</span>truthy ()](#apidoc.element.is_js.truthy)
1.  [function <span class="apidocSignatureSpan">is_js.</span>ukPostCode (value)](#apidoc.element.is_js.ukPostCode)
1.  [function <span class="apidocSignatureSpan">is_js.</span>undefined (value)](#apidoc.element.is_js.undefined)
1.  [function <span class="apidocSignatureSpan">is_js.</span>under (n, max)](#apidoc.element.is_js.under)
1.  [function <span class="apidocSignatureSpan">is_js.</span>upperCase (string)](#apidoc.element.is_js.upperCase)
1.  [function <span class="apidocSignatureSpan">is_js.</span>url (value)](#apidoc.element.is_js.url)
1.  [function <span class="apidocSignatureSpan">is_js.</span>usZipCode (value)](#apidoc.element.is_js.usZipCode)
1.  [function <span class="apidocSignatureSpan">is_js.</span>weekday ()](#apidoc.element.is_js.weekday)
1.  [function <span class="apidocSignatureSpan">is_js.</span>weekend (date)](#apidoc.element.is_js.weekend)
1.  [function <span class="apidocSignatureSpan">is_js.</span>windowObject (value)](#apidoc.element.is_js.windowObject)
1.  [function <span class="apidocSignatureSpan">is_js.</span>windows ()](#apidoc.element.is_js.windows)
1.  [function <span class="apidocSignatureSpan">is_js.</span>windowsPhone ()](#apidoc.element.is_js.windowsPhone)
1.  [function <span class="apidocSignatureSpan">is_js.</span>windowsTablet ()](#apidoc.element.is_js.windowsTablet)
1.  [function <span class="apidocSignatureSpan">is_js.</span>within (n, min, max)](#apidoc.element.is_js.within)
1.  [function <span class="apidocSignatureSpan">is_js.</span>year (date, year)](#apidoc.element.is_js.year)
1.  [function <span class="apidocSignatureSpan">is_js.</span>yesterday (date)](#apidoc.element.is_js.yesterday)
1.  object <span class="apidocSignatureSpan">is_js.</span>all
1.  object <span class="apidocSignatureSpan">is_js.</span>any
1.  object <span class="apidocSignatureSpan">is_js.</span>not
1.  string <span class="apidocSignatureSpan">is_js.</span>VERSION

#### [module is_js.all](#apidoc.module.is_js.all)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>affirmative ()](#apidoc.element.is_js.all.affirmative)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>alphaNumeric ()](#apidoc.element.is_js.all.alphaNumeric)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>arguments ()](#apidoc.element.is_js.all.arguments)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>array ()](#apidoc.element.is_js.all.array)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>boolean ()](#apidoc.element.is_js.all.boolean)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>caPostalCode ()](#apidoc.element.is_js.all.caPostalCode)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>capitalized ()](#apidoc.element.is_js.all.capitalized)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>char ()](#apidoc.element.is_js.all.char)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>creditCard ()](#apidoc.element.is_js.all.creditCard)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>date ()](#apidoc.element.is_js.all.date)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>dateString ()](#apidoc.element.is_js.all.dateString)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>dayLightSavingTime ()](#apidoc.element.is_js.all.dayLightSavingTime)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>decimal ()](#apidoc.element.is_js.all.decimal)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>domNode ()](#apidoc.element.is_js.all.domNode)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>email ()](#apidoc.element.is_js.all.email)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>empty ()](#apidoc.element.is_js.all.empty)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>eppPhone ()](#apidoc.element.is_js.all.eppPhone)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>error ()](#apidoc.element.is_js.all.error)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>even ()](#apidoc.element.is_js.all.even)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>existy ()](#apidoc.element.is_js.all.existy)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>falsy ()](#apidoc.element.is_js.all.falsy)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>finite ()](#apidoc.element.is_js.all.finite)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>function ()](#apidoc.element.is_js.all.function)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>future ()](#apidoc.element.is_js.all.future)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>hexColor ()](#apidoc.element.is_js.all.hexColor)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>hexadecimal ()](#apidoc.element.is_js.all.hexadecimal)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inLastMonth ()](#apidoc.element.is_js.all.inLastMonth)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inLastWeek ()](#apidoc.element.is_js.all.inLastWeek)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inLastYear ()](#apidoc.element.is_js.all.inLastYear)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inNextMonth ()](#apidoc.element.is_js.all.inNextMonth)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inNextWeek ()](#apidoc.element.is_js.all.inNextWeek)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>inNextYear ()](#apidoc.element.is_js.all.inNextYear)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>infinite ()](#apidoc.element.is_js.all.infinite)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>integer ()](#apidoc.element.is_js.all.integer)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>ip ()](#apidoc.element.is_js.all.ip)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>ipv4 ()](#apidoc.element.is_js.all.ipv4)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>ipv6 ()](#apidoc.element.is_js.all.ipv6)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>json ()](#apidoc.element.is_js.all.json)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>leapYear ()](#apidoc.element.is_js.all.leapYear)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>lowerCase ()](#apidoc.element.is_js.all.lowerCase)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>nan ()](#apidoc.element.is_js.all.nan)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>nanpPhone ()](#apidoc.element.is_js.all.nanpPhone)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>negative ()](#apidoc.element.is_js.all.negative)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>null ()](#apidoc.element.is_js.all.null)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>number ()](#apidoc.element.is_js.all.number)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>object ()](#apidoc.element.is_js.all.object)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>odd ()](#apidoc.element.is_js.all.odd)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>palindrome ()](#apidoc.element.is_js.all.palindrome)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>past ()](#apidoc.element.is_js.all.past)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>positive ()](#apidoc.element.is_js.all.positive)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>regexp ()](#apidoc.element.is_js.all.regexp)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>socialSecurityNumber ()](#apidoc.element.is_js.all.socialSecurityNumber)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>sorted ()](#apidoc.element.is_js.all.sorted)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>space ()](#apidoc.element.is_js.all.space)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>string ()](#apidoc.element.is_js.all.string)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>timeString ()](#apidoc.element.is_js.all.timeString)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>today ()](#apidoc.element.is_js.all.today)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>tomorrow ()](#apidoc.element.is_js.all.tomorrow)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>truthy ()](#apidoc.element.is_js.all.truthy)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>ukPostCode ()](#apidoc.element.is_js.all.ukPostCode)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>undefined ()](#apidoc.element.is_js.all.undefined)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>upperCase ()](#apidoc.element.is_js.all.upperCase)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>url ()](#apidoc.element.is_js.all.url)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>usZipCode ()](#apidoc.element.is_js.all.usZipCode)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>weekday ()](#apidoc.element.is_js.all.weekday)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>weekend ()](#apidoc.element.is_js.all.weekend)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>windowObject ()](#apidoc.element.is_js.all.windowObject)
1.  [function <span class="apidocSignatureSpan">is_js.all.</span>yesterday ()](#apidoc.element.is_js.all.yesterday)

#### [module is_js.any](#apidoc.module.is_js.any)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>affirmative ()](#apidoc.element.is_js.any.affirmative)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>alphaNumeric ()](#apidoc.element.is_js.any.alphaNumeric)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>arguments ()](#apidoc.element.is_js.any.arguments)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>array ()](#apidoc.element.is_js.any.array)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>boolean ()](#apidoc.element.is_js.any.boolean)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>caPostalCode ()](#apidoc.element.is_js.any.caPostalCode)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>capitalized ()](#apidoc.element.is_js.any.capitalized)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>char ()](#apidoc.element.is_js.any.char)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>creditCard ()](#apidoc.element.is_js.any.creditCard)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>date ()](#apidoc.element.is_js.any.date)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>dateString ()](#apidoc.element.is_js.any.dateString)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>dayLightSavingTime ()](#apidoc.element.is_js.any.dayLightSavingTime)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>decimal ()](#apidoc.element.is_js.any.decimal)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>domNode ()](#apidoc.element.is_js.any.domNode)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>email ()](#apidoc.element.is_js.any.email)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>empty ()](#apidoc.element.is_js.any.empty)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>eppPhone ()](#apidoc.element.is_js.any.eppPhone)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>error ()](#apidoc.element.is_js.any.error)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>even ()](#apidoc.element.is_js.any.even)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>existy ()](#apidoc.element.is_js.any.existy)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>falsy ()](#apidoc.element.is_js.any.falsy)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>finite ()](#apidoc.element.is_js.any.finite)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>function ()](#apidoc.element.is_js.any.function)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>future ()](#apidoc.element.is_js.any.future)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>hexColor ()](#apidoc.element.is_js.any.hexColor)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>hexadecimal ()](#apidoc.element.is_js.any.hexadecimal)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inLastMonth ()](#apidoc.element.is_js.any.inLastMonth)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inLastWeek ()](#apidoc.element.is_js.any.inLastWeek)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inLastYear ()](#apidoc.element.is_js.any.inLastYear)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inNextMonth ()](#apidoc.element.is_js.any.inNextMonth)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inNextWeek ()](#apidoc.element.is_js.any.inNextWeek)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>inNextYear ()](#apidoc.element.is_js.any.inNextYear)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>infinite ()](#apidoc.element.is_js.any.infinite)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>integer ()](#apidoc.element.is_js.any.integer)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>ip ()](#apidoc.element.is_js.any.ip)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>ipv4 ()](#apidoc.element.is_js.any.ipv4)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>ipv6 ()](#apidoc.element.is_js.any.ipv6)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>json ()](#apidoc.element.is_js.any.json)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>leapYear ()](#apidoc.element.is_js.any.leapYear)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>lowerCase ()](#apidoc.element.is_js.any.lowerCase)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>nan ()](#apidoc.element.is_js.any.nan)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>nanpPhone ()](#apidoc.element.is_js.any.nanpPhone)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>negative ()](#apidoc.element.is_js.any.negative)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>null ()](#apidoc.element.is_js.any.null)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>number ()](#apidoc.element.is_js.any.number)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>object ()](#apidoc.element.is_js.any.object)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>odd ()](#apidoc.element.is_js.any.odd)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>palindrome ()](#apidoc.element.is_js.any.palindrome)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>past ()](#apidoc.element.is_js.any.past)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>positive ()](#apidoc.element.is_js.any.positive)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>regexp ()](#apidoc.element.is_js.any.regexp)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>socialSecurityNumber ()](#apidoc.element.is_js.any.socialSecurityNumber)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>sorted ()](#apidoc.element.is_js.any.sorted)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>space ()](#apidoc.element.is_js.any.space)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>string ()](#apidoc.element.is_js.any.string)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>timeString ()](#apidoc.element.is_js.any.timeString)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>today ()](#apidoc.element.is_js.any.today)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>tomorrow ()](#apidoc.element.is_js.any.tomorrow)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>truthy ()](#apidoc.element.is_js.any.truthy)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>ukPostCode ()](#apidoc.element.is_js.any.ukPostCode)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>undefined ()](#apidoc.element.is_js.any.undefined)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>upperCase ()](#apidoc.element.is_js.any.upperCase)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>url ()](#apidoc.element.is_js.any.url)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>usZipCode ()](#apidoc.element.is_js.any.usZipCode)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>weekday ()](#apidoc.element.is_js.any.weekday)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>weekend ()](#apidoc.element.is_js.any.weekend)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>windowObject ()](#apidoc.element.is_js.any.windowObject)
1.  [function <span class="apidocSignatureSpan">is_js.any.</span>yesterday ()](#apidoc.element.is_js.any.yesterday)

#### [module is_js.not](#apidoc.module.is_js.not)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>above ()](#apidoc.element.is_js.not.above)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>affirmative ()](#apidoc.element.is_js.not.affirmative)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>alphaNumeric ()](#apidoc.element.is_js.not.alphaNumeric)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>android ()](#apidoc.element.is_js.not.android)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>androidPhone ()](#apidoc.element.is_js.not.androidPhone)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>androidTablet ()](#apidoc.element.is_js.not.androidTablet)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>arguments ()](#apidoc.element.is_js.not.arguments)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>array ()](#apidoc.element.is_js.not.array)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>blackberry ()](#apidoc.element.is_js.not.blackberry)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>boolean ()](#apidoc.element.is_js.not.boolean)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>caPostalCode ()](#apidoc.element.is_js.not.caPostalCode)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>capitalized ()](#apidoc.element.is_js.not.capitalized)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>char ()](#apidoc.element.is_js.not.char)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>chrome ()](#apidoc.element.is_js.not.chrome)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>creditCard ()](#apidoc.element.is_js.not.creditCard)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>date ()](#apidoc.element.is_js.not.date)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>dateString ()](#apidoc.element.is_js.not.dateString)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>day ()](#apidoc.element.is_js.not.day)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>dayLightSavingTime ()](#apidoc.element.is_js.not.dayLightSavingTime)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>decimal ()](#apidoc.element.is_js.not.decimal)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>desktop ()](#apidoc.element.is_js.not.desktop)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>domNode ()](#apidoc.element.is_js.not.domNode)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>edge ()](#apidoc.element.is_js.not.edge)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>email ()](#apidoc.element.is_js.not.email)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>empty ()](#apidoc.element.is_js.not.empty)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>endWith ()](#apidoc.element.is_js.not.endWith)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>eppPhone ()](#apidoc.element.is_js.not.eppPhone)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>equal ()](#apidoc.element.is_js.not.equal)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>error ()](#apidoc.element.is_js.not.error)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>even ()](#apidoc.element.is_js.not.even)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>existy ()](#apidoc.element.is_js.not.existy)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>falsy ()](#apidoc.element.is_js.not.falsy)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>finite ()](#apidoc.element.is_js.not.finite)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>firefox ()](#apidoc.element.is_js.not.firefox)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>function ()](#apidoc.element.is_js.not.function)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>future ()](#apidoc.element.is_js.not.future)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>hexColor ()](#apidoc.element.is_js.not.hexColor)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>hexadecimal ()](#apidoc.element.is_js.not.hexadecimal)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ie ()](#apidoc.element.is_js.not.ie)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inArray ()](#apidoc.element.is_js.not.inArray)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inDateRange ()](#apidoc.element.is_js.not.inDateRange)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inLastMonth ()](#apidoc.element.is_js.not.inLastMonth)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inLastWeek ()](#apidoc.element.is_js.not.inLastWeek)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inLastYear ()](#apidoc.element.is_js.not.inLastYear)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inNextMonth ()](#apidoc.element.is_js.not.inNextMonth)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inNextWeek ()](#apidoc.element.is_js.not.inNextWeek)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>inNextYear ()](#apidoc.element.is_js.not.inNextYear)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>include ()](#apidoc.element.is_js.not.include)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>infinite ()](#apidoc.element.is_js.not.infinite)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>integer ()](#apidoc.element.is_js.not.integer)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ios ()](#apidoc.element.is_js.not.ios)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ip ()](#apidoc.element.is_js.not.ip)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ipad ()](#apidoc.element.is_js.not.ipad)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>iphone ()](#apidoc.element.is_js.not.iphone)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ipod ()](#apidoc.element.is_js.not.ipod)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ipv4 ()](#apidoc.element.is_js.not.ipv4)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ipv6 ()](#apidoc.element.is_js.not.ipv6)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>json ()](#apidoc.element.is_js.not.json)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>leapYear ()](#apidoc.element.is_js.not.leapYear)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>linux ()](#apidoc.element.is_js.not.linux)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>lowerCase ()](#apidoc.element.is_js.not.lowerCase)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>mac ()](#apidoc.element.is_js.not.mac)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>mobile ()](#apidoc.element.is_js.not.mobile)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>month ()](#apidoc.element.is_js.not.month)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>nan ()](#apidoc.element.is_js.not.nan)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>nanpPhone ()](#apidoc.element.is_js.not.nanpPhone)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>negative ()](#apidoc.element.is_js.not.negative)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>null ()](#apidoc.element.is_js.not.null)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>number ()](#apidoc.element.is_js.not.number)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>object ()](#apidoc.element.is_js.not.object)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>odd ()](#apidoc.element.is_js.not.odd)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>offline ()](#apidoc.element.is_js.not.offline)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>online ()](#apidoc.element.is_js.not.online)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>opera ()](#apidoc.element.is_js.not.opera)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>palindrome ()](#apidoc.element.is_js.not.palindrome)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>past ()](#apidoc.element.is_js.not.past)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>phantom ()](#apidoc.element.is_js.not.phantom)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>positive ()](#apidoc.element.is_js.not.positive)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>propertyCount ()](#apidoc.element.is_js.not.propertyCount)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>propertyDefined ()](#apidoc.element.is_js.not.propertyDefined)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>quarterOfYear ()](#apidoc.element.is_js.not.quarterOfYear)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>regexp ()](#apidoc.element.is_js.not.regexp)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>safari ()](#apidoc.element.is_js.not.safari)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>sameType ()](#apidoc.element.is_js.not.sameType)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>socialSecurityNumber ()](#apidoc.element.is_js.not.socialSecurityNumber)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>sorted ()](#apidoc.element.is_js.not.sorted)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>space ()](#apidoc.element.is_js.not.space)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>startWith ()](#apidoc.element.is_js.not.startWith)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>string ()](#apidoc.element.is_js.not.string)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>tablet ()](#apidoc.element.is_js.not.tablet)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>timeString ()](#apidoc.element.is_js.not.timeString)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>today ()](#apidoc.element.is_js.not.today)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>tomorrow ()](#apidoc.element.is_js.not.tomorrow)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>touchDevice ()](#apidoc.element.is_js.not.touchDevice)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>truthy ()](#apidoc.element.is_js.not.truthy)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>ukPostCode ()](#apidoc.element.is_js.not.ukPostCode)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>undefined ()](#apidoc.element.is_js.not.undefined)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>under ()](#apidoc.element.is_js.not.under)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>upperCase ()](#apidoc.element.is_js.not.upperCase)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>url ()](#apidoc.element.is_js.not.url)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>usZipCode ()](#apidoc.element.is_js.not.usZipCode)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>weekday ()](#apidoc.element.is_js.not.weekday)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>weekend ()](#apidoc.element.is_js.not.weekend)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>windowObject ()](#apidoc.element.is_js.not.windowObject)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>windows ()](#apidoc.element.is_js.not.windows)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>windowsPhone ()](#apidoc.element.is_js.not.windowsPhone)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>windowsTablet ()](#apidoc.element.is_js.not.windowsTablet)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>within ()](#apidoc.element.is_js.not.within)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>year ()](#apidoc.element.is_js.not.year)
1.  [function <span class="apidocSignatureSpan">is_js.not.</span>yesterday ()](#apidoc.element.is_js.not.yesterday)



# <a name="apidoc.module.is_js"></a>[module is_js](#apidoc.module.is_js)

#### <a name="apidoc.element.is_js.above"></a>[function <span class="apidocSignatureSpan">is_js.</span>above (n, min)](#apidoc.element.is_js.above)
- description and source-code
```javascript
above = function (n, min) {
    return is.all.number(n, min) && n > min;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.negative([40, 42, -43]);
=> false
'''

is.above(value:number, min:number)
---------------------------
####Checks if the given value is above minimum value.
interface: not

'''javascript
is.above(41, 30);
=> true
...
```

#### <a name="apidoc.element.is_js.affirmative"></a>[function <span class="apidocSignatureSpan">is_js.</span>affirmative (value)](#apidoc.element.is_js.affirmative)
- description and source-code
```javascript
affirmative = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.socialSecurityNumber(['017-90-7890', '123']);
=> false
'''

is.affirmative(value:any)
-------------------------
####Checks if the given value matches affirmative regexp.
interfaces: not, all, any

'''javascript
is.affirmative('yes');
=> true
...
```

#### <a name="apidoc.element.is_js.alphaNumeric"></a>[function <span class="apidocSignatureSpan">is_js.</span>alphaNumeric (value)](#apidoc.element.is_js.alphaNumeric)
- description and source-code
```javascript
alphaNumeric = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.creditCard([378282246310005, 123, undefined]);
=> false
'''

is.alphaNumeric(value:any)
--------------------------
####Checks if the given value matches alpha numeric regexp.
interfaces: not, all, any

'''javascript
is.alphaNumeric('alphaNu3er1k');
=> true
...
```

#### <a name="apidoc.element.is_js.android"></a>[function <span class="apidocSignatureSpan">is_js.</span>android ()](#apidoc.element.is_js.android)
- description and source-code
```javascript
android = function () {
    return /android/.test(userAgent);
}
```
- example usage
```shell
...
is.ipod('>=5');
=> true if current version of iPod is greater than or equal to 5

is.not.ipod('<5');
=> true if current version of iPod is not less than 5
'''

is.android()
------------
####Checks if current device has Android.
interface: not

'''javascript
is.android();
=> true if current device has Android OS
...
```

#### <a name="apidoc.element.is_js.androidPhone"></a>[function <span class="apidocSignatureSpan">is_js.</span>androidPhone ()](#apidoc.element.is_js.androidPhone)
- description and source-code
```javascript
androidPhone = function () {
    return /android/.test(userAgent) && /mobile/.test(userAgent);
}
```
- example usage
```shell
...
is.android();
=> true if current device has Android OS

is.not.android();
=> true if current device has not Android OS
'''

is.androidPhone()
-----------------
####Checks if current device is Android phone.
interface: not

'''javascript
is.androidPhone();
=> true if current device is Android phone
...
```

#### <a name="apidoc.element.is_js.androidTablet"></a>[function <span class="apidocSignatureSpan">is_js.</span>androidTablet ()](#apidoc.element.is_js.androidTablet)
- description and source-code
```javascript
androidTablet = function () {
    return /android/.test(userAgent) && !/mobile/.test(userAgent);
}
```
- example usage
```shell
...
is.androidPhone();
=> true if current device is Android phone

is.not.androidPhone();
=> true if current device is not Android phone
'''

is.androidTablet()
------------------
####Checks if current device is Android tablet.
interface: not

'''javascript
is.androidTablet();
=> true if current device is Android tablet
...
```

#### <a name="apidoc.element.is_js.arguments"></a>[function <span class="apidocSignatureSpan">is_js.</span>arguments (value)](#apidoc.element.is_js.arguments)
- description and source-code
```javascript
arguments = function (value) {    // fallback check is for IE
    return toString.call(value) === '[object Arguments]' ||
        (value != null && typeof value === 'object' && 'callee' in value);
}
```
- example usage
```shell
...

####Contributors:
Many thanks to our contributors: https://github.com/arasatasaygin/is.js/graphs/contributors

Type checks
===========

is.arguments(value:any)
-----------------------
####Checks if the given value type is arguments.
interfaces: not, all, any

'''javascript
var getArguments = function() {
return arguments;
...
```

#### <a name="apidoc.element.is_js.array"></a>[function <span class="apidocSignatureSpan">is_js.</span>array ()](#apidoc.element.is_js.array)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.arguments([arguments, 'foo', 'bar']);
=> false
'''

is.array(value:any)
-------------------
####Checks if the given value type is array.
interfaces: not, all, any

'''javascript
is.array(['foo', 'bar', 'baz']);
=> true
...
```

#### <a name="apidoc.element.is_js.blackberry"></a>[function <span class="apidocSignatureSpan">is_js.</span>blackberry ()](#apidoc.element.is_js.blackberry)
- description and source-code
```javascript
blackberry = function () {
    return /blackberry/.test(userAgent) || /bb10/.test(userAgent);
}
```
- example usage
```shell
...
is.androidTablet();
=> true if current device is Android tablet

is.not.androidTablet();
=> true if current device is not Android tablet
'''

is.blackberry()
---------------
####Checks if current device is Blackberry.
interface: not

'''javascript
is.blackberry();
=> true if current device is Blackberry
...
```

#### <a name="apidoc.element.is_js.boolean"></a>[function <span class="apidocSignatureSpan">is_js.</span>boolean (value)](#apidoc.element.is_js.boolean)
- description and source-code
```javascript
boolean = function (value) {
    return value === true || value === false || toString.call(value) === '[object Boolean]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.array([[1, 2], 'foo', 'bar']);
=> false
'''

is.boolean(value:any)
---------------------
####Checks if the given value type is boolean.
interfaces: not, all, any

'''javascript
is.boolean(true);
=> true
...
```

#### <a name="apidoc.element.is_js.caPostalCode"></a>[function <span class="apidocSignatureSpan">is_js.</span>caPostalCode (value)](#apidoc.element.is_js.caPostalCode)
- description and source-code
```javascript
caPostalCode = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.usZipCode(['02201-1020', '123']);
=> false
'''

is.caPostalCode(value:any)
--------------------------
####Checks if the given value matches Canada postal code regexp.
interfaces: not, all, any

'''javascript
is.caPostalCode('L8V3Y1');
=> true
...
```

#### <a name="apidoc.element.is_js.capitalized"></a>[function <span class="apidocSignatureSpan">is_js.</span>capitalized (string)](#apidoc.element.is_js.capitalized)
- description and source-code
```javascript
capitalized = function (string) {
    if (is.not.string(string)) {
        return false;
    }
    var words = string.split(' ');
    for (var i = 0; i < words.length; i++) {
        var word = words[i];
        if (word.length) {
            var chr = word.charAt(0);
            if (chr !== chr.toUpperCase()) {
                return false;
            }
        }
    }
    return true;
}
```
- example usage
```shell
...
is.not.endWith('nope not that', 'not');
=> true

is.endWith('yeap that one', 'one');
=> true
'''

is.capitalized(value:string)
---------------------------------------------
####Checks if the given string is capitalized.
interfaces: not, all, any

'''javascript
is.capitalized('Yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.char"></a>[function <span class="apidocSignatureSpan">is_js.</span>char (value)](#apidoc.element.is_js.char)
- description and source-code
```javascript
char = function (value) {
    return is.string(value) && value.length === 1;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.string([{}, 'foo']);
=> false
'''

is.char(value:any)
--------------------
####Checks if the given value type is char.
interfaces: not, all, any

'''javascript
is.char('f');
=> true
...
```

#### <a name="apidoc.element.is_js.chrome"></a>[function <span class="apidocSignatureSpan">is_js.</span>chrome (range)](#apidoc.element.is_js.chrome)
- description and source-code
```javascript
chrome = function (range) {
    var match = /google inc/.test(vendor) ? userAgent.match(/(?:chrome|crios)\/(\d+)/) : null;
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.ie('>=10');
=> true if current version of ie is greater than or equal to 10

is.not.ie('<9');
=> true if current version of ie is not less than 9
'''

is.chrome(range:number|string)
-----------
####Checks if current browser is chrome. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.chrome();
=> true if current browser is chrome
...
```

#### <a name="apidoc.element.is_js.creditCard"></a>[function <span class="apidocSignatureSpan">is_js.</span>creditCard (value)](#apidoc.element.is_js.creditCard)
- description and source-code
```javascript
creditCard = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.email(['test@test.com', 'foo', undefined]);
=> false
'''

is.creditCard(value:any)
------------------------
####Checks if the given value matches credit card regexp.
interfaces: not, all, any

'''javascript
is.creditCard(378282246310005);
=> true
...
```

#### <a name="apidoc.element.is_js.date"></a>[function <span class="apidocSignatureSpan">is_js.</span>date (value)](#apidoc.element.is_js.date)
- description and source-code
```javascript
date = function (value) {
    return toString.call(value) === '[object Date]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.boolean([true, 'foo', 'bar']);
=> false
'''

is.date(value:any)
------------------
####Checks if the given value type is date.
interfaces: not, all, any

'''javascript
is.date(new Date());
=> true
...
```

#### <a name="apidoc.element.is_js.dateString"></a>[function <span class="apidocSignatureSpan">is_js.</span>dateString (value)](#apidoc.element.is_js.dateString)
- description and source-code
```javascript
dateString = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.timeString(['13:45:30', '90:90:90']);
=> false
'''

is.dateString(value:any)
------------------------
####Checks if the given value matches date string regexp.
interfaces: not, all, any

'''javascript
is.dateString('11/11/2011');
=> true
...
```

#### <a name="apidoc.element.is_js.day"></a>[function <span class="apidocSignatureSpan">is_js.</span>day (date, day)](#apidoc.element.is_js.day)
- description and source-code
```javascript
day = function (date, day) {
    return is.date(date) && day.toLowerCase() === days[date.getDay()];
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.future([yesterday, tomorrow]);
=> false
'''

is.day(value:date, day:string)
-------------------------------
####Checks if the given date objects' day equal given dayString parameter.
interface: not

'''javascript
var mondayObj = new Date('01/26/2015');
var tuesdayObj = new Date('01/27/2015');
...
```

#### <a name="apidoc.element.is_js.dayLightSavingTime"></a>[function <span class="apidocSignatureSpan">is_js.</span>dayLightSavingTime (date)](#apidoc.element.is_js.dayLightSavingTime)
- description and source-code
```javascript
dayLightSavingTime = function (date) {
    var january = new Date(date.getFullYear(), 0, 1);
    var july = new Date(date.getFullYear(), 6, 1);
    var stdTimezoneOffset = Math.max(january.getTimezoneOffset(), july.getTimezoneOffset());
    return date.getTimezoneOffset() < stdTimezoneOffset;
}
```
- example usage
```shell
...
is.quarterOfYear(secondQuarter, 1);
=> false

is.not.quarterOfYear(secondQuarter, 1);
=> true
'''

is.dayLightSavingTime(value:date)
--------------------------------------------------
####Checks if the given date is in daylight saving time.
interface: not

'''javascript
// For Turkey Time Zone
var january1 = new Date('01/01/2015');
...
```

#### <a name="apidoc.element.is_js.decimal"></a>[function <span class="apidocSignatureSpan">is_js.</span>decimal (n)](#apidoc.element.is_js.decimal)
- description and source-code
```javascript
decimal = function (n) {
    return is.number(n) && n % 1 !== 0;
}
```
- example usage
```shell
...
is.within(30, 20, 40);
=> true

is.not.within(40, 30, 35);
=> true
'''

is.decimal(value:number)
------------------------
####Checks if the given value is decimal.
interfaces: not, all, any

'''javascript
is.decimal(41.5);
=> true
...
```

#### <a name="apidoc.element.is_js.desktop"></a>[function <span class="apidocSignatureSpan">is_js.</span>desktop ()](#apidoc.element.is_js.desktop)
- description and source-code
```javascript
desktop = function () {
    return is.not.mobile() && is.not.tablet();
}
```
- example usage
```shell
...
is.linux();
=> true if current OS is linux

is.not.linux();
=> true if current OS is not linux
'''

is.desktop()
------------
####Checks if current device is desktop.
interface: not

'''javascript
is.desktop();
=> true if current device is desktop
...
```

#### <a name="apidoc.element.is_js.domNode"></a>[function <span class="apidocSignatureSpan">is_js.</span>domNode (object)](#apidoc.element.is_js.domNode)
- description and source-code
```javascript
domNode = function (object) {
    return is.object(object) && object.nodeType > 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.date([new Date(), 'foo', 'bar']);
=> false
'''

is.domNode(value:any)
-----------------------------
####Checks if the given object is a dom node.
interfaces: not, all, any

'''javascript
var obj = document.createElement('div');
is.domNode(obj);
...
```

#### <a name="apidoc.element.is_js.edge"></a>[function <span class="apidocSignatureSpan">is_js.</span>edge (range)](#apidoc.element.is_js.edge)
- description and source-code
```javascript
edge = function (range) {
    var match = userAgent.match(/edge\/(\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.firefox('>=40');
=> true if current version of firefox is greater than or equal to 40

is.not.firefox('<30');
=> true if current version of firefox is not less than 30
'''

is.edge(range:number|string)
------------
####Checks if current browser is edge. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.edge();
=> true if current browser is edge
...
```

#### <a name="apidoc.element.is_js.email"></a>[function <span class="apidocSignatureSpan">is_js.</span>email (value)](#apidoc.element.is_js.email)
- description and source-code
```javascript
email = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.url(['http://www.test.com', 'foo', undefined]);
=> false
'''

is.email(value:any)
-------------------
####Checks if the given value matches email regexp.
interfaces: not, all, any

'''javascript
is.email('test@test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.empty"></a>[function <span class="apidocSignatureSpan">is_js.</span>empty (value)](#apidoc.element.is_js.empty)
- description and source-code
```javascript
empty = function (value) {
    if (is.object(value)) {
        var length = Object.getOwnPropertyNames(value).length;
        if (length === 0 || (length === 1 && is.array(value)) ||
                (length === 2 && is.arguments(value))) {
            return true;
        }
        return false;
    }
    return value === '';
}
```
- example usage
```shell
...
is.all.windowObject([window, {nope: 'nope'}]);
=> false
'''

Presence checks
===============

is.empty(value:array|object|string)
-----------------------------------
####Checks if the given value is empty.
interfaces: not, all, any

'''javascript
is.empty({});
=> true
...
```

#### <a name="apidoc.element.is_js.endWith"></a>[function <span class="apidocSignatureSpan">is_js.</span>endWith (string, target)](#apidoc.element.is_js.endWith)
- description and source-code
```javascript
endWith = function (string, target) {
    if (is.not.string(string)) {
        return false;
    }
    target += '';
    var position = string.length - target.length;
    return position >= 0 && string.indexOf(target, position) === position;
}
```
- example usage
```shell
...
is.startWith('nope', 'ye');
=> false

is.not.startWith('nope not that', 'not');
=> true
'''

is.endWith(value:string, target:string)
-----------------------------------------
####Checks if the given string ends with substring.
interfaces: not

'''javascript
is.endWith('yeap', 'ap');
=> true
...
```

#### <a name="apidoc.element.is_js.eppPhone"></a>[function <span class="apidocSignatureSpan">is_js.</span>eppPhone (value)](#apidoc.element.is_js.eppPhone)
- description and source-code
```javascript
eppPhone = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nanpPhone(['609-555-0175', '123']);
=> false
'''

is.eppPhone(value:any)
----------------------
####Checks if the given value matches extensible provisioning protocol phone regexp.
interfaces: not, all, any

'''javascript
is.eppPhone('+90.2322456789');
=> true
...
```

#### <a name="apidoc.element.is_js.equal"></a>[function <span class="apidocSignatureSpan">is_js.</span>equal (value, other)](#apidoc.element.is_js.equal)
- description and source-code
```javascript
equal = function (value, other) {
    // check 0 and -0 equity with Infinity and -Infinity
    if (is.all.number(value, other)) {
        return value === other && 1 / value === 1 / other;
    }
    // check regexes as strings too
    if (is.all.string(value, other) || is.all.regexp(value, other)) {
        return '' + value === '' + other;
    }
    if (is.all.boolean(value, other)) {
        return value === other;
    }
    return false;
}
```
- example usage
```shell
...
is.all.palindrome(['Nope', 'testset']);
=> false
'''

Arithmetic checks
=================

is.equal(value:any, other:any)
------------------------------
####Checks if the given values are equal.
interfaces: not

'''javascript
is.equal(42, 40 + 2);
=> true
...
```

#### <a name="apidoc.element.is_js.error"></a>[function <span class="apidocSignatureSpan">is_js.</span>error (value)](#apidoc.element.is_js.error)
- description and source-code
```javascript
error = function (value) {
    return toString.call(value) === '[object Error]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.domNode([obj, {nope: 'nope'}]);
=> false
'''

is.error(value:any)
-------------------
####Checks if the given value type is error.
interfaces: not, all, any

'''javascript
is.error(new Error());
=> true
...
```

#### <a name="apidoc.element.is_js.even"></a>[function <span class="apidocSignatureSpan">is_js.</span>even (n)](#apidoc.element.is_js.even)
- description and source-code
```javascript
even = function (n) {
    return is.number(n) && n % 2 === 0;
}
```
- example usage
```shell
...
is.equal(true, true);
=> true

is.not.equal('yeap', 'nope');
=> true
'''

is.even(value:number)
---------------------
####Checks if the given value is even.
interfaces: not, all, any

'''javascript
is.even(42);
=> true
...
```

#### <a name="apidoc.element.is_js.existy"></a>[function <span class="apidocSignatureSpan">is_js.</span>existy (value)](#apidoc.element.is_js.existy)
- description and source-code
```javascript
existy = function (value) {
    return value != null;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.empty([{}, 'foo']);
=> false
'''

is.existy(value:any)
--------------------
####Checks if the given value is existy. (not null or undefined)
interfaces: not, all, any

'''javascript
is.existy({});
=> true
...
```

#### <a name="apidoc.element.is_js.falsy"></a>[function <span class="apidocSignatureSpan">is_js.</span>falsy (value)](#apidoc.element.is_js.falsy)
- description and source-code
```javascript
falsy = function (value) {
    return !value;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.truthy([{}, true]);
=> true
'''

is.falsy(value:any)
-------------------
####Checks if the given value is falsy.
interfaces: not, all, any

'''javascript
is.falsy(false);
=> true
...
```

#### <a name="apidoc.element.is_js.finite"></a>[function <span class="apidocSignatureSpan">is_js.</span>finite ()](#apidoc.element.is_js.finite)
- description and source-code
```javascript
function isFinite() { [native code] }
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.integer([40, 42.5, -43]);
=> false
'''

is.finite(value:number)
-----------------------
####Checks if the given value is finite.
interfaces: not, all, any

'''javascript
is.finite(41);
=> true
...
```

#### <a name="apidoc.element.is_js.firefox"></a>[function <span class="apidocSignatureSpan">is_js.</span>firefox (range)](#apidoc.element.is_js.firefox)
- description and source-code
```javascript
firefox = function (range) {
    var match = userAgent.match(/(?:firefox|fxios)\/(\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.chrome('>=40');
=> true if current version of chrome is greater than or equal to 40

is.not.chrome('<30');
=> true if current version of chrome is not less than 30
'''

is.firefox(range:number|string)
------------
####Checks if current browser is firefox. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.firefox();
=> true if current browser is firefox
...
```

#### <a name="apidoc.element.is_js.function"></a>[function <span class="apidocSignatureSpan">is_js.</span>function (value)](#apidoc.element.is_js.function)
- description and source-code
```javascript
function = function (value) {    // fallback check is for IE
    return toString.call(value) === '[object Function]' || typeof value === 'function';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.error([new Error(), 'foo', 'bar']);
=> false
'''

is.function(value:any)
----------------------
####Checks if the given value type is function.
interfaces: not, all, any

'''javascript
is.function(toString);
=> true
...
```

#### <a name="apidoc.element.is_js.future"></a>[function <span class="apidocSignatureSpan">is_js.</span>future (date)](#apidoc.element.is_js.future)
- description and source-code
```javascript
future = function (date) {
    var now = new Date();
    return is.date(date) && date.getTime() > now.getTime();
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.past([yesterday, tomorrow]);
=> false
'''

is.future(value:date)
-----------------------
####Checks if the given date object indicate future.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.hexColor"></a>[function <span class="apidocSignatureSpan">is_js.</span>hexColor (value)](#apidoc.element.is_js.hexColor)
- description and source-code
```javascript
hexColor = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.hexadecimal(['fff', '333', 'f50']);
=> true
'''

is.hexColor(value:any)
-------------------------
####Checks if the given value matches hexcolor regexp.
interfaces: not, all, any

'''javascript
is.hexColor('#333');
=> true
...
```

#### <a name="apidoc.element.is_js.hexadecimal"></a>[function <span class="apidocSignatureSpan">is_js.</span>hexadecimal (value)](#apidoc.element.is_js.hexadecimal)
- description and source-code
```javascript
hexadecimal = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.affirmative(['yes', 'y', 'true', 't', 'ok', 'okay']);
=> true
'''

is.hexadecimal(value:any)
-------------------------
####Checks if the given value matches hexadecimal regexp.
interfaces: not, all, any

'''javascript
is.hexadecimal('f0f0f0');
=> true
...
```

#### <a name="apidoc.element.is_js.ie"></a>[function <span class="apidocSignatureSpan">is_js.</span>ie (range)](#apidoc.element.is_js.ie)
- description and source-code
```javascript
ie = function (range) {
    var match = userAgent.match(/(?:msie |trident.+?; rv:)(\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
=> false
'''

Environment checks
==================
####Environment checks are not available as node module.

is.ie(range:number|string)
-------------------
####Checks if current browser is ie. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.ie();
=> true if current browser is ie
...
```

#### <a name="apidoc.element.is_js.inArray"></a>[function <span class="apidocSignatureSpan">is_js.</span>inArray (value, array)](#apidoc.element.is_js.inArray)
- description and source-code
```javascript
inArray = function (value, array) {
    if (is.not.array(array)) {
        return false;
    }
    for (var i = 0; i < array.length; i++) {
        if (array[i] === value) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.not.propertyDefined({}, 'nope');
=> true
'''

Array checks
============

is.inArray(value:any, array)
---------------------
####Checks if the given item is in array?
interface: not
'''javascript
is.inArray(2, [1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.inDateRange"></a>[function <span class="apidocSignatureSpan">is_js.</span>inDateRange (date, start, end)](#apidoc.element.is_js.inDateRange)
- description and source-code
```javascript
inDateRange = function (date, start, end) {
    if (is.not.date(date) || is.not.date(start) || is.not.date(end)) {
        return false;
    }
    var stamp = date.getTime();
    return stamp > start.getTime() && stamp < end.getTime();
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekday([sunday, saturday, monday]);
=> false
'''

is.inDateRange(value:date, start:date, end:date)
----------------------------------------------------
####Checks if date is within given range.
interface: not

'''javascript
var saturday = new Date('01/24/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.inLastMonth"></a>[function <span class="apidocSignatureSpan">is_js.</span>inLastMonth (date)](#apidoc.element.is_js.inLastMonth)
- description and source-code
```javascript
inLastMonth = function (date) {
    return is.inDateRange(date, new Date(new Date().setMonth(new Date().getMonth() - 1)), new Date());
}
```
- example usage
```shell
...
is.inLastWeek(nineDaysAgo);
=> false

is.not.inLastWeek(nineDaysAgo);
=> true
'''

is.inLastMonth(value:date)
----------------------------
####Checks if the given date is between now and a month ago.
interface: not

'''javascript
var tenDaysAgo = new Date(new Date().setDate(new Date().getDate() - 10));
var fortyDaysAgo = new Date(new Date().setDate(new Date().getDate() - 40));
...
```

#### <a name="apidoc.element.is_js.inLastWeek"></a>[function <span class="apidocSignatureSpan">is_js.</span>inLastWeek (date)](#apidoc.element.is_js.inLastWeek)
- description and source-code
```javascript
inLastWeek = function (date) {
    return is.inDateRange(date, new Date(new Date().setDate(new Date().getDate() - 7)), new Date());
}
```
- example usage
```shell
...
is.inDateRange(saturday, sunday, monday);
=> false

is.not.inDateRange(saturday, sunday, monday);
=> true
'''

is.inLastWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days ago.
interface: not

'''javascript
var twoDaysAgo = new Date(new Date().setDate(new Date().getDate() - 2));
var nineDaysAgo = new Date(new Date().setDate(new Date().getDate() - 9));
...
```

#### <a name="apidoc.element.is_js.inLastYear"></a>[function <span class="apidocSignatureSpan">is_js.</span>inLastYear (date)](#apidoc.element.is_js.inLastYear)
- description and source-code
```javascript
inLastYear = function (date) {
    return is.inDateRange(date, new Date(new Date().setFullYear(new Date().getFullYear() - 1)), new Date());
}
```
- example usage
```shell
...
is.inLastMonth(fortyDaysAgo);
=> false

is.not.inLastMonth(fortyDaysAgo);
=> true
'''

is.inLastYear(value:date)
---------------------------
####Checks if the given date is between now and a year ago.
interface: not

'''javascript
var twoMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 2));
var thirteenMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 13));
...
```

#### <a name="apidoc.element.is_js.inNextMonth"></a>[function <span class="apidocSignatureSpan">is_js.</span>inNextMonth (date)](#apidoc.element.is_js.inNextMonth)
- description and source-code
```javascript
inNextMonth = function (date) {
    return is.inDateRange(date, new Date(), new Date(new Date().setMonth(new Date().getMonth() + 1)));
}
```
- example usage
```shell
...
is.inNextWeek(nineDaysLater);
=> false

is.not.inNextWeek(nineDaysLater);
=> true
'''

is.inNextMonth(value:date)
----------------------------
####Checks if the given date is between now and a month later.
interface: not

'''javascript
var tenDaysLater = new Date(new Date().setDate(new Date().getDate() + 10));
var fortyDaysLater = new Date(new Date().setDate(new Date().getDate() + 40));
...
```

#### <a name="apidoc.element.is_js.inNextWeek"></a>[function <span class="apidocSignatureSpan">is_js.</span>inNextWeek (date)](#apidoc.element.is_js.inNextWeek)
- description and source-code
```javascript
inNextWeek = function (date) {
    return is.inDateRange(date, new Date(), new Date(new Date().setDate(new Date().getDate() + 7)));
}
```
- example usage
```shell
...
is.inLastYear(thirteenMonthsAgo);
=> false

is.not.inLastYear(thirteenMonthsAgo);
=> true
'''

is.inNextWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days later.
interface: not

'''javascript
var twoDaysLater = new Date(new Date().setDate(new Date().getDate() + 2));
var nineDaysLater = new Date(new Date().setDate(new Date().getDate() + 9));
...
```

#### <a name="apidoc.element.is_js.inNextYear"></a>[function <span class="apidocSignatureSpan">is_js.</span>inNextYear (date)](#apidoc.element.is_js.inNextYear)
- description and source-code
```javascript
inNextYear = function (date) {
    return is.inDateRange(date, new Date(), new Date(new Date().setFullYear(new Date().getFullYear() + 1)));
}
```
- example usage
```shell
...
is.inNextMonth(fortyDaysLater);
=> false

is.not.inNextMonth(fortyDaysLater);
=> true
'''

is.inNextYear(value:date)
---------------------------
####Checks if the given date is between now and a year later.
interface: not

'''javascript
var twoMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 2));
var thirteenMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 13));
...
```

#### <a name="apidoc.element.is_js.include"></a>[function <span class="apidocSignatureSpan">is_js.</span>include (string, target)](#apidoc.element.is_js.include)
- description and source-code
```javascript
include = function (string, target) {
    return string.indexOf(target) > -1;
}
```
- example usage
```shell
...
is.all.ipv6(['2001:DB8:0:0:1::1', '1.2.3']);
=> false
'''

String checks
=============

is.include(value:string, target:string)
-----------------------------------------
####Checks if the given string contains a substring.
interface: not

'''javascript
is.include('Some text goes here', 'text');
=> true
...
```

#### <a name="apidoc.element.is_js.infinite"></a>[function <span class="apidocSignatureSpan">is_js.</span>infinite (n)](#apidoc.element.is_js.infinite)
- description and source-code
```javascript
infinite = function (n) {
    return n === Infinity || n === -Infinity;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.finite([Infinity, -Infinity, 42.5]);
=> false
'''

is.infinite(value:number)
-------------------------
####Checks if the given value is infinite.
interfaces: not, all, any

'''javascript
is.infinite(Infinity);
=> true
...
```

#### <a name="apidoc.element.is_js.integer"></a>[function <span class="apidocSignatureSpan">is_js.</span>integer (n)](#apidoc.element.is_js.integer)
- description and source-code
```javascript
integer = function (n) {
    return is.number(n) && n % 1 === 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.decimal([40, 42.5, -43]);
=> false
'''

is.integer(value:number)
------------------------
####Checks if the given value is integer.
interfaces: not, all, any

'''javascript
is.integer(41);
=> true
...
```

#### <a name="apidoc.element.is_js.ios"></a>[function <span class="apidocSignatureSpan">is_js.</span>ios ()](#apidoc.element.is_js.ios)
- description and source-code
```javascript
ios = function () {
    return is.iphone() || is.ipad() || is.ipod();
}
```
- example usage
```shell
...
is.phantom('>=1');
=> true if current version of phantomjs is greater than or equal to 1

is.not.phantom('<2');
=> true if current version of phantomjs is not less than 2
'''

is.ios()
--------
####Checks if current device has ios.
interface: not

'''javascript
is.ios();
=> true if current device is iPhone, iPad or iPod
...
```

#### <a name="apidoc.element.is_js.ip"></a>[function <span class="apidocSignatureSpan">is_js.</span>ip (value)](#apidoc.element.is_js.ip)
- description and source-code
```javascript
ip = function (value) {
    return is.ipv4(value) || is.ipv6(value);
}
```
- example usage
```shell
...
=> false

// 'all' and 'any' interfaces can also take array parameter
is.all.hexColor(['fff', '333', 'f50']);
=> true
'''

is.ip(value:any)
-------------------------
####Checks if the given value matches ip regexp
interfaces: not, all, any

'''javascript
is.ip('198.156.23.5');
=> true
...
```

#### <a name="apidoc.element.is_js.ipad"></a>[function <span class="apidocSignatureSpan">is_js.</span>ipad (range)](#apidoc.element.is_js.ipad)
- description and source-code
```javascript
ipad = function (range) {
    var match = userAgent.match(/ipad.+?os (\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.iphone('>=7');
=> true if current version of iPhone is greater than or equal to 7

is.not.iphone('<8');
=> true if current version of iPhone is not less than 8
'''

is.ipad(range:number|string)
---------
####Checks if current device is iPad.
interface: not

'''javascript
is.ipad();
=> true if current device is iPad
...
```

#### <a name="apidoc.element.is_js.iphone"></a>[function <span class="apidocSignatureSpan">is_js.</span>iphone (range)](#apidoc.element.is_js.iphone)
- description and source-code
```javascript
iphone = function (range) {
    // original iPhone doesn't have the os portion of the UA
    var match = userAgent.match(/iphone(?:.+?os (\d+))?/);
    return match !== null && compareVersion(match[1] || 1, range);
}
```
- example usage
```shell
...
is.ios();
=> true if current device is iPhone, iPad or iPod

is.not.ios();
=> true if current device is not iPhone, iPad or iPod
'''

is.iphone(range:number|string)
-----------
####Checks if current device is iPhone. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.iphone();
=> true if current device is iPhone
...
```

#### <a name="apidoc.element.is_js.ipod"></a>[function <span class="apidocSignatureSpan">is_js.</span>ipod (range)](#apidoc.element.is_js.ipod)
- description and source-code
```javascript
ipod = function (range) {
    var match = userAgent.match(/ipod.+?os (\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.ipad('>=7');
=> true if current version of iPad is greater than or equal to 7

is.not.ipad('<8');
=> true if current version of iPad is not less than 8
'''

is.ipod(range:number|string)
---------
####Checks if current device is iPod.
interface: not

'''javascript
is.ipod();
=> true if current device is iPod
...
```

#### <a name="apidoc.element.is_js.ipv4"></a>[function <span class="apidocSignatureSpan">is_js.</span>ipv4 (value)](#apidoc.element.is_js.ipv4)
- description and source-code
```javascript
ipv4 = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ip(['123.123.23.12', 'A:B:C:D:E:F:0:0']);
=> true
'''

is.ipv4(value:any)
-------------------------
####Checks if the given value matches ipv4 regexp
interfaces: not, all, any

'''javascript
is.ipv4('198.12.3.142');
=> true
...
```

#### <a name="apidoc.element.is_js.ipv6"></a>[function <span class="apidocSignatureSpan">is_js.</span>ipv6 (value)](#apidoc.element.is_js.ipv6)
- description and source-code
```javascript
ipv6 = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.ipv4(['198.12.3.142', '1.2.3']);
=> false

'''

is.ipv6(value:any)
-------------------------
####Checks if the given value matches ipv6 regexp
interfaces: not, all, any

'''javascript
is.ipv6('2001:DB8:0:0:1::1');
=> true
...
```

#### <a name="apidoc.element.is_js.json"></a>[function <span class="apidocSignatureSpan">is_js.</span>json (value)](#apidoc.element.is_js.json)
- description and source-code
```javascript
json = function (value) {
    return toString.call(value) === '[object Object]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.object([{}, new Object()]);
=> true
'''

is.json(value:any)
--------------------
####Checks if the given value type is pure json object.
interfaces: not, all, any

'''javascript
is.json({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.leapYear"></a>[function <span class="apidocSignatureSpan">is_js.</span>leapYear (year)](#apidoc.element.is_js.leapYear)
- description and source-code
```javascript
leapYear = function (year) {
    return is.number(year) && ((year % 4 === 0 && year % 100 !== 0) || year % 400 === 0);
}
```
- example usage
```shell
...
is.year(year2016, 2015);
=> false

is.not.year(year2016, 2015);
=> true
'''

is.leapYear(value:number)
---------------------------------
####Checks if the given year number is a leap year
interfaces: not, all, any

'''javascript
is.leapYear(2016);
=> true
...
```

#### <a name="apidoc.element.is_js.linux"></a>[function <span class="apidocSignatureSpan">is_js.</span>linux ()](#apidoc.element.is_js.linux)
- description and source-code
```javascript
linux = function () {
    return /linux/.test(appVersion);
}
```
- example usage
```shell
...
is.mac();
=> true if current OS is Mac OS X

is.not.mac();
=> true if current OS is not Mac OS X
'''

is.linux()
----------
####Checks if current OS is linux.
interface: not

'''javascript
is.linux();
=> true if current OS is linux
...
```

#### <a name="apidoc.element.is_js.lowerCase"></a>[function <span class="apidocSignatureSpan">is_js.</span>lowerCase (string)](#apidoc.element.is_js.lowerCase)
- description and source-code
```javascript
lowerCase = function (string) {
    return is.string(string) && string === string.toLowerCase();
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.upperCase(['YEAP', 'ALL UPPERCASE']);
=> true
'''


is.lowerCase(value:string)
--------------------------
####Checks if the given string is lowercase.
interfaces: not, all, any

'''javascript
is.lowerCase('yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.mac"></a>[function <span class="apidocSignatureSpan">is_js.</span>mac ()](#apidoc.element.is_js.mac)
- description and source-code
```javascript
mac = function () {
    return /mac/.test(appVersion);
}
```
- example usage
```shell
...
is.windows();
=> true if current OS is Windows

is.not.windows();
=> true if current OS is not Windows
'''

is.mac()
--------
####Checks if current OS is Mac OS X.
interface: not

'''javascript
is.mac();
=> true if current OS is Mac OS X
...
```

#### <a name="apidoc.element.is_js.mobile"></a>[function <span class="apidocSignatureSpan">is_js.</span>mobile ()](#apidoc.element.is_js.mobile)
- description and source-code
```javascript
mobile = function () {
    return is.iphone() || is.ipod() || is.androidPhone() || is.blackberry() || is.windowsPhone();
}
```
- example usage
```shell
...
is.desktop();
=> true if current device is desktop

is.not.desktop();
=> true if current device is not desktop
'''

is.mobile()
-----------
####Checks if current device is mobile.
interface: not
iPhone, iPod, Android Phone, Windows Phone, Blackberry.
'''javascript

is.mobile();
...
```

#### <a name="apidoc.element.is_js.month"></a>[function <span class="apidocSignatureSpan">is_js.</span>month (date, month)](#apidoc.element.is_js.month)
- description and source-code
```javascript
month = function (date, month) {
    return is.date(date) && month.toLowerCase() === months[date.getMonth()];
}
```
- example usage
```shell
...
is.day(mondayObj, 'tuesday');
=> false

is.not.day(mondayObj, 'tuesday');
=> true
'''

is.month(value:date, month:string)
-----------------------------------
####Checks if the given date objects' month equal given monthString parameter.
interface: not

'''javascript
var januaryObj = new Date('01/26/2015');
var februaryObj = new Date('02/26/2015');
...
```

#### <a name="apidoc.element.is_js.nan"></a>[function <span class="apidocSignatureSpan">is_js.</span>nan (value)](#apidoc.element.is_js.nan)
- description and source-code
```javascript
nan = function (value) {    // NaN is number :) Also it is the only value which does not equal itself
    return value !== value;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.function([toString, 'foo', 'bar']);
=> false
'''

is.nan(value:any)
-----------------
####Checks if the given value type is NaN.
interfaces: not, all, any

'''javascript
is.nan(NaN);
=> true
...
```

#### <a name="apidoc.element.is_js.nanpPhone"></a>[function <span class="apidocSignatureSpan">is_js.</span>nanpPhone (value)](#apidoc.element.is_js.nanpPhone)
- description and source-code
```javascript
nanpPhone = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ukPostCode(['B184BJ', '123']);
=> false
'''

is.nanpPhone(value:any)
-----------------------
####Checks if the given value matches North American numbering plan phone regexp.
interfaces: not, all, any

'''javascript
is.nanpPhone('609-555-0175');
=> true
...
```

#### <a name="apidoc.element.is_js.negative"></a>[function <span class="apidocSignatureSpan">is_js.</span>negative (n)](#apidoc.element.is_js.negative)
- description and source-code
```javascript
negative = function (n) {
    return is.number(n) && n < 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.positive([40, 42, -43]);
=> false
'''

is.negative(value:number)
-------------------------
####Checks if the given value is negative.
interfaces: not, all, any

'''javascript
is.negative(-41);
=> true
...
```

#### <a name="apidoc.element.is_js.null"></a>[function <span class="apidocSignatureSpan">is_js.</span>null (value)](#apidoc.element.is_js.null)
- description and source-code
```javascript
null = function (value) {
    return value === null;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nan([NaN, 'foo', 1]);
=> false
'''

is.null(value:any)
------------------
####Checks if the given value type is null.
interfaces: not, all, any

'''javascript
is.null(null);
=> true
...
```

#### <a name="apidoc.element.is_js.number"></a>[function <span class="apidocSignatureSpan">is_js.</span>number (value)](#apidoc.element.is_js.number)
- description and source-code
```javascript
number = function (value) {
    return is.not.nan(value) && toString.call(value) === '[object Number]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.null([null, 'foo', 1]);
=> false
'''

is.number(value:any)
--------------------
####Checks if the given value type is number.
interfaces: not, all, any

'''javascript
is.number(42);
=> true
...
```

#### <a name="apidoc.element.is_js.object"></a>[function <span class="apidocSignatureSpan">is_js.</span>object (value)](#apidoc.element.is_js.object)
- description and source-code
```javascript
object = function (value) {
    return Object(value) === value;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.number([42, 'foo', 1]);
=> false
'''

is.object(value:any)
--------------------
####Checks if the given value type is object.
interfaces: not, all, any

'''javascript
is.object({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.odd"></a>[function <span class="apidocSignatureSpan">is_js.</span>odd (n)](#apidoc.element.is_js.odd)
- description and source-code
```javascript
odd = function (n) {
    return is.number(n) && n % 2 === 1;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.even([40, 42, 43]);
=> false
'''

is.odd(value:number)
--------------------
####Checks if the given value is odd.
interfaces: not, all, any

'''javascript
is.odd(41);
=> true
...
```

#### <a name="apidoc.element.is_js.offline"></a>[function <span class="apidocSignatureSpan">is_js.</span>offline ()](#apidoc.element.is_js.offline)
- description and source-code
```javascript
offline = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.online();
=> true if current device is online

is.not.online();
=> true if current device is not online
'''

is.offline()
------------
####Checks if current device is offline.
interface: not

'''javascript
is.offline();
=> true if current device is offline
...
```

#### <a name="apidoc.element.is_js.online"></a>[function <span class="apidocSignatureSpan">is_js.</span>online ()](#apidoc.element.is_js.online)
- description and source-code
```javascript
online = function () {
    return !navigator || navigator.onLine === true;
}
```
- example usage
```shell
...
is.tablet();
=> true if current device is tablet

is.not.tablet();
=> true if current device is not tablet
'''

is.online()
-----------
####Checks if current device is online.
interface: not

'''javascript
is.online();
=> true if current device is online
...
```

#### <a name="apidoc.element.is_js.opera"></a>[function <span class="apidocSignatureSpan">is_js.</span>opera (range)](#apidoc.element.is_js.opera)
- description and source-code
```javascript
opera = function (range) {
    var match = userAgent.match(/(?:^opera.+?version|opr)\/(\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.edge('>=12');
=> true if current version of edge is greater than or equal to 12

is.not.edge('<13');
=> true if current version of edge is not less than 13
'''

is.opera(range:number|string)
----------
####Checks if current browser is opera. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.opera();
=> true if current browser is opera
...
```

#### <a name="apidoc.element.is_js.palindrome"></a>[function <span class="apidocSignatureSpan">is_js.</span>palindrome (string)](#apidoc.element.is_js.palindrome)
- description and source-code
```javascript
palindrome = function (string) {
    if (is.not.string(string)) {
        return false;
    }
    string = string.replace(/[^a-zA-Z0-9]+/g, '').toLowerCase();
    var length = string.length - 1;
    for (var i = 0, half = Math.floor(length / 2); i <= half; i++) {
        if (string.charAt(i) !== string.charAt(length - i)) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.capitalized(['Nope', 'not']);
=> false
'''

is.palindrome(value:string)
---------------------------------------------
####Checks if the given string is palindrome.
interfaces: not, all, any

'''javascript
is.palindrome('testset');
=> true
...
```

#### <a name="apidoc.element.is_js.past"></a>[function <span class="apidocSignatureSpan">is_js.</span>past (date)](#apidoc.element.is_js.past)
- description and source-code
```javascript
past = function (date) {
    var now = new Date();
    return is.date(date) && date.getTime() < now.getTime();
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.tomorrow([today, tomorrow]);
=> false
'''

is.past(value:date)
---------------------
####Checks if the given date object indicate past.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.phantom"></a>[function <span class="apidocSignatureSpan">is_js.</span>phantom (range)](#apidoc.element.is_js.phantom)
- description and source-code
```javascript
phantom = function (range) {
    var match = userAgent.match(/phantomjs\/(\d+)/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.safari('>=8');
=> true if current version of safari is greater than or equal to 8

is.not.safari('<7');
=> true if current version of safari is not less than 7
'''

is.phantom(range:number|string)
-----------
####Checks if current browser is phantomjs. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.phantom();
=> true if current browser is phantomjs
...
```

#### <a name="apidoc.element.is_js.positive"></a>[function <span class="apidocSignatureSpan">is_js.</span>positive (n)](#apidoc.element.is_js.positive)
- description and source-code
```javascript
positive = function (n) {
    return is.number(n) && n > 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.odd([40, 42, 43]);
=> false
'''

is.positive(value:number)
-------------------------
####Checks if the given value is positive.
interfaces: not, all, any

'''javascript
is.positive(41);
=> true
...
```

#### <a name="apidoc.element.is_js.propertyCount"></a>[function <span class="apidocSignatureSpan">is_js.</span>propertyCount (object, count)](#apidoc.element.is_js.propertyCount)
- description and source-code
```javascript
propertyCount = function (object, count) {
    if (is.not.object(object) || is.not.number(count)) {
        return false;
    }
    var n = 0;
    for (var property in object) {
        if (hasOwnProperty.call(object, property) && ++n > count) {
            return false;
        }
    }
    return n === count;
}
```
- example usage
```shell
...
is.all.infinite([Infinity, -Infinity, 42.5]);
=> false
'''

Object checks
=============

is.propertyCount(value:object, count:number)
-------------------------------------
####Checks if objects' property count is equal to given count.
interface: not

'''javascript
is.propertyCount({this: 'is', 'sample': object}, 2);
=> true
...
```

#### <a name="apidoc.element.is_js.propertyDefined"></a>[function <span class="apidocSignatureSpan">is_js.</span>propertyDefined (object, property)](#apidoc.element.is_js.propertyDefined)
- description and source-code
```javascript
propertyDefined = function (object, property) {
    return is.object(object) && is.string(property) && property in object;
}
```
- example usage
```shell
...
is.propertyCount({this: 'is', 'sample': object}, 3);
=> false

is.not.propertyCount({}, 2);
=> true
'''

is.propertyDefined(value:object, property:string)
------------------------------------------
####Checks if the given property is defined on object.
interface: not

'''javascript
is.propertyDefined({yeap: 'yeap'}, 'yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.quarterOfYear"></a>[function <span class="apidocSignatureSpan">is_js.</span>quarterOfYear (date, quarter)](#apidoc.element.is_js.quarterOfYear)
- description and source-code
```javascript
quarterOfYear = function (date, quarter) {
    return is.date(date) && is.number(quarter) && quarter === Math.floor((date.getMonth() + 3) / 3);
}
```
- example usage
```shell
...
is.inNextYear(thirteenMonthsLater);
=> false

is.not.inNextYear(thirteenMonthsLater);
=> true
'''

is.quarterOfYear(value:date, quarter:number)
---------------------------------------------
####Checks if the given date is in the parameter quarter.
interface: not

'''javascript
var firstQuarter = new Date('01/26/2015');
var secondQuarter = new Date('05/26/2015');
...
```

#### <a name="apidoc.element.is_js.regexp"></a>[function <span class="apidocSignatureSpan">is_js.</span>regexp (value)](#apidoc.element.is_js.regexp)
- description and source-code
```javascript
regexp = function (value) {
    return toString.call(value) === '[object RegExp]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.json([{}, {foo: 'bar'}]);
=> true
'''

is.regexp(value:any)
--------------------
####Checks if the given value type is RegExp.
interfaces: not, all, any

'''javascript
is.regexp(/test/);
=> true
...
```

#### <a name="apidoc.element.is_js.safari"></a>[function <span class="apidocSignatureSpan">is_js.</span>safari (range)](#apidoc.element.is_js.safari)
- description and source-code
```javascript
safari = function (range) {
    var match = userAgent.match(/version\/(\d+).+?safari/);
    return match !== null && compareVersion(match[1], range);
}
```
- example usage
```shell
...
is.opera('>=35');
=> true if current version of opera is greater than or equal to 35

is.not.opera('<20');
=> true if current version of opera is not less than 20
'''

is.safari(range:number|string)
-----------
####Checks if current browser is safari. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.safari();
=> true if current browser is safari
...
```

#### <a name="apidoc.element.is_js.sameType"></a>[function <span class="apidocSignatureSpan">is_js.</span>sameType (value, other)](#apidoc.element.is_js.sameType)
- description and source-code
```javascript
sameType = function (value, other) {
    var tag = toString.call(value);
    if (tag !== toString.call(other)) {
        return false;
    }
    if (tag === '[object Number]') {
        return !is.any.nan(value, other) || is.all.nan(value, other);
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.undefined([{}, undefined]);
=> false
'''

is.sameType(value:any, other:any)
---------------------------------
####Checks if the given value types are same type.
interface: not

'''javascript
is.sameType(42, 7);
=> true
...
```

#### <a name="apidoc.element.is_js.setNamespace"></a>[function <span class="apidocSignatureSpan">is_js.</span>setNamespace ()](#apidoc.element.is_js.setNamespace)
- description and source-code
```javascript
setNamespace = function () {
    root.is = previousIs;
    return this;
}
```
- example usage
```shell
...
is.not.dayLightSavingTime(january1);
=> true
'''

Configuration methods
=====================

is.setNamespace()
-----------------
Change namespace of library to prevent name collisions.

'''javascript
var customName = is.setNamespace();
customName.odd(3);
=> true
...
```

#### <a name="apidoc.element.is_js.setRegexp"></a>[function <span class="apidocSignatureSpan">is_js.</span>setRegexp (regexp, name)](#apidoc.element.is_js.setRegexp)
- description and source-code
```javascript
setRegexp = function (regexp, name) {
    for (var r in regexes) {
        if (hasOwnProperty.call(regexes, r) && (name === r)) {
            regexes[r] = regexp;
        }
    }
}
```
- example usage
```shell
...

'''javascript
var customName = is.setNamespace();
customName.odd(3);
=> true
'''

is.setRegexp(value:regexp, name:string)
----------------------------------------
Override RegExps if you think they suck.

'''javascript
is.url('https://www.duckduckgo.com');
=> true
...
```

#### <a name="apidoc.element.is_js.socialSecurityNumber"></a>[function <span class="apidocSignatureSpan">is_js.</span>socialSecurityNumber (value)](#apidoc.element.is_js.socialSecurityNumber)
- description and source-code
```javascript
socialSecurityNumber = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.eppPhone(['+90.2322456789', '123']);
=> false
'''

is.socialSecurityNumber(value:any)
----------------------------------
####Checks if the given value matches social security number regexp.
interfaces: not, all, any

'''javascript
is.socialSecurityNumber('017-90-7890');
=> true
...
```

#### <a name="apidoc.element.is_js.sorted"></a>[function <span class="apidocSignatureSpan">is_js.</span>sorted (array, sign)](#apidoc.element.is_js.sorted)
- description and source-code
```javascript
sorted = function (array, sign) {
    if (is.not.array(array)) {
        return false;
    }
    var predicate = comparator[sign] || comparator['>='];
    for (var i = 1; i < array.length; i++) {
        if (!predicate(array[i], array[i - 1])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inArray(4, [1, 2, 3]);
=> false

is.not.inArray(4, [1, 2, 3]);
=> true
'''

is.sorted(value:array, sign:string)
----------------------
####Checks if the given array is sorted. Sign is optional parameter.
interfaces: not, all, any

'''javascript
is.sorted([1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.space"></a>[function <span class="apidocSignatureSpan">is_js.</span>space (value)](#apidoc.element.is_js.space)
- description and source-code
```javascript
space = function (value) {
    if (is.not.char(value)) {
        return false;
    }
    var charCode = value.charCodeAt(0);
    return (charCode > 8 && charCode < 14) || charCode === 32;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.falsy([false, true, undefined]);
=> false
'''

is.space(value:any)
----------------------
####Checks if the given value is space.
interfaces: not, all, any

'''javascript
is.space(' ');
=> true
...
```

#### <a name="apidoc.element.is_js.startWith"></a>[function <span class="apidocSignatureSpan">is_js.</span>startWith (string, target)](#apidoc.element.is_js.startWith)
- description and source-code
```javascript
startWith = function (string, target) {
    return is.string(string) && string.indexOf(target) === 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.lowerCase(['yeap', 'all lowercase']);
=> true
'''

is.startWith(value:string, target:string)
-------------------------------------------
####Checks if the given string starts with substring.
interface: not

'''javascript
is.startWith('yeap', 'ye');
=> true
...
```

#### <a name="apidoc.element.is_js.string"></a>[function <span class="apidocSignatureSpan">is_js.</span>string (value)](#apidoc.element.is_js.string)
- description and source-code
```javascript
string = function (value) {
    return toString.call(value) === '[object String]';
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.regexp([{}, /test/]);
=> false
'''

is.string(value:any)
--------------------
####Checks if the given value type is string.
interfaces: not, all, any

'''javascript
is.string('foo');
=> true
...
```

#### <a name="apidoc.element.is_js.tablet"></a>[function <span class="apidocSignatureSpan">is_js.</span>tablet ()](#apidoc.element.is_js.tablet)
- description and source-code
```javascript
tablet = function () {
    return is.ipad() || is.androidTablet() || is.windowsTablet();
}
```
- example usage
```shell
...
is.mobile();
=> true if current device is mobile

is.not.mobile();
=> true if current device is not mobile
'''

is.tablet()
-----------
####Checks if current device is tablet.
interface: not
iPad, Android Tablet, Windows Tablet
'''javascript

is.tablet();
...
```

#### <a name="apidoc.element.is_js.timeString"></a>[function <span class="apidocSignatureSpan">is_js.</span>timeString (value)](#apidoc.element.is_js.timeString)
- description and source-code
```javascript
timeString = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.alphaNumeric(['alphaNu3er1k', '*?']);
=> false
'''

is.timeString(value:any)
------------------------
####Checks if the given value matches time string regexp.
interfaces: not, all, any

'''javascript
is.timeString('13:45:30');
=> true
...
```

#### <a name="apidoc.element.is_js.today"></a>[function <span class="apidocSignatureSpan">is_js.</span>today (date)](#apidoc.element.is_js.today)
- description and source-code
```javascript
today = function (date) {
    var now = new Date();
    var todayString = now.toDateString();
    return is.date(date) && date.toDateString() === todayString;
}
```
- example usage
```shell
...
is.not.touchDevice();
=> true if current device does not support touch
'''

Time checks
===========

is.today(value:date)
----------------------
####Checks if the given date object indicate today.
interfaces: not, all, any

'''javascript
var today = new Date();
is.today(today);
...
```

#### <a name="apidoc.element.is_js.tomorrow"></a>[function <span class="apidocSignatureSpan">is_js.</span>tomorrow (date)](#apidoc.element.is_js.tomorrow)
- description and source-code
```javascript
tomorrow = function (date) {
    var now = new Date();
    var tomorrowString = new Date(now.setDate(now.getDate() + 1)).toDateString();
    return is.date(date) && date.toDateString() === tomorrowString;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.yesterday([today, yesterday]);
=> false
'''

is.tomorrow(value:date)
-------------------------
####Checks if the given date object indicate tomorrow.
interfaces: not, all, any

'''javascript
var today = new Date();
is.tomorrow(today);
...
```

#### <a name="apidoc.element.is_js.touchDevice"></a>[function <span class="apidocSignatureSpan">is_js.</span>touchDevice ()](#apidoc.element.is_js.touchDevice)
- description and source-code
```javascript
touchDevice = function () {
    return !!document && ('ontouchstart' in freeSelf ||
        ('DocumentTouch' in freeSelf && document instanceof DocumentTouch));
}
```
- example usage
```shell
...
is.offline();
=> true if current device is offline

is.not.offline();
=> true if current device is not offline
'''

is.touchDevice()
------------
####Checks if current device supports touch.
interface: not

'''javascript
is.touchDevice();
=> true if current device supports touch
...
```

#### <a name="apidoc.element.is_js.truthy"></a>[function <span class="apidocSignatureSpan">is_js.</span>truthy ()](#apidoc.element.is_js.truthy)
- description and source-code
```javascript
truthy = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.existy([{}, 'foo']);
=> true
'''

is.truthy(value:any)
--------------------
####Checks if the given value is truthy. (existy and not false)
interfaces: not, all, any

'''javascript
is.truthy(true);
=> true
...
```

#### <a name="apidoc.element.is_js.ukPostCode"></a>[function <span class="apidocSignatureSpan">is_js.</span>ukPostCode (value)](#apidoc.element.is_js.ukPostCode)
- description and source-code
```javascript
ukPostCode = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.caPostalCode(['L8V3Y1', '123']);
=> false
'''

is.ukPostCode(value:any)
------------------------
####Checks if the given value matches UK post code regexp.
interfaces: not, all, any

'''javascript
is.ukPostCode('B184BJ');
=> true
...
```

#### <a name="apidoc.element.is_js.undefined"></a>[function <span class="apidocSignatureSpan">is_js.</span>undefined (value)](#apidoc.element.is_js.undefined)
- description and source-code
```javascript
undefined = function (value) {
    return value === void 0;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.char(['f', 'o', 'o']);
=> true
'''

is.undefined(value:any)
-----------------------
####Checks if the given value type is undefined.
interfaces: not, all, any

'''javascript
is.undefined(undefined);
=> true
...
```

#### <a name="apidoc.element.is_js.under"></a>[function <span class="apidocSignatureSpan">is_js.</span>under (n, max)](#apidoc.element.is_js.under)
- description and source-code
```javascript
under = function (n, max) {
    return is.all.number(n, max) && n < max;
}
```
- example usage
```shell
...
is.above(41, 30);
=> true

is.not.above(42, 50);
=> true
'''

is.under(value:number, max:number)
---------------------------
####Checks if the given value is under maximum value.
interface: not

'''javascript
is.under(30, 35);
=> true
...
```

#### <a name="apidoc.element.is_js.upperCase"></a>[function <span class="apidocSignatureSpan">is_js.</span>upperCase (string)](#apidoc.element.is_js.upperCase)
- description and source-code
```javascript
upperCase = function (string) {
    return is.string(string) && string === string.toUpperCase();
}
```
- example usage
```shell
...
is.include('test', 'text');
=> false

is.not.include('test', 'text');
=> true
'''

is.upperCase(value:string)
--------------------------
####Checks if the given string is UPPERCASE.
interfaces: not, all, any

'''javascript
is.upperCase('YEAP');
=> true
...
```

#### <a name="apidoc.element.is_js.url"></a>[function <span class="apidocSignatureSpan">is_js.</span>url (value)](#apidoc.element.is_js.url)
- description and source-code
```javascript
url = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
is.all.space([' ', 'foo', undefined]);
=> false
'''

RegExp checks
=============

is.url(value:any)
-----------------
####Checks if the given value matches url regexp.
interfaces: not, all, any

'''javascript
is.url('http://www.test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.usZipCode"></a>[function <span class="apidocSignatureSpan">is_js.</span>usZipCode (value)](#apidoc.element.is_js.usZipCode)
- description and source-code
```javascript
usZipCode = function (value) {
    return regexes[regexp].test(value);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.dateString(['11/11/2011', '90/11/2011']);
=> false
'''

is.usZipCode(value:any)
-----------------------
####Checks if the given value matches US zip code regexp.
interfaces: not, all, any

'''javascript
is.usZipCode('02201-1020');
=> true
...
```

#### <a name="apidoc.element.is_js.weekday"></a>[function <span class="apidocSignatureSpan">is_js.</span>weekday ()](#apidoc.element.is_js.weekday)
- description and source-code
```javascript
weekday = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekend([sunday, saturday, monday]);
=> false
'''

is.weekday(value:date)
------------------------
####Checks if the given date objects' day is weekday.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.weekend"></a>[function <span class="apidocSignatureSpan">is_js.</span>weekend (date)](#apidoc.element.is_js.weekend)
- description and source-code
```javascript
weekend = function (date) {
    return is.date(date) && (date.getDay() === 6 || date.getDay() === 0);
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.leapYear([2016, 2080]);
=> true
'''

is.weekend(value:date)
------------------------
####Checks if the given date objects' day is weekend.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.windowObject"></a>[function <span class="apidocSignatureSpan">is_js.</span>windowObject (value)](#apidoc.element.is_js.windowObject)
- description and source-code
```javascript
windowObject = function (value) {
    return value != null && typeof value === 'object' && 'setInterval' in value;
}
```
- example usage
```shell
...
is.sameType(42, '7');
=> false

is.not.sameType(42, 7);
=> false
'''

is.windowObject(value:any)
-----------------------------
####Checks if the given object is window object.
interfaces: not, all, any

'''javascript
is.windowObject(window);
=> true
...
```

#### <a name="apidoc.element.is_js.windows"></a>[function <span class="apidocSignatureSpan">is_js.</span>windows ()](#apidoc.element.is_js.windows)
- description and source-code
```javascript
windows = function () {
    return /win/.test(appVersion);
}
```
- example usage
```shell
...
is.windowsTablet();
=> true if current device is Windows tablet

is.not.windowsTablet();
=> true if current device is not Windows tablet
'''

is.windows()
------------
####Checks if current OS is Windows.
interface: not

'''javascript
is.windows();
=> true if current OS is Windows
...
```

#### <a name="apidoc.element.is_js.windowsPhone"></a>[function <span class="apidocSignatureSpan">is_js.</span>windowsPhone ()](#apidoc.element.is_js.windowsPhone)
- description and source-code
```javascript
windowsPhone = function () {
    return is.windows() && /phone/.test(userAgent);
}
```
- example usage
```shell
...
is.blackberry();
=> true if current device is Blackberry

is.not.blackberry();
=> true if current device is not Blackberry
'''

is.windowsPhone()
-----------------
####Checks if current device is Windows phone.
interface: not

'''javascript
is.windowsPhone();
=> true if current device is Windows phone
...
```

#### <a name="apidoc.element.is_js.windowsTablet"></a>[function <span class="apidocSignatureSpan">is_js.</span>windowsTablet ()](#apidoc.element.is_js.windowsTablet)
- description and source-code
```javascript
windowsTablet = function () {
    return is.windows() && is.not.windowsPhone() && /touch/.test(userAgent);
}
```
- example usage
```shell
...
is.windowsPhone();
=> true if current device is Windows phone

is.not.windowsPhone();
=> true if current device is not Windows Phone
'''

is.windowsTablet()
------------------
####Checks if current device is Windows tablet.
interface: not

'''javascript
is.windowsTablet();
=> true if current device is Windows tablet
...
```

#### <a name="apidoc.element.is_js.within"></a>[function <span class="apidocSignatureSpan">is_js.</span>within (n, min, max)](#apidoc.element.is_js.within)
- description and source-code
```javascript
within = function (n, min, max) {
    return is.all.number(n, min, max) && n > min && n < max;
}
```
- example usage
```shell
...
is.under(30, 35);
=> true

is.not.under(42, 30);
=> true
'''

is.within(value:number, min:number, max:number)
---------------------------------
####Checks if the given value is within minimum and maximum values.
interface: not

'''javascript
is.within(30, 20, 40);
=> true
...
```

#### <a name="apidoc.element.is_js.year"></a>[function <span class="apidocSignatureSpan">is_js.</span>year (date, year)](#apidoc.element.is_js.year)
- description and source-code
```javascript
year = function (date, year) {
    return is.date(date) && is.number(year) && year === date.getFullYear();
}
```
- example usage
```shell
...
is.month(februaryObj, 'january');
=> false

is.not.month(februaryObj, 'january');
=> true
'''

is.year(value:date, year:number)
---------------------------------
####Checks if the given date objects' year equal given yearNumber parameter.
interface: not

'''javascript
var year2015 = new Date('01/26/2015');
var year2016 = new Date('01/26/2016');
...
```

#### <a name="apidoc.element.is_js.yesterday"></a>[function <span class="apidocSignatureSpan">is_js.</span>yesterday (date)](#apidoc.element.is_js.yesterday)
- description and source-code
```javascript
yesterday = function (date) {
    var now = new Date();
    var yesterdayString = new Date(now.setDate(now.getDate() - 1)).toDateString();
    return is.date(date) && date.toDateString() === yesterdayString;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.today([today, yesterday]);
=> false
'''

is.yesterday(value:date)
--------------------------
####Checks if the given date object indicate yesterday.
interfaces: not, all, any

'''javascript
var today = new Date();
is.yesterday(today);
...
```



# <a name="apidoc.module.is_js.all"></a>[module is_js.all](#apidoc.module.is_js.all)

#### <a name="apidoc.element.is_js.all.affirmative"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>affirmative ()](#apidoc.element.is_js.all.affirmative)
- description and source-code
```javascript
affirmative = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.socialSecurityNumber(['017-90-7890', '123']);
=> false
'''

is.affirmative(value:any)
-------------------------
####Checks if the given value matches affirmative regexp.
interfaces: not, all, any

'''javascript
is.affirmative('yes');
=> true
...
```

#### <a name="apidoc.element.is_js.all.alphaNumeric"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>alphaNumeric ()](#apidoc.element.is_js.all.alphaNumeric)
- description and source-code
```javascript
alphaNumeric = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.creditCard([378282246310005, 123, undefined]);
=> false
'''

is.alphaNumeric(value:any)
--------------------------
####Checks if the given value matches alpha numeric regexp.
interfaces: not, all, any

'''javascript
is.alphaNumeric('alphaNu3er1k');
=> true
...
```

#### <a name="apidoc.element.is_js.all.arguments"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>arguments ()](#apidoc.element.is_js.all.arguments)
- description and source-code
```javascript
arguments = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...

####Contributors:
Many thanks to our contributors: https://github.com/arasatasaygin/is.js/graphs/contributors

Type checks
===========

is.arguments(value:any)
-----------------------
####Checks if the given value type is arguments.
interfaces: not, all, any

'''javascript
var getArguments = function() {
return arguments;
...
```

#### <a name="apidoc.element.is_js.all.array"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>array ()](#apidoc.element.is_js.all.array)
- description and source-code
```javascript
array = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.arguments([arguments, 'foo', 'bar']);
=> false
'''

is.array(value:any)
-------------------
####Checks if the given value type is array.
interfaces: not, all, any

'''javascript
is.array(['foo', 'bar', 'baz']);
=> true
...
```

#### <a name="apidoc.element.is_js.all.boolean"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>boolean ()](#apidoc.element.is_js.all.boolean)
- description and source-code
```javascript
boolean = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.array([[1, 2], 'foo', 'bar']);
=> false
'''

is.boolean(value:any)
---------------------
####Checks if the given value type is boolean.
interfaces: not, all, any

'''javascript
is.boolean(true);
=> true
...
```

#### <a name="apidoc.element.is_js.all.caPostalCode"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>caPostalCode ()](#apidoc.element.is_js.all.caPostalCode)
- description and source-code
```javascript
caPostalCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.usZipCode(['02201-1020', '123']);
=> false
'''

is.caPostalCode(value:any)
--------------------------
####Checks if the given value matches Canada postal code regexp.
interfaces: not, all, any

'''javascript
is.caPostalCode('L8V3Y1');
=> true
...
```

#### <a name="apidoc.element.is_js.all.capitalized"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>capitalized ()](#apidoc.element.is_js.all.capitalized)
- description and source-code
```javascript
capitalized = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.not.endWith('nope not that', 'not');
=> true

is.endWith('yeap that one', 'one');
=> true
'''

is.capitalized(value:string)
---------------------------------------------
####Checks if the given string is capitalized.
interfaces: not, all, any

'''javascript
is.capitalized('Yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.all.char"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>char ()](#apidoc.element.is_js.all.char)
- description and source-code
```javascript
char = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.string([{}, 'foo']);
=> false
'''

is.char(value:any)
--------------------
####Checks if the given value type is char.
interfaces: not, all, any

'''javascript
is.char('f');
=> true
...
```

#### <a name="apidoc.element.is_js.all.creditCard"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>creditCard ()](#apidoc.element.is_js.all.creditCard)
- description and source-code
```javascript
creditCard = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.email(['test@test.com', 'foo', undefined]);
=> false
'''

is.creditCard(value:any)
------------------------
####Checks if the given value matches credit card regexp.
interfaces: not, all, any

'''javascript
is.creditCard(378282246310005);
=> true
...
```

#### <a name="apidoc.element.is_js.all.date"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>date ()](#apidoc.element.is_js.all.date)
- description and source-code
```javascript
date = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.boolean([true, 'foo', 'bar']);
=> false
'''

is.date(value:any)
------------------
####Checks if the given value type is date.
interfaces: not, all, any

'''javascript
is.date(new Date());
=> true
...
```

#### <a name="apidoc.element.is_js.all.dateString"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>dateString ()](#apidoc.element.is_js.all.dateString)
- description and source-code
```javascript
dateString = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.timeString(['13:45:30', '90:90:90']);
=> false
'''

is.dateString(value:any)
------------------------
####Checks if the given value matches date string regexp.
interfaces: not, all, any

'''javascript
is.dateString('11/11/2011');
=> true
...
```

#### <a name="apidoc.element.is_js.all.dayLightSavingTime"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>dayLightSavingTime ()](#apidoc.element.is_js.all.dayLightSavingTime)
- description and source-code
```javascript
dayLightSavingTime = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.quarterOfYear(secondQuarter, 1);
=> false

is.not.quarterOfYear(secondQuarter, 1);
=> true
'''

is.dayLightSavingTime(value:date)
--------------------------------------------------
####Checks if the given date is in daylight saving time.
interface: not

'''javascript
// For Turkey Time Zone
var january1 = new Date('01/01/2015');
...
```

#### <a name="apidoc.element.is_js.all.decimal"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>decimal ()](#apidoc.element.is_js.all.decimal)
- description and source-code
```javascript
decimal = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.within(30, 20, 40);
=> true

is.not.within(40, 30, 35);
=> true
'''

is.decimal(value:number)
------------------------
####Checks if the given value is decimal.
interfaces: not, all, any

'''javascript
is.decimal(41.5);
=> true
...
```

#### <a name="apidoc.element.is_js.all.domNode"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>domNode ()](#apidoc.element.is_js.all.domNode)
- description and source-code
```javascript
domNode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.date([new Date(), 'foo', 'bar']);
=> false
'''

is.domNode(value:any)
-----------------------------
####Checks if the given object is a dom node.
interfaces: not, all, any

'''javascript
var obj = document.createElement('div');
is.domNode(obj);
...
```

#### <a name="apidoc.element.is_js.all.email"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>email ()](#apidoc.element.is_js.all.email)
- description and source-code
```javascript
email = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.url(['http://www.test.com', 'foo', undefined]);
=> false
'''

is.email(value:any)
-------------------
####Checks if the given value matches email regexp.
interfaces: not, all, any

'''javascript
is.email('test@test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.all.empty"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>empty ()](#apidoc.element.is_js.all.empty)
- description and source-code
```javascript
empty = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.all.windowObject([window, {nope: 'nope'}]);
=> false
'''

Presence checks
===============

is.empty(value:array|object|string)
-----------------------------------
####Checks if the given value is empty.
interfaces: not, all, any

'''javascript
is.empty({});
=> true
...
```

#### <a name="apidoc.element.is_js.all.eppPhone"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>eppPhone ()](#apidoc.element.is_js.all.eppPhone)
- description and source-code
```javascript
eppPhone = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nanpPhone(['609-555-0175', '123']);
=> false
'''

is.eppPhone(value:any)
----------------------
####Checks if the given value matches extensible provisioning protocol phone regexp.
interfaces: not, all, any

'''javascript
is.eppPhone('+90.2322456789');
=> true
...
```

#### <a name="apidoc.element.is_js.all.error"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>error ()](#apidoc.element.is_js.all.error)
- description and source-code
```javascript
error = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.domNode([obj, {nope: 'nope'}]);
=> false
'''

is.error(value:any)
-------------------
####Checks if the given value type is error.
interfaces: not, all, any

'''javascript
is.error(new Error());
=> true
...
```

#### <a name="apidoc.element.is_js.all.even"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>even ()](#apidoc.element.is_js.all.even)
- description and source-code
```javascript
even = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.equal(true, true);
=> true

is.not.equal('yeap', 'nope');
=> true
'''

is.even(value:number)
---------------------
####Checks if the given value is even.
interfaces: not, all, any

'''javascript
is.even(42);
=> true
...
```

#### <a name="apidoc.element.is_js.all.existy"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>existy ()](#apidoc.element.is_js.all.existy)
- description and source-code
```javascript
existy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.empty([{}, 'foo']);
=> false
'''

is.existy(value:any)
--------------------
####Checks if the given value is existy. (not null or undefined)
interfaces: not, all, any

'''javascript
is.existy({});
=> true
...
```

#### <a name="apidoc.element.is_js.all.falsy"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>falsy ()](#apidoc.element.is_js.all.falsy)
- description and source-code
```javascript
falsy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.truthy([{}, true]);
=> true
'''

is.falsy(value:any)
-------------------
####Checks if the given value is falsy.
interfaces: not, all, any

'''javascript
is.falsy(false);
=> true
...
```

#### <a name="apidoc.element.is_js.all.finite"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>finite ()](#apidoc.element.is_js.all.finite)
- description and source-code
```javascript
finite = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.integer([40, 42.5, -43]);
=> false
'''

is.finite(value:number)
-----------------------
####Checks if the given value is finite.
interfaces: not, all, any

'''javascript
is.finite(41);
=> true
...
```

#### <a name="apidoc.element.is_js.all.function"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>function ()](#apidoc.element.is_js.all.function)
- description and source-code
```javascript
function = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.error([new Error(), 'foo', 'bar']);
=> false
'''

is.function(value:any)
----------------------
####Checks if the given value type is function.
interfaces: not, all, any

'''javascript
is.function(toString);
=> true
...
```

#### <a name="apidoc.element.is_js.all.future"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>future ()](#apidoc.element.is_js.all.future)
- description and source-code
```javascript
future = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.past([yesterday, tomorrow]);
=> false
'''

is.future(value:date)
-----------------------
####Checks if the given date object indicate future.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.all.hexColor"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>hexColor ()](#apidoc.element.is_js.all.hexColor)
- description and source-code
```javascript
hexColor = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.hexadecimal(['fff', '333', 'f50']);
=> true
'''

is.hexColor(value:any)
-------------------------
####Checks if the given value matches hexcolor regexp.
interfaces: not, all, any

'''javascript
is.hexColor('#333');
=> true
...
```

#### <a name="apidoc.element.is_js.all.hexadecimal"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>hexadecimal ()](#apidoc.element.is_js.all.hexadecimal)
- description and source-code
```javascript
hexadecimal = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.affirmative(['yes', 'y', 'true', 't', 'ok', 'okay']);
=> true
'''

is.hexadecimal(value:any)
-------------------------
####Checks if the given value matches hexadecimal regexp.
interfaces: not, all, any

'''javascript
is.hexadecimal('f0f0f0');
=> true
...
```

#### <a name="apidoc.element.is_js.all.inLastMonth"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inLastMonth ()](#apidoc.element.is_js.all.inLastMonth)
- description and source-code
```javascript
inLastMonth = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inLastWeek(nineDaysAgo);
=> false

is.not.inLastWeek(nineDaysAgo);
=> true
'''

is.inLastMonth(value:date)
----------------------------
####Checks if the given date is between now and a month ago.
interface: not

'''javascript
var tenDaysAgo = new Date(new Date().setDate(new Date().getDate() - 10));
var fortyDaysAgo = new Date(new Date().setDate(new Date().getDate() - 40));
...
```

#### <a name="apidoc.element.is_js.all.inLastWeek"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inLastWeek ()](#apidoc.element.is_js.all.inLastWeek)
- description and source-code
```javascript
inLastWeek = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inDateRange(saturday, sunday, monday);
=> false

is.not.inDateRange(saturday, sunday, monday);
=> true
'''

is.inLastWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days ago.
interface: not

'''javascript
var twoDaysAgo = new Date(new Date().setDate(new Date().getDate() - 2));
var nineDaysAgo = new Date(new Date().setDate(new Date().getDate() - 9));
...
```

#### <a name="apidoc.element.is_js.all.inLastYear"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inLastYear ()](#apidoc.element.is_js.all.inLastYear)
- description and source-code
```javascript
inLastYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inLastMonth(fortyDaysAgo);
=> false

is.not.inLastMonth(fortyDaysAgo);
=> true
'''

is.inLastYear(value:date)
---------------------------
####Checks if the given date is between now and a year ago.
interface: not

'''javascript
var twoMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 2));
var thirteenMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 13));
...
```

#### <a name="apidoc.element.is_js.all.inNextMonth"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inNextMonth ()](#apidoc.element.is_js.all.inNextMonth)
- description and source-code
```javascript
inNextMonth = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inNextWeek(nineDaysLater);
=> false

is.not.inNextWeek(nineDaysLater);
=> true
'''

is.inNextMonth(value:date)
----------------------------
####Checks if the given date is between now and a month later.
interface: not

'''javascript
var tenDaysLater = new Date(new Date().setDate(new Date().getDate() + 10));
var fortyDaysLater = new Date(new Date().setDate(new Date().getDate() + 40));
...
```

#### <a name="apidoc.element.is_js.all.inNextWeek"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inNextWeek ()](#apidoc.element.is_js.all.inNextWeek)
- description and source-code
```javascript
inNextWeek = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inLastYear(thirteenMonthsAgo);
=> false

is.not.inLastYear(thirteenMonthsAgo);
=> true
'''

is.inNextWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days later.
interface: not

'''javascript
var twoDaysLater = new Date(new Date().setDate(new Date().getDate() + 2));
var nineDaysLater = new Date(new Date().setDate(new Date().getDate() + 9));
...
```

#### <a name="apidoc.element.is_js.all.inNextYear"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>inNextYear ()](#apidoc.element.is_js.all.inNextYear)
- description and source-code
```javascript
inNextYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inNextMonth(fortyDaysLater);
=> false

is.not.inNextMonth(fortyDaysLater);
=> true
'''

is.inNextYear(value:date)
---------------------------
####Checks if the given date is between now and a year later.
interface: not

'''javascript
var twoMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 2));
var thirteenMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 13));
...
```

#### <a name="apidoc.element.is_js.all.infinite"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>infinite ()](#apidoc.element.is_js.all.infinite)
- description and source-code
```javascript
infinite = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.finite([Infinity, -Infinity, 42.5]);
=> false
'''

is.infinite(value:number)
-------------------------
####Checks if the given value is infinite.
interfaces: not, all, any

'''javascript
is.infinite(Infinity);
=> true
...
```

#### <a name="apidoc.element.is_js.all.integer"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>integer ()](#apidoc.element.is_js.all.integer)
- description and source-code
```javascript
integer = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.decimal([40, 42.5, -43]);
=> false
'''

is.integer(value:number)
------------------------
####Checks if the given value is integer.
interfaces: not, all, any

'''javascript
is.integer(41);
=> true
...
```

#### <a name="apidoc.element.is_js.all.ip"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>ip ()](#apidoc.element.is_js.all.ip)
- description and source-code
```javascript
ip = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> false

// 'all' and 'any' interfaces can also take array parameter
is.all.hexColor(['fff', '333', 'f50']);
=> true
'''

is.ip(value:any)
-------------------------
####Checks if the given value matches ip regexp
interfaces: not, all, any

'''javascript
is.ip('198.156.23.5');
=> true
...
```

#### <a name="apidoc.element.is_js.all.ipv4"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>ipv4 ()](#apidoc.element.is_js.all.ipv4)
- description and source-code
```javascript
ipv4 = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ip(['123.123.23.12', 'A:B:C:D:E:F:0:0']);
=> true
'''

is.ipv4(value:any)
-------------------------
####Checks if the given value matches ipv4 regexp
interfaces: not, all, any

'''javascript
is.ipv4('198.12.3.142');
=> true
...
```

#### <a name="apidoc.element.is_js.all.ipv6"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>ipv6 ()](#apidoc.element.is_js.all.ipv6)
- description and source-code
```javascript
ipv6 = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.ipv4(['198.12.3.142', '1.2.3']);
=> false

'''

is.ipv6(value:any)
-------------------------
####Checks if the given value matches ipv6 regexp
interfaces: not, all, any

'''javascript
is.ipv6('2001:DB8:0:0:1::1');
=> true
...
```

#### <a name="apidoc.element.is_js.all.json"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>json ()](#apidoc.element.is_js.all.json)
- description and source-code
```javascript
json = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.object([{}, new Object()]);
=> true
'''

is.json(value:any)
--------------------
####Checks if the given value type is pure json object.
interfaces: not, all, any

'''javascript
is.json({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.all.leapYear"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>leapYear ()](#apidoc.element.is_js.all.leapYear)
- description and source-code
```javascript
leapYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.year(year2016, 2015);
=> false

is.not.year(year2016, 2015);
=> true
'''

is.leapYear(value:number)
---------------------------------
####Checks if the given year number is a leap year
interfaces: not, all, any

'''javascript
is.leapYear(2016);
=> true
...
```

#### <a name="apidoc.element.is_js.all.lowerCase"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>lowerCase ()](#apidoc.element.is_js.all.lowerCase)
- description and source-code
```javascript
lowerCase = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.upperCase(['YEAP', 'ALL UPPERCASE']);
=> true
'''


is.lowerCase(value:string)
--------------------------
####Checks if the given string is lowercase.
interfaces: not, all, any

'''javascript
is.lowerCase('yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.all.nan"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>nan ()](#apidoc.element.is_js.all.nan)
- description and source-code
```javascript
nan = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.function([toString, 'foo', 'bar']);
=> false
'''

is.nan(value:any)
-----------------
####Checks if the given value type is NaN.
interfaces: not, all, any

'''javascript
is.nan(NaN);
=> true
...
```

#### <a name="apidoc.element.is_js.all.nanpPhone"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>nanpPhone ()](#apidoc.element.is_js.all.nanpPhone)
- description and source-code
```javascript
nanpPhone = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ukPostCode(['B184BJ', '123']);
=> false
'''

is.nanpPhone(value:any)
-----------------------
####Checks if the given value matches North American numbering plan phone regexp.
interfaces: not, all, any

'''javascript
is.nanpPhone('609-555-0175');
=> true
...
```

#### <a name="apidoc.element.is_js.all.negative"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>negative ()](#apidoc.element.is_js.all.negative)
- description and source-code
```javascript
negative = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.positive([40, 42, -43]);
=> false
'''

is.negative(value:number)
-------------------------
####Checks if the given value is negative.
interfaces: not, all, any

'''javascript
is.negative(-41);
=> true
...
```

#### <a name="apidoc.element.is_js.all.null"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>null ()](#apidoc.element.is_js.all.null)
- description and source-code
```javascript
null = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nan([NaN, 'foo', 1]);
=> false
'''

is.null(value:any)
------------------
####Checks if the given value type is null.
interfaces: not, all, any

'''javascript
is.null(null);
=> true
...
```

#### <a name="apidoc.element.is_js.all.number"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>number ()](#apidoc.element.is_js.all.number)
- description and source-code
```javascript
number = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.null([null, 'foo', 1]);
=> false
'''

is.number(value:any)
--------------------
####Checks if the given value type is number.
interfaces: not, all, any

'''javascript
is.number(42);
=> true
...
```

#### <a name="apidoc.element.is_js.all.object"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>object ()](#apidoc.element.is_js.all.object)
- description and source-code
```javascript
object = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.number([42, 'foo', 1]);
=> false
'''

is.object(value:any)
--------------------
####Checks if the given value type is object.
interfaces: not, all, any

'''javascript
is.object({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.all.odd"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>odd ()](#apidoc.element.is_js.all.odd)
- description and source-code
```javascript
odd = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.even([40, 42, 43]);
=> false
'''

is.odd(value:number)
--------------------
####Checks if the given value is odd.
interfaces: not, all, any

'''javascript
is.odd(41);
=> true
...
```

#### <a name="apidoc.element.is_js.all.palindrome"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>palindrome ()](#apidoc.element.is_js.all.palindrome)
- description and source-code
```javascript
palindrome = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.capitalized(['Nope', 'not']);
=> false
'''

is.palindrome(value:string)
---------------------------------------------
####Checks if the given string is palindrome.
interfaces: not, all, any

'''javascript
is.palindrome('testset');
=> true
...
```

#### <a name="apidoc.element.is_js.all.past"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>past ()](#apidoc.element.is_js.all.past)
- description and source-code
```javascript
past = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.tomorrow([today, tomorrow]);
=> false
'''

is.past(value:date)
---------------------
####Checks if the given date object indicate past.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.all.positive"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>positive ()](#apidoc.element.is_js.all.positive)
- description and source-code
```javascript
positive = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.odd([40, 42, 43]);
=> false
'''

is.positive(value:number)
-------------------------
####Checks if the given value is positive.
interfaces: not, all, any

'''javascript
is.positive(41);
=> true
...
```

#### <a name="apidoc.element.is_js.all.regexp"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>regexp ()](#apidoc.element.is_js.all.regexp)
- description and source-code
```javascript
regexp = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.json([{}, {foo: 'bar'}]);
=> true
'''

is.regexp(value:any)
--------------------
####Checks if the given value type is RegExp.
interfaces: not, all, any

'''javascript
is.regexp(/test/);
=> true
...
```

#### <a name="apidoc.element.is_js.all.socialSecurityNumber"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>socialSecurityNumber ()](#apidoc.element.is_js.all.socialSecurityNumber)
- description and source-code
```javascript
socialSecurityNumber = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.eppPhone(['+90.2322456789', '123']);
=> false
'''

is.socialSecurityNumber(value:any)
----------------------------------
####Checks if the given value matches social security number regexp.
interfaces: not, all, any

'''javascript
is.socialSecurityNumber('017-90-7890');
=> true
...
```

#### <a name="apidoc.element.is_js.all.sorted"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>sorted ()](#apidoc.element.is_js.all.sorted)
- description and source-code
```javascript
sorted = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.inArray(4, [1, 2, 3]);
=> false

is.not.inArray(4, [1, 2, 3]);
=> true
'''

is.sorted(value:array, sign:string)
----------------------
####Checks if the given array is sorted. Sign is optional parameter.
interfaces: not, all, any

'''javascript
is.sorted([1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.all.space"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>space ()](#apidoc.element.is_js.all.space)
- description and source-code
```javascript
space = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.falsy([false, true, undefined]);
=> false
'''

is.space(value:any)
----------------------
####Checks if the given value is space.
interfaces: not, all, any

'''javascript
is.space(' ');
=> true
...
```

#### <a name="apidoc.element.is_js.all.string"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>string ()](#apidoc.element.is_js.all.string)
- description and source-code
```javascript
string = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.regexp([{}, /test/]);
=> false
'''

is.string(value:any)
--------------------
####Checks if the given value type is string.
interfaces: not, all, any

'''javascript
is.string('foo');
=> true
...
```

#### <a name="apidoc.element.is_js.all.timeString"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>timeString ()](#apidoc.element.is_js.all.timeString)
- description and source-code
```javascript
timeString = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.alphaNumeric(['alphaNu3er1k', '*?']);
=> false
'''

is.timeString(value:any)
------------------------
####Checks if the given value matches time string regexp.
interfaces: not, all, any

'''javascript
is.timeString('13:45:30');
=> true
...
```

#### <a name="apidoc.element.is_js.all.today"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>today ()](#apidoc.element.is_js.all.today)
- description and source-code
```javascript
today = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.not.touchDevice();
=> true if current device does not support touch
'''

Time checks
===========

is.today(value:date)
----------------------
####Checks if the given date object indicate today.
interfaces: not, all, any

'''javascript
var today = new Date();
is.today(today);
...
```

#### <a name="apidoc.element.is_js.all.tomorrow"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>tomorrow ()](#apidoc.element.is_js.all.tomorrow)
- description and source-code
```javascript
tomorrow = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.yesterday([today, yesterday]);
=> false
'''

is.tomorrow(value:date)
-------------------------
####Checks if the given date object indicate tomorrow.
interfaces: not, all, any

'''javascript
var today = new Date();
is.tomorrow(today);
...
```

#### <a name="apidoc.element.is_js.all.truthy"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>truthy ()](#apidoc.element.is_js.all.truthy)
- description and source-code
```javascript
truthy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.existy([{}, 'foo']);
=> true
'''

is.truthy(value:any)
--------------------
####Checks if the given value is truthy. (existy and not false)
interfaces: not, all, any

'''javascript
is.truthy(true);
=> true
...
```

#### <a name="apidoc.element.is_js.all.ukPostCode"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>ukPostCode ()](#apidoc.element.is_js.all.ukPostCode)
- description and source-code
```javascript
ukPostCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.caPostalCode(['L8V3Y1', '123']);
=> false
'''

is.ukPostCode(value:any)
------------------------
####Checks if the given value matches UK post code regexp.
interfaces: not, all, any

'''javascript
is.ukPostCode('B184BJ');
=> true
...
```

#### <a name="apidoc.element.is_js.all.undefined"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>undefined ()](#apidoc.element.is_js.all.undefined)
- description and source-code
```javascript
undefined = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.char(['f', 'o', 'o']);
=> true
'''

is.undefined(value:any)
-----------------------
####Checks if the given value type is undefined.
interfaces: not, all, any

'''javascript
is.undefined(undefined);
=> true
...
```

#### <a name="apidoc.element.is_js.all.upperCase"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>upperCase ()](#apidoc.element.is_js.all.upperCase)
- description and source-code
```javascript
upperCase = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.include('test', 'text');
=> false

is.not.include('test', 'text');
=> true
'''

is.upperCase(value:string)
--------------------------
####Checks if the given string is UPPERCASE.
interfaces: not, all, any

'''javascript
is.upperCase('YEAP');
=> true
...
```

#### <a name="apidoc.element.is_js.all.url"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>url ()](#apidoc.element.is_js.all.url)
- description and source-code
```javascript
url = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.all.space([' ', 'foo', undefined]);
=> false
'''

RegExp checks
=============

is.url(value:any)
-----------------
####Checks if the given value matches url regexp.
interfaces: not, all, any

'''javascript
is.url('http://www.test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.all.usZipCode"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>usZipCode ()](#apidoc.element.is_js.all.usZipCode)
- description and source-code
```javascript
usZipCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.dateString(['11/11/2011', '90/11/2011']);
=> false
'''

is.usZipCode(value:any)
-----------------------
####Checks if the given value matches US zip code regexp.
interfaces: not, all, any

'''javascript
is.usZipCode('02201-1020');
=> true
...
```

#### <a name="apidoc.element.is_js.all.weekday"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>weekday ()](#apidoc.element.is_js.all.weekday)
- description and source-code
```javascript
weekday = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekend([sunday, saturday, monday]);
=> false
'''

is.weekday(value:date)
------------------------
####Checks if the given date objects' day is weekday.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.all.weekend"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>weekend ()](#apidoc.element.is_js.all.weekend)
- description and source-code
```javascript
weekend = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.leapYear([2016, 2080]);
=> true
'''

is.weekend(value:date)
------------------------
####Checks if the given date objects' day is weekend.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.all.windowObject"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>windowObject ()](#apidoc.element.is_js.all.windowObject)
- description and source-code
```javascript
windowObject = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
is.sameType(42, '7');
=> false

is.not.sameType(42, 7);
=> false
'''

is.windowObject(value:any)
-----------------------------
####Checks if the given object is window object.
interfaces: not, all, any

'''javascript
is.windowObject(window);
=> true
...
```

#### <a name="apidoc.element.is_js.all.yesterday"></a>[function <span class="apidocSignatureSpan">is_js.all.</span>yesterday ()](#apidoc.element.is_js.all.yesterday)
- description and source-code
```javascript
yesterday = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (!func.call(null, params[i])) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.today([today, yesterday]);
=> false
'''

is.yesterday(value:date)
--------------------------
####Checks if the given date object indicate yesterday.
interfaces: not, all, any

'''javascript
var today = new Date();
is.yesterday(today);
...
```



# <a name="apidoc.module.is_js.any"></a>[module is_js.any](#apidoc.module.is_js.any)

#### <a name="apidoc.element.is_js.any.affirmative"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>affirmative ()](#apidoc.element.is_js.any.affirmative)
- description and source-code
```javascript
affirmative = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.socialSecurityNumber(['017-90-7890', '123']);
=> false
'''

is.affirmative(value:any)
-------------------------
####Checks if the given value matches affirmative regexp.
interfaces: not, all, any

'''javascript
is.affirmative('yes');
=> true
...
```

#### <a name="apidoc.element.is_js.any.alphaNumeric"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>alphaNumeric ()](#apidoc.element.is_js.any.alphaNumeric)
- description and source-code
```javascript
alphaNumeric = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.creditCard([378282246310005, 123, undefined]);
=> false
'''

is.alphaNumeric(value:any)
--------------------------
####Checks if the given value matches alpha numeric regexp.
interfaces: not, all, any

'''javascript
is.alphaNumeric('alphaNu3er1k');
=> true
...
```

#### <a name="apidoc.element.is_js.any.arguments"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>arguments ()](#apidoc.element.is_js.any.arguments)
- description and source-code
```javascript
arguments = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...

####Contributors:
Many thanks to our contributors: https://github.com/arasatasaygin/is.js/graphs/contributors

Type checks
===========

is.arguments(value:any)
-----------------------
####Checks if the given value type is arguments.
interfaces: not, all, any

'''javascript
var getArguments = function() {
return arguments;
...
```

#### <a name="apidoc.element.is_js.any.array"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>array ()](#apidoc.element.is_js.any.array)
- description and source-code
```javascript
array = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.arguments([arguments, 'foo', 'bar']);
=> false
'''

is.array(value:any)
-------------------
####Checks if the given value type is array.
interfaces: not, all, any

'''javascript
is.array(['foo', 'bar', 'baz']);
=> true
...
```

#### <a name="apidoc.element.is_js.any.boolean"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>boolean ()](#apidoc.element.is_js.any.boolean)
- description and source-code
```javascript
boolean = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.array([[1, 2], 'foo', 'bar']);
=> false
'''

is.boolean(value:any)
---------------------
####Checks if the given value type is boolean.
interfaces: not, all, any

'''javascript
is.boolean(true);
=> true
...
```

#### <a name="apidoc.element.is_js.any.caPostalCode"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>caPostalCode ()](#apidoc.element.is_js.any.caPostalCode)
- description and source-code
```javascript
caPostalCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.usZipCode(['02201-1020', '123']);
=> false
'''

is.caPostalCode(value:any)
--------------------------
####Checks if the given value matches Canada postal code regexp.
interfaces: not, all, any

'''javascript
is.caPostalCode('L8V3Y1');
=> true
...
```

#### <a name="apidoc.element.is_js.any.capitalized"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>capitalized ()](#apidoc.element.is_js.any.capitalized)
- description and source-code
```javascript
capitalized = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.not.endWith('nope not that', 'not');
=> true

is.endWith('yeap that one', 'one');
=> true
'''

is.capitalized(value:string)
---------------------------------------------
####Checks if the given string is capitalized.
interfaces: not, all, any

'''javascript
is.capitalized('Yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.any.char"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>char ()](#apidoc.element.is_js.any.char)
- description and source-code
```javascript
char = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.string([{}, 'foo']);
=> false
'''

is.char(value:any)
--------------------
####Checks if the given value type is char.
interfaces: not, all, any

'''javascript
is.char('f');
=> true
...
```

#### <a name="apidoc.element.is_js.any.creditCard"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>creditCard ()](#apidoc.element.is_js.any.creditCard)
- description and source-code
```javascript
creditCard = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.email(['test@test.com', 'foo', undefined]);
=> false
'''

is.creditCard(value:any)
------------------------
####Checks if the given value matches credit card regexp.
interfaces: not, all, any

'''javascript
is.creditCard(378282246310005);
=> true
...
```

#### <a name="apidoc.element.is_js.any.date"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>date ()](#apidoc.element.is_js.any.date)
- description and source-code
```javascript
date = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.boolean([true, 'foo', 'bar']);
=> false
'''

is.date(value:any)
------------------
####Checks if the given value type is date.
interfaces: not, all, any

'''javascript
is.date(new Date());
=> true
...
```

#### <a name="apidoc.element.is_js.any.dateString"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>dateString ()](#apidoc.element.is_js.any.dateString)
- description and source-code
```javascript
dateString = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.timeString(['13:45:30', '90:90:90']);
=> false
'''

is.dateString(value:any)
------------------------
####Checks if the given value matches date string regexp.
interfaces: not, all, any

'''javascript
is.dateString('11/11/2011');
=> true
...
```

#### <a name="apidoc.element.is_js.any.dayLightSavingTime"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>dayLightSavingTime ()](#apidoc.element.is_js.any.dayLightSavingTime)
- description and source-code
```javascript
dayLightSavingTime = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.quarterOfYear(secondQuarter, 1);
=> false

is.not.quarterOfYear(secondQuarter, 1);
=> true
'''

is.dayLightSavingTime(value:date)
--------------------------------------------------
####Checks if the given date is in daylight saving time.
interface: not

'''javascript
// For Turkey Time Zone
var january1 = new Date('01/01/2015');
...
```

#### <a name="apidoc.element.is_js.any.decimal"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>decimal ()](#apidoc.element.is_js.any.decimal)
- description and source-code
```javascript
decimal = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.within(30, 20, 40);
=> true

is.not.within(40, 30, 35);
=> true
'''

is.decimal(value:number)
------------------------
####Checks if the given value is decimal.
interfaces: not, all, any

'''javascript
is.decimal(41.5);
=> true
...
```

#### <a name="apidoc.element.is_js.any.domNode"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>domNode ()](#apidoc.element.is_js.any.domNode)
- description and source-code
```javascript
domNode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.date([new Date(), 'foo', 'bar']);
=> false
'''

is.domNode(value:any)
-----------------------------
####Checks if the given object is a dom node.
interfaces: not, all, any

'''javascript
var obj = document.createElement('div');
is.domNode(obj);
...
```

#### <a name="apidoc.element.is_js.any.email"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>email ()](#apidoc.element.is_js.any.email)
- description and source-code
```javascript
email = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.url(['http://www.test.com', 'foo', undefined]);
=> false
'''

is.email(value:any)
-------------------
####Checks if the given value matches email regexp.
interfaces: not, all, any

'''javascript
is.email('test@test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.any.empty"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>empty ()](#apidoc.element.is_js.any.empty)
- description and source-code
```javascript
empty = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.all.windowObject([window, {nope: 'nope'}]);
=> false
'''

Presence checks
===============

is.empty(value:array|object|string)
-----------------------------------
####Checks if the given value is empty.
interfaces: not, all, any

'''javascript
is.empty({});
=> true
...
```

#### <a name="apidoc.element.is_js.any.eppPhone"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>eppPhone ()](#apidoc.element.is_js.any.eppPhone)
- description and source-code
```javascript
eppPhone = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nanpPhone(['609-555-0175', '123']);
=> false
'''

is.eppPhone(value:any)
----------------------
####Checks if the given value matches extensible provisioning protocol phone regexp.
interfaces: not, all, any

'''javascript
is.eppPhone('+90.2322456789');
=> true
...
```

#### <a name="apidoc.element.is_js.any.error"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>error ()](#apidoc.element.is_js.any.error)
- description and source-code
```javascript
error = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.domNode([obj, {nope: 'nope'}]);
=> false
'''

is.error(value:any)
-------------------
####Checks if the given value type is error.
interfaces: not, all, any

'''javascript
is.error(new Error());
=> true
...
```

#### <a name="apidoc.element.is_js.any.even"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>even ()](#apidoc.element.is_js.any.even)
- description and source-code
```javascript
even = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.equal(true, true);
=> true

is.not.equal('yeap', 'nope');
=> true
'''

is.even(value:number)
---------------------
####Checks if the given value is even.
interfaces: not, all, any

'''javascript
is.even(42);
=> true
...
```

#### <a name="apidoc.element.is_js.any.existy"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>existy ()](#apidoc.element.is_js.any.existy)
- description and source-code
```javascript
existy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.empty([{}, 'foo']);
=> false
'''

is.existy(value:any)
--------------------
####Checks if the given value is existy. (not null or undefined)
interfaces: not, all, any

'''javascript
is.existy({});
=> true
...
```

#### <a name="apidoc.element.is_js.any.falsy"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>falsy ()](#apidoc.element.is_js.any.falsy)
- description and source-code
```javascript
falsy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.truthy([{}, true]);
=> true
'''

is.falsy(value:any)
-------------------
####Checks if the given value is falsy.
interfaces: not, all, any

'''javascript
is.falsy(false);
=> true
...
```

#### <a name="apidoc.element.is_js.any.finite"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>finite ()](#apidoc.element.is_js.any.finite)
- description and source-code
```javascript
finite = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.integer([40, 42.5, -43]);
=> false
'''

is.finite(value:number)
-----------------------
####Checks if the given value is finite.
interfaces: not, all, any

'''javascript
is.finite(41);
=> true
...
```

#### <a name="apidoc.element.is_js.any.function"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>function ()](#apidoc.element.is_js.any.function)
- description and source-code
```javascript
function = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.error([new Error(), 'foo', 'bar']);
=> false
'''

is.function(value:any)
----------------------
####Checks if the given value type is function.
interfaces: not, all, any

'''javascript
is.function(toString);
=> true
...
```

#### <a name="apidoc.element.is_js.any.future"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>future ()](#apidoc.element.is_js.any.future)
- description and source-code
```javascript
future = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.past([yesterday, tomorrow]);
=> false
'''

is.future(value:date)
-----------------------
####Checks if the given date object indicate future.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.any.hexColor"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>hexColor ()](#apidoc.element.is_js.any.hexColor)
- description and source-code
```javascript
hexColor = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.hexadecimal(['fff', '333', 'f50']);
=> true
'''

is.hexColor(value:any)
-------------------------
####Checks if the given value matches hexcolor regexp.
interfaces: not, all, any

'''javascript
is.hexColor('#333');
=> true
...
```

#### <a name="apidoc.element.is_js.any.hexadecimal"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>hexadecimal ()](#apidoc.element.is_js.any.hexadecimal)
- description and source-code
```javascript
hexadecimal = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.affirmative(['yes', 'y', 'true', 't', 'ok', 'okay']);
=> true
'''

is.hexadecimal(value:any)
-------------------------
####Checks if the given value matches hexadecimal regexp.
interfaces: not, all, any

'''javascript
is.hexadecimal('f0f0f0');
=> true
...
```

#### <a name="apidoc.element.is_js.any.inLastMonth"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inLastMonth ()](#apidoc.element.is_js.any.inLastMonth)
- description and source-code
```javascript
inLastMonth = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inLastWeek(nineDaysAgo);
=> false

is.not.inLastWeek(nineDaysAgo);
=> true
'''

is.inLastMonth(value:date)
----------------------------
####Checks if the given date is between now and a month ago.
interface: not

'''javascript
var tenDaysAgo = new Date(new Date().setDate(new Date().getDate() - 10));
var fortyDaysAgo = new Date(new Date().setDate(new Date().getDate() - 40));
...
```

#### <a name="apidoc.element.is_js.any.inLastWeek"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inLastWeek ()](#apidoc.element.is_js.any.inLastWeek)
- description and source-code
```javascript
inLastWeek = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inDateRange(saturday, sunday, monday);
=> false

is.not.inDateRange(saturday, sunday, monday);
=> true
'''

is.inLastWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days ago.
interface: not

'''javascript
var twoDaysAgo = new Date(new Date().setDate(new Date().getDate() - 2));
var nineDaysAgo = new Date(new Date().setDate(new Date().getDate() - 9));
...
```

#### <a name="apidoc.element.is_js.any.inLastYear"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inLastYear ()](#apidoc.element.is_js.any.inLastYear)
- description and source-code
```javascript
inLastYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inLastMonth(fortyDaysAgo);
=> false

is.not.inLastMonth(fortyDaysAgo);
=> true
'''

is.inLastYear(value:date)
---------------------------
####Checks if the given date is between now and a year ago.
interface: not

'''javascript
var twoMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 2));
var thirteenMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 13));
...
```

#### <a name="apidoc.element.is_js.any.inNextMonth"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inNextMonth ()](#apidoc.element.is_js.any.inNextMonth)
- description and source-code
```javascript
inNextMonth = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inNextWeek(nineDaysLater);
=> false

is.not.inNextWeek(nineDaysLater);
=> true
'''

is.inNextMonth(value:date)
----------------------------
####Checks if the given date is between now and a month later.
interface: not

'''javascript
var tenDaysLater = new Date(new Date().setDate(new Date().getDate() + 10));
var fortyDaysLater = new Date(new Date().setDate(new Date().getDate() + 40));
...
```

#### <a name="apidoc.element.is_js.any.inNextWeek"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inNextWeek ()](#apidoc.element.is_js.any.inNextWeek)
- description and source-code
```javascript
inNextWeek = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inLastYear(thirteenMonthsAgo);
=> false

is.not.inLastYear(thirteenMonthsAgo);
=> true
'''

is.inNextWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days later.
interface: not

'''javascript
var twoDaysLater = new Date(new Date().setDate(new Date().getDate() + 2));
var nineDaysLater = new Date(new Date().setDate(new Date().getDate() + 9));
...
```

#### <a name="apidoc.element.is_js.any.inNextYear"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>inNextYear ()](#apidoc.element.is_js.any.inNextYear)
- description and source-code
```javascript
inNextYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inNextMonth(fortyDaysLater);
=> false

is.not.inNextMonth(fortyDaysLater);
=> true
'''

is.inNextYear(value:date)
---------------------------
####Checks if the given date is between now and a year later.
interface: not

'''javascript
var twoMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 2));
var thirteenMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 13));
...
```

#### <a name="apidoc.element.is_js.any.infinite"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>infinite ()](#apidoc.element.is_js.any.infinite)
- description and source-code
```javascript
infinite = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.finite([Infinity, -Infinity, 42.5]);
=> false
'''

is.infinite(value:number)
-------------------------
####Checks if the given value is infinite.
interfaces: not, all, any

'''javascript
is.infinite(Infinity);
=> true
...
```

#### <a name="apidoc.element.is_js.any.integer"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>integer ()](#apidoc.element.is_js.any.integer)
- description and source-code
```javascript
integer = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.decimal([40, 42.5, -43]);
=> false
'''

is.integer(value:number)
------------------------
####Checks if the given value is integer.
interfaces: not, all, any

'''javascript
is.integer(41);
=> true
...
```

#### <a name="apidoc.element.is_js.any.ip"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>ip ()](#apidoc.element.is_js.any.ip)
- description and source-code
```javascript
ip = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> false

// 'all' and 'any' interfaces can also take array parameter
is.all.hexColor(['fff', '333', 'f50']);
=> true
'''

is.ip(value:any)
-------------------------
####Checks if the given value matches ip regexp
interfaces: not, all, any

'''javascript
is.ip('198.156.23.5');
=> true
...
```

#### <a name="apidoc.element.is_js.any.ipv4"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>ipv4 ()](#apidoc.element.is_js.any.ipv4)
- description and source-code
```javascript
ipv4 = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ip(['123.123.23.12', 'A:B:C:D:E:F:0:0']);
=> true
'''

is.ipv4(value:any)
-------------------------
####Checks if the given value matches ipv4 regexp
interfaces: not, all, any

'''javascript
is.ipv4('198.12.3.142');
=> true
...
```

#### <a name="apidoc.element.is_js.any.ipv6"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>ipv6 ()](#apidoc.element.is_js.any.ipv6)
- description and source-code
```javascript
ipv6 = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.ipv4(['198.12.3.142', '1.2.3']);
=> false

'''

is.ipv6(value:any)
-------------------------
####Checks if the given value matches ipv6 regexp
interfaces: not, all, any

'''javascript
is.ipv6('2001:DB8:0:0:1::1');
=> true
...
```

#### <a name="apidoc.element.is_js.any.json"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>json ()](#apidoc.element.is_js.any.json)
- description and source-code
```javascript
json = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.object([{}, new Object()]);
=> true
'''

is.json(value:any)
--------------------
####Checks if the given value type is pure json object.
interfaces: not, all, any

'''javascript
is.json({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.any.leapYear"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>leapYear ()](#apidoc.element.is_js.any.leapYear)
- description and source-code
```javascript
leapYear = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.year(year2016, 2015);
=> false

is.not.year(year2016, 2015);
=> true
'''

is.leapYear(value:number)
---------------------------------
####Checks if the given year number is a leap year
interfaces: not, all, any

'''javascript
is.leapYear(2016);
=> true
...
```

#### <a name="apidoc.element.is_js.any.lowerCase"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>lowerCase ()](#apidoc.element.is_js.any.lowerCase)
- description and source-code
```javascript
lowerCase = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.upperCase(['YEAP', 'ALL UPPERCASE']);
=> true
'''


is.lowerCase(value:string)
--------------------------
####Checks if the given string is lowercase.
interfaces: not, all, any

'''javascript
is.lowerCase('yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.any.nan"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>nan ()](#apidoc.element.is_js.any.nan)
- description and source-code
```javascript
nan = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.function([toString, 'foo', 'bar']);
=> false
'''

is.nan(value:any)
-----------------
####Checks if the given value type is NaN.
interfaces: not, all, any

'''javascript
is.nan(NaN);
=> true
...
```

#### <a name="apidoc.element.is_js.any.nanpPhone"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>nanpPhone ()](#apidoc.element.is_js.any.nanpPhone)
- description and source-code
```javascript
nanpPhone = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ukPostCode(['B184BJ', '123']);
=> false
'''

is.nanpPhone(value:any)
-----------------------
####Checks if the given value matches North American numbering plan phone regexp.
interfaces: not, all, any

'''javascript
is.nanpPhone('609-555-0175');
=> true
...
```

#### <a name="apidoc.element.is_js.any.negative"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>negative ()](#apidoc.element.is_js.any.negative)
- description and source-code
```javascript
negative = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.positive([40, 42, -43]);
=> false
'''

is.negative(value:number)
-------------------------
####Checks if the given value is negative.
interfaces: not, all, any

'''javascript
is.negative(-41);
=> true
...
```

#### <a name="apidoc.element.is_js.any.null"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>null ()](#apidoc.element.is_js.any.null)
- description and source-code
```javascript
null = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nan([NaN, 'foo', 1]);
=> false
'''

is.null(value:any)
------------------
####Checks if the given value type is null.
interfaces: not, all, any

'''javascript
is.null(null);
=> true
...
```

#### <a name="apidoc.element.is_js.any.number"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>number ()](#apidoc.element.is_js.any.number)
- description and source-code
```javascript
number = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.null([null, 'foo', 1]);
=> false
'''

is.number(value:any)
--------------------
####Checks if the given value type is number.
interfaces: not, all, any

'''javascript
is.number(42);
=> true
...
```

#### <a name="apidoc.element.is_js.any.object"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>object ()](#apidoc.element.is_js.any.object)
- description and source-code
```javascript
object = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.number([42, 'foo', 1]);
=> false
'''

is.object(value:any)
--------------------
####Checks if the given value type is object.
interfaces: not, all, any

'''javascript
is.object({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.any.odd"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>odd ()](#apidoc.element.is_js.any.odd)
- description and source-code
```javascript
odd = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.even([40, 42, 43]);
=> false
'''

is.odd(value:number)
--------------------
####Checks if the given value is odd.
interfaces: not, all, any

'''javascript
is.odd(41);
=> true
...
```

#### <a name="apidoc.element.is_js.any.palindrome"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>palindrome ()](#apidoc.element.is_js.any.palindrome)
- description and source-code
```javascript
palindrome = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.capitalized(['Nope', 'not']);
=> false
'''

is.palindrome(value:string)
---------------------------------------------
####Checks if the given string is palindrome.
interfaces: not, all, any

'''javascript
is.palindrome('testset');
=> true
...
```

#### <a name="apidoc.element.is_js.any.past"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>past ()](#apidoc.element.is_js.any.past)
- description and source-code
```javascript
past = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.tomorrow([today, tomorrow]);
=> false
'''

is.past(value:date)
---------------------
####Checks if the given date object indicate past.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.any.positive"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>positive ()](#apidoc.element.is_js.any.positive)
- description and source-code
```javascript
positive = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.odd([40, 42, 43]);
=> false
'''

is.positive(value:number)
-------------------------
####Checks if the given value is positive.
interfaces: not, all, any

'''javascript
is.positive(41);
=> true
...
```

#### <a name="apidoc.element.is_js.any.regexp"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>regexp ()](#apidoc.element.is_js.any.regexp)
- description and source-code
```javascript
regexp = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.json([{}, {foo: 'bar'}]);
=> true
'''

is.regexp(value:any)
--------------------
####Checks if the given value type is RegExp.
interfaces: not, all, any

'''javascript
is.regexp(/test/);
=> true
...
```

#### <a name="apidoc.element.is_js.any.socialSecurityNumber"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>socialSecurityNumber ()](#apidoc.element.is_js.any.socialSecurityNumber)
- description and source-code
```javascript
socialSecurityNumber = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.eppPhone(['+90.2322456789', '123']);
=> false
'''

is.socialSecurityNumber(value:any)
----------------------------------
####Checks if the given value matches social security number regexp.
interfaces: not, all, any

'''javascript
is.socialSecurityNumber('017-90-7890');
=> true
...
```

#### <a name="apidoc.element.is_js.any.sorted"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>sorted ()](#apidoc.element.is_js.any.sorted)
- description and source-code
```javascript
sorted = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.inArray(4, [1, 2, 3]);
=> false

is.not.inArray(4, [1, 2, 3]);
=> true
'''

is.sorted(value:array, sign:string)
----------------------
####Checks if the given array is sorted. Sign is optional parameter.
interfaces: not, all, any

'''javascript
is.sorted([1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.any.space"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>space ()](#apidoc.element.is_js.any.space)
- description and source-code
```javascript
space = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.falsy([false, true, undefined]);
=> false
'''

is.space(value:any)
----------------------
####Checks if the given value is space.
interfaces: not, all, any

'''javascript
is.space(' ');
=> true
...
```

#### <a name="apidoc.element.is_js.any.string"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>string ()](#apidoc.element.is_js.any.string)
- description and source-code
```javascript
string = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.regexp([{}, /test/]);
=> false
'''

is.string(value:any)
--------------------
####Checks if the given value type is string.
interfaces: not, all, any

'''javascript
is.string('foo');
=> true
...
```

#### <a name="apidoc.element.is_js.any.timeString"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>timeString ()](#apidoc.element.is_js.any.timeString)
- description and source-code
```javascript
timeString = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.alphaNumeric(['alphaNu3er1k', '*?']);
=> false
'''

is.timeString(value:any)
------------------------
####Checks if the given value matches time string regexp.
interfaces: not, all, any

'''javascript
is.timeString('13:45:30');
=> true
...
```

#### <a name="apidoc.element.is_js.any.today"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>today ()](#apidoc.element.is_js.any.today)
- description and source-code
```javascript
today = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.not.touchDevice();
=> true if current device does not support touch
'''

Time checks
===========

is.today(value:date)
----------------------
####Checks if the given date object indicate today.
interfaces: not, all, any

'''javascript
var today = new Date();
is.today(today);
...
```

#### <a name="apidoc.element.is_js.any.tomorrow"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>tomorrow ()](#apidoc.element.is_js.any.tomorrow)
- description and source-code
```javascript
tomorrow = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.yesterday([today, yesterday]);
=> false
'''

is.tomorrow(value:date)
-------------------------
####Checks if the given date object indicate tomorrow.
interfaces: not, all, any

'''javascript
var today = new Date();
is.tomorrow(today);
...
```

#### <a name="apidoc.element.is_js.any.truthy"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>truthy ()](#apidoc.element.is_js.any.truthy)
- description and source-code
```javascript
truthy = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.existy([{}, 'foo']);
=> true
'''

is.truthy(value:any)
--------------------
####Checks if the given value is truthy. (existy and not false)
interfaces: not, all, any

'''javascript
is.truthy(true);
=> true
...
```

#### <a name="apidoc.element.is_js.any.ukPostCode"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>ukPostCode ()](#apidoc.element.is_js.any.ukPostCode)
- description and source-code
```javascript
ukPostCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.caPostalCode(['L8V3Y1', '123']);
=> false
'''

is.ukPostCode(value:any)
------------------------
####Checks if the given value matches UK post code regexp.
interfaces: not, all, any

'''javascript
is.ukPostCode('B184BJ');
=> true
...
```

#### <a name="apidoc.element.is_js.any.undefined"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>undefined ()](#apidoc.element.is_js.any.undefined)
- description and source-code
```javascript
undefined = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.char(['f', 'o', 'o']);
=> true
'''

is.undefined(value:any)
-----------------------
####Checks if the given value type is undefined.
interfaces: not, all, any

'''javascript
is.undefined(undefined);
=> true
...
```

#### <a name="apidoc.element.is_js.any.upperCase"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>upperCase ()](#apidoc.element.is_js.any.upperCase)
- description and source-code
```javascript
upperCase = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.include('test', 'text');
=> false

is.not.include('test', 'text');
=> true
'''

is.upperCase(value:string)
--------------------------
####Checks if the given string is UPPERCASE.
interfaces: not, all, any

'''javascript
is.upperCase('YEAP');
=> true
...
```

#### <a name="apidoc.element.is_js.any.url"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>url ()](#apidoc.element.is_js.any.url)
- description and source-code
```javascript
url = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.all.space([' ', 'foo', undefined]);
=> false
'''

RegExp checks
=============

is.url(value:any)
-----------------
####Checks if the given value matches url regexp.
interfaces: not, all, any

'''javascript
is.url('http://www.test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.any.usZipCode"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>usZipCode ()](#apidoc.element.is_js.any.usZipCode)
- description and source-code
```javascript
usZipCode = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.dateString(['11/11/2011', '90/11/2011']);
=> false
'''

is.usZipCode(value:any)
-----------------------
####Checks if the given value matches US zip code regexp.
interfaces: not, all, any

'''javascript
is.usZipCode('02201-1020');
=> true
...
```

#### <a name="apidoc.element.is_js.any.weekday"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>weekday ()](#apidoc.element.is_js.any.weekday)
- description and source-code
```javascript
weekday = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekend([sunday, saturday, monday]);
=> false
'''

is.weekday(value:date)
------------------------
####Checks if the given date objects' day is weekday.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.any.weekend"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>weekend ()](#apidoc.element.is_js.any.weekend)
- description and source-code
```javascript
weekend = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.leapYear([2016, 2080]);
=> true
'''

is.weekend(value:date)
------------------------
####Checks if the given date objects' day is weekend.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.any.windowObject"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>windowObject ()](#apidoc.element.is_js.any.windowObject)
- description and source-code
```javascript
windowObject = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
is.sameType(42, '7');
=> false

is.not.sameType(42, 7);
=> false
'''

is.windowObject(value:any)
-----------------------------
####Checks if the given object is window object.
interfaces: not, all, any

'''javascript
is.windowObject(window);
=> true
...
```

#### <a name="apidoc.element.is_js.any.yesterday"></a>[function <span class="apidocSignatureSpan">is_js.any.</span>yesterday ()](#apidoc.element.is_js.any.yesterday)
- description and source-code
```javascript
yesterday = function () {
    var params = getParams(arguments);
    var length = params.length;
    for (var i = 0; i < length; i++) {
        if (func.call(null, params[i])) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.today([today, yesterday]);
=> false
'''

is.yesterday(value:date)
--------------------------
####Checks if the given date object indicate yesterday.
interfaces: not, all, any

'''javascript
var today = new Date();
is.yesterday(today);
...
```



# <a name="apidoc.module.is_js.not"></a>[module is_js.not](#apidoc.module.is_js.not)

#### <a name="apidoc.element.is_js.not.above"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>above ()](#apidoc.element.is_js.not.above)
- description and source-code
```javascript
above = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.negative([40, 42, -43]);
=> false
'''

is.above(value:number, min:number)
---------------------------
####Checks if the given value is above minimum value.
interface: not

'''javascript
is.above(41, 30);
=> true
...
```

#### <a name="apidoc.element.is_js.not.affirmative"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>affirmative ()](#apidoc.element.is_js.not.affirmative)
- description and source-code
```javascript
affirmative = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.socialSecurityNumber(['017-90-7890', '123']);
=> false
'''

is.affirmative(value:any)
-------------------------
####Checks if the given value matches affirmative regexp.
interfaces: not, all, any

'''javascript
is.affirmative('yes');
=> true
...
```

#### <a name="apidoc.element.is_js.not.alphaNumeric"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>alphaNumeric ()](#apidoc.element.is_js.not.alphaNumeric)
- description and source-code
```javascript
alphaNumeric = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.creditCard([378282246310005, 123, undefined]);
=> false
'''

is.alphaNumeric(value:any)
--------------------------
####Checks if the given value matches alpha numeric regexp.
interfaces: not, all, any

'''javascript
is.alphaNumeric('alphaNu3er1k');
=> true
...
```

#### <a name="apidoc.element.is_js.not.android"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>android ()](#apidoc.element.is_js.not.android)
- description and source-code
```javascript
android = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.ipod('>=5');
=> true if current version of iPod is greater than or equal to 5

is.not.ipod('<5');
=> true if current version of iPod is not less than 5
'''

is.android()
------------
####Checks if current device has Android.
interface: not

'''javascript
is.android();
=> true if current device has Android OS
...
```

#### <a name="apidoc.element.is_js.not.androidPhone"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>androidPhone ()](#apidoc.element.is_js.not.androidPhone)
- description and source-code
```javascript
androidPhone = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.android();
=> true if current device has Android OS

is.not.android();
=> true if current device has not Android OS
'''

is.androidPhone()
-----------------
####Checks if current device is Android phone.
interface: not

'''javascript
is.androidPhone();
=> true if current device is Android phone
...
```

#### <a name="apidoc.element.is_js.not.androidTablet"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>androidTablet ()](#apidoc.element.is_js.not.androidTablet)
- description and source-code
```javascript
androidTablet = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.androidPhone();
=> true if current device is Android phone

is.not.androidPhone();
=> true if current device is not Android phone
'''

is.androidTablet()
------------------
####Checks if current device is Android tablet.
interface: not

'''javascript
is.androidTablet();
=> true if current device is Android tablet
...
```

#### <a name="apidoc.element.is_js.not.arguments"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>arguments ()](#apidoc.element.is_js.not.arguments)
- description and source-code
```javascript
arguments = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...

####Contributors:
Many thanks to our contributors: https://github.com/arasatasaygin/is.js/graphs/contributors

Type checks
===========

is.arguments(value:any)
-----------------------
####Checks if the given value type is arguments.
interfaces: not, all, any

'''javascript
var getArguments = function() {
return arguments;
...
```

#### <a name="apidoc.element.is_js.not.array"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>array ()](#apidoc.element.is_js.not.array)
- description and source-code
```javascript
array = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.arguments([arguments, 'foo', 'bar']);
=> false
'''

is.array(value:any)
-------------------
####Checks if the given value type is array.
interfaces: not, all, any

'''javascript
is.array(['foo', 'bar', 'baz']);
=> true
...
```

#### <a name="apidoc.element.is_js.not.blackberry"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>blackberry ()](#apidoc.element.is_js.not.blackberry)
- description and source-code
```javascript
blackberry = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.androidTablet();
=> true if current device is Android tablet

is.not.androidTablet();
=> true if current device is not Android tablet
'''

is.blackberry()
---------------
####Checks if current device is Blackberry.
interface: not

'''javascript
is.blackberry();
=> true if current device is Blackberry
...
```

#### <a name="apidoc.element.is_js.not.boolean"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>boolean ()](#apidoc.element.is_js.not.boolean)
- description and source-code
```javascript
boolean = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.array([[1, 2], 'foo', 'bar']);
=> false
'''

is.boolean(value:any)
---------------------
####Checks if the given value type is boolean.
interfaces: not, all, any

'''javascript
is.boolean(true);
=> true
...
```

#### <a name="apidoc.element.is_js.not.caPostalCode"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>caPostalCode ()](#apidoc.element.is_js.not.caPostalCode)
- description and source-code
```javascript
caPostalCode = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.usZipCode(['02201-1020', '123']);
=> false
'''

is.caPostalCode(value:any)
--------------------------
####Checks if the given value matches Canada postal code regexp.
interfaces: not, all, any

'''javascript
is.caPostalCode('L8V3Y1');
=> true
...
```

#### <a name="apidoc.element.is_js.not.capitalized"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>capitalized ()](#apidoc.element.is_js.not.capitalized)
- description and source-code
```javascript
capitalized = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.not.endWith('nope not that', 'not');
=> true

is.endWith('yeap that one', 'one');
=> true
'''

is.capitalized(value:string)
---------------------------------------------
####Checks if the given string is capitalized.
interfaces: not, all, any

'''javascript
is.capitalized('Yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.not.char"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>char ()](#apidoc.element.is_js.not.char)
- description and source-code
```javascript
char = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.string([{}, 'foo']);
=> false
'''

is.char(value:any)
--------------------
####Checks if the given value type is char.
interfaces: not, all, any

'''javascript
is.char('f');
=> true
...
```

#### <a name="apidoc.element.is_js.not.chrome"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>chrome ()](#apidoc.element.is_js.not.chrome)
- description and source-code
```javascript
chrome = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.ie('>=10');
=> true if current version of ie is greater than or equal to 10

is.not.ie('<9');
=> true if current version of ie is not less than 9
'''

is.chrome(range:number|string)
-----------
####Checks if current browser is chrome. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.chrome();
=> true if current browser is chrome
...
```

#### <a name="apidoc.element.is_js.not.creditCard"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>creditCard ()](#apidoc.element.is_js.not.creditCard)
- description and source-code
```javascript
creditCard = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.email(['test@test.com', 'foo', undefined]);
=> false
'''

is.creditCard(value:any)
------------------------
####Checks if the given value matches credit card regexp.
interfaces: not, all, any

'''javascript
is.creditCard(378282246310005);
=> true
...
```

#### <a name="apidoc.element.is_js.not.date"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>date ()](#apidoc.element.is_js.not.date)
- description and source-code
```javascript
date = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.boolean([true, 'foo', 'bar']);
=> false
'''

is.date(value:any)
------------------
####Checks if the given value type is date.
interfaces: not, all, any

'''javascript
is.date(new Date());
=> true
...
```

#### <a name="apidoc.element.is_js.not.dateString"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>dateString ()](#apidoc.element.is_js.not.dateString)
- description and source-code
```javascript
dateString = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.timeString(['13:45:30', '90:90:90']);
=> false
'''

is.dateString(value:any)
------------------------
####Checks if the given value matches date string regexp.
interfaces: not, all, any

'''javascript
is.dateString('11/11/2011');
=> true
...
```

#### <a name="apidoc.element.is_js.not.day"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>day ()](#apidoc.element.is_js.not.day)
- description and source-code
```javascript
day = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.future([yesterday, tomorrow]);
=> false
'''

is.day(value:date, day:string)
-------------------------------
####Checks if the given date objects' day equal given dayString parameter.
interface: not

'''javascript
var mondayObj = new Date('01/26/2015');
var tuesdayObj = new Date('01/27/2015');
...
```

#### <a name="apidoc.element.is_js.not.dayLightSavingTime"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>dayLightSavingTime ()](#apidoc.element.is_js.not.dayLightSavingTime)
- description and source-code
```javascript
dayLightSavingTime = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.quarterOfYear(secondQuarter, 1);
=> false

is.not.quarterOfYear(secondQuarter, 1);
=> true
'''

is.dayLightSavingTime(value:date)
--------------------------------------------------
####Checks if the given date is in daylight saving time.
interface: not

'''javascript
// For Turkey Time Zone
var january1 = new Date('01/01/2015');
...
```

#### <a name="apidoc.element.is_js.not.decimal"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>decimal ()](#apidoc.element.is_js.not.decimal)
- description and source-code
```javascript
decimal = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.within(30, 20, 40);
=> true

is.not.within(40, 30, 35);
=> true
'''

is.decimal(value:number)
------------------------
####Checks if the given value is decimal.
interfaces: not, all, any

'''javascript
is.decimal(41.5);
=> true
...
```

#### <a name="apidoc.element.is_js.not.desktop"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>desktop ()](#apidoc.element.is_js.not.desktop)
- description and source-code
```javascript
desktop = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.linux();
=> true if current OS is linux

is.not.linux();
=> true if current OS is not linux
'''

is.desktop()
------------
####Checks if current device is desktop.
interface: not

'''javascript
is.desktop();
=> true if current device is desktop
...
```

#### <a name="apidoc.element.is_js.not.domNode"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>domNode ()](#apidoc.element.is_js.not.domNode)
- description and source-code
```javascript
domNode = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.date([new Date(), 'foo', 'bar']);
=> false
'''

is.domNode(value:any)
-----------------------------
####Checks if the given object is a dom node.
interfaces: not, all, any

'''javascript
var obj = document.createElement('div');
is.domNode(obj);
...
```

#### <a name="apidoc.element.is_js.not.edge"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>edge ()](#apidoc.element.is_js.not.edge)
- description and source-code
```javascript
edge = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.firefox('>=40');
=> true if current version of firefox is greater than or equal to 40

is.not.firefox('<30');
=> true if current version of firefox is not less than 30
'''

is.edge(range:number|string)
------------
####Checks if current browser is edge. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.edge();
=> true if current browser is edge
...
```

#### <a name="apidoc.element.is_js.not.email"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>email ()](#apidoc.element.is_js.not.email)
- description and source-code
```javascript
email = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.url(['http://www.test.com', 'foo', undefined]);
=> false
'''

is.email(value:any)
-------------------
####Checks if the given value matches email regexp.
interfaces: not, all, any

'''javascript
is.email('test@test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.not.empty"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>empty ()](#apidoc.element.is_js.not.empty)
- description and source-code
```javascript
empty = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.all.windowObject([window, {nope: 'nope'}]);
=> false
'''

Presence checks
===============

is.empty(value:array|object|string)
-----------------------------------
####Checks if the given value is empty.
interfaces: not, all, any

'''javascript
is.empty({});
=> true
...
```

#### <a name="apidoc.element.is_js.not.endWith"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>endWith ()](#apidoc.element.is_js.not.endWith)
- description and source-code
```javascript
endWith = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.startWith('nope', 'ye');
=> false

is.not.startWith('nope not that', 'not');
=> true
'''

is.endWith(value:string, target:string)
-----------------------------------------
####Checks if the given string ends with substring.
interfaces: not

'''javascript
is.endWith('yeap', 'ap');
=> true
...
```

#### <a name="apidoc.element.is_js.not.eppPhone"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>eppPhone ()](#apidoc.element.is_js.not.eppPhone)
- description and source-code
```javascript
eppPhone = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nanpPhone(['609-555-0175', '123']);
=> false
'''

is.eppPhone(value:any)
----------------------
####Checks if the given value matches extensible provisioning protocol phone regexp.
interfaces: not, all, any

'''javascript
is.eppPhone('+90.2322456789');
=> true
...
```

#### <a name="apidoc.element.is_js.not.equal"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>equal ()](#apidoc.element.is_js.not.equal)
- description and source-code
```javascript
equal = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.all.palindrome(['Nope', 'testset']);
=> false
'''

Arithmetic checks
=================

is.equal(value:any, other:any)
------------------------------
####Checks if the given values are equal.
interfaces: not

'''javascript
is.equal(42, 40 + 2);
=> true
...
```

#### <a name="apidoc.element.is_js.not.error"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>error ()](#apidoc.element.is_js.not.error)
- description and source-code
```javascript
error = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.domNode([obj, {nope: 'nope'}]);
=> false
'''

is.error(value:any)
-------------------
####Checks if the given value type is error.
interfaces: not, all, any

'''javascript
is.error(new Error());
=> true
...
```

#### <a name="apidoc.element.is_js.not.even"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>even ()](#apidoc.element.is_js.not.even)
- description and source-code
```javascript
even = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.equal(true, true);
=> true

is.not.equal('yeap', 'nope');
=> true
'''

is.even(value:number)
---------------------
####Checks if the given value is even.
interfaces: not, all, any

'''javascript
is.even(42);
=> true
...
```

#### <a name="apidoc.element.is_js.not.existy"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>existy ()](#apidoc.element.is_js.not.existy)
- description and source-code
```javascript
existy = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.empty([{}, 'foo']);
=> false
'''

is.existy(value:any)
--------------------
####Checks if the given value is existy. (not null or undefined)
interfaces: not, all, any

'''javascript
is.existy({});
=> true
...
```

#### <a name="apidoc.element.is_js.not.falsy"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>falsy ()](#apidoc.element.is_js.not.falsy)
- description and source-code
```javascript
falsy = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.truthy([{}, true]);
=> true
'''

is.falsy(value:any)
-------------------
####Checks if the given value is falsy.
interfaces: not, all, any

'''javascript
is.falsy(false);
=> true
...
```

#### <a name="apidoc.element.is_js.not.finite"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>finite ()](#apidoc.element.is_js.not.finite)
- description and source-code
```javascript
finite = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.integer([40, 42.5, -43]);
=> false
'''

is.finite(value:number)
-----------------------
####Checks if the given value is finite.
interfaces: not, all, any

'''javascript
is.finite(41);
=> true
...
```

#### <a name="apidoc.element.is_js.not.firefox"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>firefox ()](#apidoc.element.is_js.not.firefox)
- description and source-code
```javascript
firefox = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.chrome('>=40');
=> true if current version of chrome is greater than or equal to 40

is.not.chrome('<30');
=> true if current version of chrome is not less than 30
'''

is.firefox(range:number|string)
------------
####Checks if current browser is firefox. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.firefox();
=> true if current browser is firefox
...
```

#### <a name="apidoc.element.is_js.not.function"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>function ()](#apidoc.element.is_js.not.function)
- description and source-code
```javascript
function = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.error([new Error(), 'foo', 'bar']);
=> false
'''

is.function(value:any)
----------------------
####Checks if the given value type is function.
interfaces: not, all, any

'''javascript
is.function(toString);
=> true
...
```

#### <a name="apidoc.element.is_js.not.future"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>future ()](#apidoc.element.is_js.not.future)
- description and source-code
```javascript
future = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.past([yesterday, tomorrow]);
=> false
'''

is.future(value:date)
-----------------------
####Checks if the given date object indicate future.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.not.hexColor"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>hexColor ()](#apidoc.element.is_js.not.hexColor)
- description and source-code
```javascript
hexColor = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.hexadecimal(['fff', '333', 'f50']);
=> true
'''

is.hexColor(value:any)
-------------------------
####Checks if the given value matches hexcolor regexp.
interfaces: not, all, any

'''javascript
is.hexColor('#333');
=> true
...
```

#### <a name="apidoc.element.is_js.not.hexadecimal"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>hexadecimal ()](#apidoc.element.is_js.not.hexadecimal)
- description and source-code
```javascript
hexadecimal = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.affirmative(['yes', 'y', 'true', 't', 'ok', 'okay']);
=> true
'''

is.hexadecimal(value:any)
-------------------------
####Checks if the given value matches hexadecimal regexp.
interfaces: not, all, any

'''javascript
is.hexadecimal('f0f0f0');
=> true
...
```

#### <a name="apidoc.element.is_js.not.ie"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ie ()](#apidoc.element.is_js.not.ie)
- description and source-code
```javascript
ie = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> false
'''

Environment checks
==================
####Environment checks are not available as node module.

is.ie(range:number|string)
-------------------
####Checks if current browser is ie. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.ie();
=> true if current browser is ie
...
```

#### <a name="apidoc.element.is_js.not.inArray"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inArray ()](#apidoc.element.is_js.not.inArray)
- description and source-code
```javascript
inArray = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.not.propertyDefined({}, 'nope');
=> true
'''

Array checks
============

is.inArray(value:any, array)
---------------------
####Checks if the given item is in array?
interface: not
'''javascript
is.inArray(2, [1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.not.inDateRange"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inDateRange ()](#apidoc.element.is_js.not.inDateRange)
- description and source-code
```javascript
inDateRange = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekday([sunday, saturday, monday]);
=> false
'''

is.inDateRange(value:date, start:date, end:date)
----------------------------------------------------
####Checks if date is within given range.
interface: not

'''javascript
var saturday = new Date('01/24/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.not.inLastMonth"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inLastMonth ()](#apidoc.element.is_js.not.inLastMonth)
- description and source-code
```javascript
inLastMonth = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inLastWeek(nineDaysAgo);
=> false

is.not.inLastWeek(nineDaysAgo);
=> true
'''

is.inLastMonth(value:date)
----------------------------
####Checks if the given date is between now and a month ago.
interface: not

'''javascript
var tenDaysAgo = new Date(new Date().setDate(new Date().getDate() - 10));
var fortyDaysAgo = new Date(new Date().setDate(new Date().getDate() - 40));
...
```

#### <a name="apidoc.element.is_js.not.inLastWeek"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inLastWeek ()](#apidoc.element.is_js.not.inLastWeek)
- description and source-code
```javascript
inLastWeek = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inDateRange(saturday, sunday, monday);
=> false

is.not.inDateRange(saturday, sunday, monday);
=> true
'''

is.inLastWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days ago.
interface: not

'''javascript
var twoDaysAgo = new Date(new Date().setDate(new Date().getDate() - 2));
var nineDaysAgo = new Date(new Date().setDate(new Date().getDate() - 9));
...
```

#### <a name="apidoc.element.is_js.not.inLastYear"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inLastYear ()](#apidoc.element.is_js.not.inLastYear)
- description and source-code
```javascript
inLastYear = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inLastMonth(fortyDaysAgo);
=> false

is.not.inLastMonth(fortyDaysAgo);
=> true
'''

is.inLastYear(value:date)
---------------------------
####Checks if the given date is between now and a year ago.
interface: not

'''javascript
var twoMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 2));
var thirteenMonthsAgo = new Date(new Date().setMonth(new Date().getMonth() - 13));
...
```

#### <a name="apidoc.element.is_js.not.inNextMonth"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inNextMonth ()](#apidoc.element.is_js.not.inNextMonth)
- description and source-code
```javascript
inNextMonth = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inNextWeek(nineDaysLater);
=> false

is.not.inNextWeek(nineDaysLater);
=> true
'''

is.inNextMonth(value:date)
----------------------------
####Checks if the given date is between now and a month later.
interface: not

'''javascript
var tenDaysLater = new Date(new Date().setDate(new Date().getDate() + 10));
var fortyDaysLater = new Date(new Date().setDate(new Date().getDate() + 40));
...
```

#### <a name="apidoc.element.is_js.not.inNextWeek"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inNextWeek ()](#apidoc.element.is_js.not.inNextWeek)
- description and source-code
```javascript
inNextWeek = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inLastYear(thirteenMonthsAgo);
=> false

is.not.inLastYear(thirteenMonthsAgo);
=> true
'''

is.inNextWeek(value:date)
---------------------------
####Checks if the given date is between now and 7 days later.
interface: not

'''javascript
var twoDaysLater = new Date(new Date().setDate(new Date().getDate() + 2));
var nineDaysLater = new Date(new Date().setDate(new Date().getDate() + 9));
...
```

#### <a name="apidoc.element.is_js.not.inNextYear"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>inNextYear ()](#apidoc.element.is_js.not.inNextYear)
- description and source-code
```javascript
inNextYear = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inNextMonth(fortyDaysLater);
=> false

is.not.inNextMonth(fortyDaysLater);
=> true
'''

is.inNextYear(value:date)
---------------------------
####Checks if the given date is between now and a year later.
interface: not

'''javascript
var twoMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 2));
var thirteenMonthsLater = new Date(new Date().setMonth(new Date().getMonth() + 13));
...
```

#### <a name="apidoc.element.is_js.not.include"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>include ()](#apidoc.element.is_js.not.include)
- description and source-code
```javascript
include = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.all.ipv6(['2001:DB8:0:0:1::1', '1.2.3']);
=> false
'''

String checks
=============

is.include(value:string, target:string)
-----------------------------------------
####Checks if the given string contains a substring.
interface: not

'''javascript
is.include('Some text goes here', 'text');
=> true
...
```

#### <a name="apidoc.element.is_js.not.infinite"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>infinite ()](#apidoc.element.is_js.not.infinite)
- description and source-code
```javascript
infinite = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.finite([Infinity, -Infinity, 42.5]);
=> false
'''

is.infinite(value:number)
-------------------------
####Checks if the given value is infinite.
interfaces: not, all, any

'''javascript
is.infinite(Infinity);
=> true
...
```

#### <a name="apidoc.element.is_js.not.integer"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>integer ()](#apidoc.element.is_js.not.integer)
- description and source-code
```javascript
integer = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.decimal([40, 42.5, -43]);
=> false
'''

is.integer(value:number)
------------------------
####Checks if the given value is integer.
interfaces: not, all, any

'''javascript
is.integer(41);
=> true
...
```

#### <a name="apidoc.element.is_js.not.ios"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ios ()](#apidoc.element.is_js.not.ios)
- description and source-code
```javascript
ios = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.phantom('>=1');
=> true if current version of phantomjs is greater than or equal to 1

is.not.phantom('<2');
=> true if current version of phantomjs is not less than 2
'''

is.ios()
--------
####Checks if current device has ios.
interface: not

'''javascript
is.ios();
=> true if current device is iPhone, iPad or iPod
...
```

#### <a name="apidoc.element.is_js.not.ip"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ip ()](#apidoc.element.is_js.not.ip)
- description and source-code
```javascript
ip = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> false

// 'all' and 'any' interfaces can also take array parameter
is.all.hexColor(['fff', '333', 'f50']);
=> true
'''

is.ip(value:any)
-------------------------
####Checks if the given value matches ip regexp
interfaces: not, all, any

'''javascript
is.ip('198.156.23.5');
=> true
...
```

#### <a name="apidoc.element.is_js.not.ipad"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ipad ()](#apidoc.element.is_js.not.ipad)
- description and source-code
```javascript
ipad = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.iphone('>=7');
=> true if current version of iPhone is greater than or equal to 7

is.not.iphone('<8');
=> true if current version of iPhone is not less than 8
'''

is.ipad(range:number|string)
---------
####Checks if current device is iPad.
interface: not

'''javascript
is.ipad();
=> true if current device is iPad
...
```

#### <a name="apidoc.element.is_js.not.iphone"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>iphone ()](#apidoc.element.is_js.not.iphone)
- description and source-code
```javascript
iphone = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.ios();
=> true if current device is iPhone, iPad or iPod

is.not.ios();
=> true if current device is not iPhone, iPad or iPod
'''

is.iphone(range:number|string)
-----------
####Checks if current device is iPhone. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.iphone();
=> true if current device is iPhone
...
```

#### <a name="apidoc.element.is_js.not.ipod"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ipod ()](#apidoc.element.is_js.not.ipod)
- description and source-code
```javascript
ipod = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.ipad('>=7');
=> true if current version of iPad is greater than or equal to 7

is.not.ipad('<8');
=> true if current version of iPad is not less than 8
'''

is.ipod(range:number|string)
---------
####Checks if current device is iPod.
interface: not

'''javascript
is.ipod();
=> true if current device is iPod
...
```

#### <a name="apidoc.element.is_js.not.ipv4"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ipv4 ()](#apidoc.element.is_js.not.ipv4)
- description and source-code
```javascript
ipv4 = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ip(['123.123.23.12', 'A:B:C:D:E:F:0:0']);
=> true
'''

is.ipv4(value:any)
-------------------------
####Checks if the given value matches ipv4 regexp
interfaces: not, all, any

'''javascript
is.ipv4('198.12.3.142');
=> true
...
```

#### <a name="apidoc.element.is_js.not.ipv6"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ipv6 ()](#apidoc.element.is_js.not.ipv6)
- description and source-code
```javascript
ipv6 = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.ipv4(['198.12.3.142', '1.2.3']);
=> false

'''

is.ipv6(value:any)
-------------------------
####Checks if the given value matches ipv6 regexp
interfaces: not, all, any

'''javascript
is.ipv6('2001:DB8:0:0:1::1');
=> true
...
```

#### <a name="apidoc.element.is_js.not.json"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>json ()](#apidoc.element.is_js.not.json)
- description and source-code
```javascript
json = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.object([{}, new Object()]);
=> true
'''

is.json(value:any)
--------------------
####Checks if the given value type is pure json object.
interfaces: not, all, any

'''javascript
is.json({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.not.leapYear"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>leapYear ()](#apidoc.element.is_js.not.leapYear)
- description and source-code
```javascript
leapYear = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.year(year2016, 2015);
=> false

is.not.year(year2016, 2015);
=> true
'''

is.leapYear(value:number)
---------------------------------
####Checks if the given year number is a leap year
interfaces: not, all, any

'''javascript
is.leapYear(2016);
=> true
...
```

#### <a name="apidoc.element.is_js.not.linux"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>linux ()](#apidoc.element.is_js.not.linux)
- description and source-code
```javascript
linux = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.mac();
=> true if current OS is Mac OS X

is.not.mac();
=> true if current OS is not Mac OS X
'''

is.linux()
----------
####Checks if current OS is linux.
interface: not

'''javascript
is.linux();
=> true if current OS is linux
...
```

#### <a name="apidoc.element.is_js.not.lowerCase"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>lowerCase ()](#apidoc.element.is_js.not.lowerCase)
- description and source-code
```javascript
lowerCase = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...

// 'all' and 'any' interfaces can also take array parameter
is.all.upperCase(['YEAP', 'ALL UPPERCASE']);
=> true
'''


is.lowerCase(value:string)
--------------------------
####Checks if the given string is lowercase.
interfaces: not, all, any

'''javascript
is.lowerCase('yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.not.mac"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>mac ()](#apidoc.element.is_js.not.mac)
- description and source-code
```javascript
mac = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.windows();
=> true if current OS is Windows

is.not.windows();
=> true if current OS is not Windows
'''

is.mac()
--------
####Checks if current OS is Mac OS X.
interface: not

'''javascript
is.mac();
=> true if current OS is Mac OS X
...
```

#### <a name="apidoc.element.is_js.not.mobile"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>mobile ()](#apidoc.element.is_js.not.mobile)
- description and source-code
```javascript
mobile = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.desktop();
=> true if current device is desktop

is.not.desktop();
=> true if current device is not desktop
'''

is.mobile()
-----------
####Checks if current device is mobile.
interface: not
iPhone, iPod, Android Phone, Windows Phone, Blackberry.
'''javascript

is.mobile();
...
```

#### <a name="apidoc.element.is_js.not.month"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>month ()](#apidoc.element.is_js.not.month)
- description and source-code
```javascript
month = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.day(mondayObj, 'tuesday');
=> false

is.not.day(mondayObj, 'tuesday');
=> true
'''

is.month(value:date, month:string)
-----------------------------------
####Checks if the given date objects' month equal given monthString parameter.
interface: not

'''javascript
var januaryObj = new Date('01/26/2015');
var februaryObj = new Date('02/26/2015');
...
```

#### <a name="apidoc.element.is_js.not.nan"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>nan ()](#apidoc.element.is_js.not.nan)
- description and source-code
```javascript
nan = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.function([toString, 'foo', 'bar']);
=> false
'''

is.nan(value:any)
-----------------
####Checks if the given value type is NaN.
interfaces: not, all, any

'''javascript
is.nan(NaN);
=> true
...
```

#### <a name="apidoc.element.is_js.not.nanpPhone"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>nanpPhone ()](#apidoc.element.is_js.not.nanpPhone)
- description and source-code
```javascript
nanpPhone = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.ukPostCode(['B184BJ', '123']);
=> false
'''

is.nanpPhone(value:any)
-----------------------
####Checks if the given value matches North American numbering plan phone regexp.
interfaces: not, all, any

'''javascript
is.nanpPhone('609-555-0175');
=> true
...
```

#### <a name="apidoc.element.is_js.not.negative"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>negative ()](#apidoc.element.is_js.not.negative)
- description and source-code
```javascript
negative = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.positive([40, 42, -43]);
=> false
'''

is.negative(value:number)
-------------------------
####Checks if the given value is negative.
interfaces: not, all, any

'''javascript
is.negative(-41);
=> true
...
```

#### <a name="apidoc.element.is_js.not.null"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>null ()](#apidoc.element.is_js.not.null)
- description and source-code
```javascript
null = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.nan([NaN, 'foo', 1]);
=> false
'''

is.null(value:any)
------------------
####Checks if the given value type is null.
interfaces: not, all, any

'''javascript
is.null(null);
=> true
...
```

#### <a name="apidoc.element.is_js.not.number"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>number ()](#apidoc.element.is_js.not.number)
- description and source-code
```javascript
number = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.null([null, 'foo', 1]);
=> false
'''

is.number(value:any)
--------------------
####Checks if the given value type is number.
interfaces: not, all, any

'''javascript
is.number(42);
=> true
...
```

#### <a name="apidoc.element.is_js.not.object"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>object ()](#apidoc.element.is_js.not.object)
- description and source-code
```javascript
object = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.number([42, 'foo', 1]);
=> false
'''

is.object(value:any)
--------------------
####Checks if the given value type is object.
interfaces: not, all, any

'''javascript
is.object({foo: 'bar'});
=> true
...
```

#### <a name="apidoc.element.is_js.not.odd"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>odd ()](#apidoc.element.is_js.not.odd)
- description and source-code
```javascript
odd = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.even([40, 42, 43]);
=> false
'''

is.odd(value:number)
--------------------
####Checks if the given value is odd.
interfaces: not, all, any

'''javascript
is.odd(41);
=> true
...
```

#### <a name="apidoc.element.is_js.not.offline"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>offline ()](#apidoc.element.is_js.not.offline)
- description and source-code
```javascript
offline = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.online();
=> true if current device is online

is.not.online();
=> true if current device is not online
'''

is.offline()
------------
####Checks if current device is offline.
interface: not

'''javascript
is.offline();
=> true if current device is offline
...
```

#### <a name="apidoc.element.is_js.not.online"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>online ()](#apidoc.element.is_js.not.online)
- description and source-code
```javascript
online = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.tablet();
=> true if current device is tablet

is.not.tablet();
=> true if current device is not tablet
'''

is.online()
-----------
####Checks if current device is online.
interface: not

'''javascript
is.online();
=> true if current device is online
...
```

#### <a name="apidoc.element.is_js.not.opera"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>opera ()](#apidoc.element.is_js.not.opera)
- description and source-code
```javascript
opera = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.edge('>=12');
=> true if current version of edge is greater than or equal to 12

is.not.edge('<13');
=> true if current version of edge is not less than 13
'''

is.opera(range:number|string)
----------
####Checks if current browser is opera. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.opera();
=> true if current browser is opera
...
```

#### <a name="apidoc.element.is_js.not.palindrome"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>palindrome ()](#apidoc.element.is_js.not.palindrome)
- description and source-code
```javascript
palindrome = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.capitalized(['Nope', 'not']);
=> false
'''

is.palindrome(value:string)
---------------------------------------------
####Checks if the given string is palindrome.
interfaces: not, all, any

'''javascript
is.palindrome('testset');
=> true
...
```

#### <a name="apidoc.element.is_js.not.past"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>past ()](#apidoc.element.is_js.not.past)
- description and source-code
```javascript
past = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.tomorrow([today, tomorrow]);
=> false
'''

is.past(value:date)
---------------------
####Checks if the given date object indicate past.
interfaces: not, all, any

'''javascript
var yesterday = new Date(new Date().setDate(new Date().getDate() - 1));
var tomorrow = new Date(new Date().setDate(new Date().getDate() + 1));
...
```

#### <a name="apidoc.element.is_js.not.phantom"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>phantom ()](#apidoc.element.is_js.not.phantom)
- description and source-code
```javascript
phantom = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.safari('>=8');
=> true if current version of safari is greater than or equal to 8

is.not.safari('<7');
=> true if current version of safari is not less than 7
'''

is.phantom(range:number|string)
-----------
####Checks if current browser is phantomjs. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.phantom();
=> true if current browser is phantomjs
...
```

#### <a name="apidoc.element.is_js.not.positive"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>positive ()](#apidoc.element.is_js.not.positive)
- description and source-code
```javascript
positive = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.odd([40, 42, 43]);
=> false
'''

is.positive(value:number)
-------------------------
####Checks if the given value is positive.
interfaces: not, all, any

'''javascript
is.positive(41);
=> true
...
```

#### <a name="apidoc.element.is_js.not.propertyCount"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>propertyCount ()](#apidoc.element.is_js.not.propertyCount)
- description and source-code
```javascript
propertyCount = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.all.infinite([Infinity, -Infinity, 42.5]);
=> false
'''

Object checks
=============

is.propertyCount(value:object, count:number)
-------------------------------------
####Checks if objects' property count is equal to given count.
interface: not

'''javascript
is.propertyCount({this: 'is', 'sample': object}, 2);
=> true
...
```

#### <a name="apidoc.element.is_js.not.propertyDefined"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>propertyDefined ()](#apidoc.element.is_js.not.propertyDefined)
- description and source-code
```javascript
propertyDefined = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.propertyCount({this: 'is', 'sample': object}, 3);
=> false

is.not.propertyCount({}, 2);
=> true
'''

is.propertyDefined(value:object, property:string)
------------------------------------------
####Checks if the given property is defined on object.
interface: not

'''javascript
is.propertyDefined({yeap: 'yeap'}, 'yeap');
=> true
...
```

#### <a name="apidoc.element.is_js.not.quarterOfYear"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>quarterOfYear ()](#apidoc.element.is_js.not.quarterOfYear)
- description and source-code
```javascript
quarterOfYear = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inNextYear(thirteenMonthsLater);
=> false

is.not.inNextYear(thirteenMonthsLater);
=> true
'''

is.quarterOfYear(value:date, quarter:number)
---------------------------------------------
####Checks if the given date is in the parameter quarter.
interface: not

'''javascript
var firstQuarter = new Date('01/26/2015');
var secondQuarter = new Date('05/26/2015');
...
```

#### <a name="apidoc.element.is_js.not.regexp"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>regexp ()](#apidoc.element.is_js.not.regexp)
- description and source-code
```javascript
regexp = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.json([{}, {foo: 'bar'}]);
=> true
'''

is.regexp(value:any)
--------------------
####Checks if the given value type is RegExp.
interfaces: not, all, any

'''javascript
is.regexp(/test/);
=> true
...
```

#### <a name="apidoc.element.is_js.not.safari"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>safari ()](#apidoc.element.is_js.not.safari)
- description and source-code
```javascript
safari = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.opera('>=35');
=> true if current version of opera is greater than or equal to 35

is.not.opera('<20');
=> true if current version of opera is not less than 20
'''

is.safari(range:number|string)
-----------
####Checks if current browser is safari. Parameter is optional version range (or number) of browser.
interface: not

'''javascript
is.safari();
=> true if current browser is safari
...
```

#### <a name="apidoc.element.is_js.not.sameType"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>sameType ()](#apidoc.element.is_js.not.sameType)
- description and source-code
```javascript
sameType = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.undefined([{}, undefined]);
=> false
'''

is.sameType(value:any, other:any)
---------------------------------
####Checks if the given value types are same type.
interface: not

'''javascript
is.sameType(42, 7);
=> true
...
```

#### <a name="apidoc.element.is_js.not.socialSecurityNumber"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>socialSecurityNumber ()](#apidoc.element.is_js.not.socialSecurityNumber)
- description and source-code
```javascript
socialSecurityNumber = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.eppPhone(['+90.2322456789', '123']);
=> false
'''

is.socialSecurityNumber(value:any)
----------------------------------
####Checks if the given value matches social security number regexp.
interfaces: not, all, any

'''javascript
is.socialSecurityNumber('017-90-7890');
=> true
...
```

#### <a name="apidoc.element.is_js.not.sorted"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>sorted ()](#apidoc.element.is_js.not.sorted)
- description and source-code
```javascript
sorted = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.inArray(4, [1, 2, 3]);
=> false

is.not.inArray(4, [1, 2, 3]);
=> true
'''

is.sorted(value:array, sign:string)
----------------------
####Checks if the given array is sorted. Sign is optional parameter.
interfaces: not, all, any

'''javascript
is.sorted([1, 2, 3]);
=> true
...
```

#### <a name="apidoc.element.is_js.not.space"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>space ()](#apidoc.element.is_js.not.space)
- description and source-code
```javascript
space = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.falsy([false, true, undefined]);
=> false
'''

is.space(value:any)
----------------------
####Checks if the given value is space.
interfaces: not, all, any

'''javascript
is.space(' ');
=> true
...
```

#### <a name="apidoc.element.is_js.not.startWith"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>startWith ()](#apidoc.element.is_js.not.startWith)
- description and source-code
```javascript
startWith = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.lowerCase(['yeap', 'all lowercase']);
=> true
'''

is.startWith(value:string, target:string)
-------------------------------------------
####Checks if the given string starts with substring.
interface: not

'''javascript
is.startWith('yeap', 'ye');
=> true
...
```

#### <a name="apidoc.element.is_js.not.string"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>string ()](#apidoc.element.is_js.not.string)
- description and source-code
```javascript
string = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.regexp([{}, /test/]);
=> false
'''

is.string(value:any)
--------------------
####Checks if the given value type is string.
interfaces: not, all, any

'''javascript
is.string('foo');
=> true
...
```

#### <a name="apidoc.element.is_js.not.tablet"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>tablet ()](#apidoc.element.is_js.not.tablet)
- description and source-code
```javascript
tablet = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.mobile();
=> true if current device is mobile

is.not.mobile();
=> true if current device is not mobile
'''

is.tablet()
-----------
####Checks if current device is tablet.
interface: not
iPad, Android Tablet, Windows Tablet
'''javascript

is.tablet();
...
```

#### <a name="apidoc.element.is_js.not.timeString"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>timeString ()](#apidoc.element.is_js.not.timeString)
- description and source-code
```javascript
timeString = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.alphaNumeric(['alphaNu3er1k', '*?']);
=> false
'''

is.timeString(value:any)
------------------------
####Checks if the given value matches time string regexp.
interfaces: not, all, any

'''javascript
is.timeString('13:45:30');
=> true
...
```

#### <a name="apidoc.element.is_js.not.today"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>today ()](#apidoc.element.is_js.not.today)
- description and source-code
```javascript
today = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.not.touchDevice();
=> true if current device does not support touch
'''

Time checks
===========

is.today(value:date)
----------------------
####Checks if the given date object indicate today.
interfaces: not, all, any

'''javascript
var today = new Date();
is.today(today);
...
```

#### <a name="apidoc.element.is_js.not.tomorrow"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>tomorrow ()](#apidoc.element.is_js.not.tomorrow)
- description and source-code
```javascript
tomorrow = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.yesterday([today, yesterday]);
=> false
'''

is.tomorrow(value:date)
-------------------------
####Checks if the given date object indicate tomorrow.
interfaces: not, all, any

'''javascript
var today = new Date();
is.tomorrow(today);
...
```

#### <a name="apidoc.element.is_js.not.touchDevice"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>touchDevice ()](#apidoc.element.is_js.not.touchDevice)
- description and source-code
```javascript
touchDevice = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.offline();
=> true if current device is offline

is.not.offline();
=> true if current device is not offline
'''

is.touchDevice()
------------
####Checks if current device supports touch.
interface: not

'''javascript
is.touchDevice();
=> true if current device supports touch
...
```

#### <a name="apidoc.element.is_js.not.truthy"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>truthy ()](#apidoc.element.is_js.not.truthy)
- description and source-code
```javascript
truthy = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.existy([{}, 'foo']);
=> true
'''

is.truthy(value:any)
--------------------
####Checks if the given value is truthy. (existy and not false)
interfaces: not, all, any

'''javascript
is.truthy(true);
=> true
...
```

#### <a name="apidoc.element.is_js.not.ukPostCode"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>ukPostCode ()](#apidoc.element.is_js.not.ukPostCode)
- description and source-code
```javascript
ukPostCode = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.caPostalCode(['L8V3Y1', '123']);
=> false
'''

is.ukPostCode(value:any)
------------------------
####Checks if the given value matches UK post code regexp.
interfaces: not, all, any

'''javascript
is.ukPostCode('B184BJ');
=> true
...
```

#### <a name="apidoc.element.is_js.not.undefined"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>undefined ()](#apidoc.element.is_js.not.undefined)
- description and source-code
```javascript
undefined = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.char(['f', 'o', 'o']);
=> true
'''

is.undefined(value:any)
-----------------------
####Checks if the given value type is undefined.
interfaces: not, all, any

'''javascript
is.undefined(undefined);
=> true
...
```

#### <a name="apidoc.element.is_js.not.under"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>under ()](#apidoc.element.is_js.not.under)
- description and source-code
```javascript
under = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.above(41, 30);
=> true

is.not.above(42, 50);
=> true
'''

is.under(value:number, max:number)
---------------------------
####Checks if the given value is under maximum value.
interface: not

'''javascript
is.under(30, 35);
=> true
...
```

#### <a name="apidoc.element.is_js.not.upperCase"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>upperCase ()](#apidoc.element.is_js.not.upperCase)
- description and source-code
```javascript
upperCase = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.include('test', 'text');
=> false

is.not.include('test', 'text');
=> true
'''

is.upperCase(value:string)
--------------------------
####Checks if the given string is UPPERCASE.
interfaces: not, all, any

'''javascript
is.upperCase('YEAP');
=> true
...
```

#### <a name="apidoc.element.is_js.not.url"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>url ()](#apidoc.element.is_js.not.url)
- description and source-code
```javascript
url = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.all.space([' ', 'foo', undefined]);
=> false
'''

RegExp checks
=============

is.url(value:any)
-----------------
####Checks if the given value matches url regexp.
interfaces: not, all, any

'''javascript
is.url('http://www.test.com');
=> true
...
```

#### <a name="apidoc.element.is_js.not.usZipCode"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>usZipCode ()](#apidoc.element.is_js.not.usZipCode)
- description and source-code
```javascript
usZipCode = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.dateString(['11/11/2011', '90/11/2011']);
=> false
'''

is.usZipCode(value:any)
-----------------------
####Checks if the given value matches US zip code regexp.
interfaces: not, all, any

'''javascript
is.usZipCode('02201-1020');
=> true
...
```

#### <a name="apidoc.element.is_js.not.weekday"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>weekday ()](#apidoc.element.is_js.not.weekday)
- description and source-code
```javascript
weekday = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.weekend([sunday, saturday, monday]);
=> false
'''

is.weekday(value:date)
------------------------
####Checks if the given date objects' day is weekday.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.not.weekend"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>weekend ()](#apidoc.element.is_js.not.weekend)
- description and source-code
```javascript
weekend = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.leapYear([2016, 2080]);
=> true
'''

is.weekend(value:date)
------------------------
####Checks if the given date objects' day is weekend.
interfaces: not, all, any

'''javascript
var monday = new Date('01/26/2015');
var sunday = new Date('01/25/2015');
...
```

#### <a name="apidoc.element.is_js.not.windowObject"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>windowObject ()](#apidoc.element.is_js.not.windowObject)
- description and source-code
```javascript
windowObject = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.sameType(42, '7');
=> false

is.not.sameType(42, 7);
=> false
'''

is.windowObject(value:any)
-----------------------------
####Checks if the given object is window object.
interfaces: not, all, any

'''javascript
is.windowObject(window);
=> true
...
```

#### <a name="apidoc.element.is_js.not.windows"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>windows ()](#apidoc.element.is_js.not.windows)
- description and source-code
```javascript
windows = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.windowsTablet();
=> true if current device is Windows tablet

is.not.windowsTablet();
=> true if current device is not Windows tablet
'''

is.windows()
------------
####Checks if current OS is Windows.
interface: not

'''javascript
is.windows();
=> true if current OS is Windows
...
```

#### <a name="apidoc.element.is_js.not.windowsPhone"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>windowsPhone ()](#apidoc.element.is_js.not.windowsPhone)
- description and source-code
```javascript
windowsPhone = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.blackberry();
=> true if current device is Blackberry

is.not.blackberry();
=> true if current device is not Blackberry
'''

is.windowsPhone()
-----------------
####Checks if current device is Windows phone.
interface: not

'''javascript
is.windowsPhone();
=> true if current device is Windows phone
...
```

#### <a name="apidoc.element.is_js.not.windowsTablet"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>windowsTablet ()](#apidoc.element.is_js.not.windowsTablet)
- description and source-code
```javascript
windowsTablet = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.windowsPhone();
=> true if current device is Windows phone

is.not.windowsPhone();
=> true if current device is not Windows Phone
'''

is.windowsTablet()
------------------
####Checks if current device is Windows tablet.
interface: not

'''javascript
is.windowsTablet();
=> true if current device is Windows tablet
...
```

#### <a name="apidoc.element.is_js.not.within"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>within ()](#apidoc.element.is_js.not.within)
- description and source-code
```javascript
within = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.under(30, 35);
=> true

is.not.under(42, 30);
=> true
'''

is.within(value:number, min:number, max:number)
---------------------------------
####Checks if the given value is within minimum and maximum values.
interface: not

'''javascript
is.within(30, 20, 40);
=> true
...
```

#### <a name="apidoc.element.is_js.not.year"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>year ()](#apidoc.element.is_js.not.year)
- description and source-code
```javascript
year = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
is.month(februaryObj, 'january');
=> false

is.not.month(februaryObj, 'january');
=> true
'''

is.year(value:date, year:number)
---------------------------------
####Checks if the given date objects' year equal given yearNumber parameter.
interface: not

'''javascript
var year2015 = new Date('01/26/2015');
var year2016 = new Date('01/26/2016');
...
```

#### <a name="apidoc.element.is_js.not.yesterday"></a>[function <span class="apidocSignatureSpan">is_js.not.</span>yesterday ()](#apidoc.element.is_js.not.yesterday)
- description and source-code
```javascript
yesterday = function () {
    return !func.apply(null, slice.call(arguments));
}
```
- example usage
```shell
...
=> true

// 'all' and 'any' interfaces can also take array parameter
is.all.today([today, yesterday]);
=> false
'''

is.yesterday(value:date)
--------------------------
####Checks if the given date object indicate yesterday.
interfaces: not, all, any

'''javascript
var today = new Date();
is.yesterday(today);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
