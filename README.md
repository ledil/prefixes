Country Prefix Codes For Go
===========================

[![Build Status](https://travis-ci.org/relops/prefixes.png?branch=master)](https://travis-ci.org/relops/prefixes)

Installation
------------

    go get github.com/relops/prefixes


Features
--------

* Looks up country dialing code prefixes using a given number
* Can tell the difference between the US and Canada
* Handles the Vatican City

Example
-------

```go
package main

import (
	"github.com/relops/prefixes"
	"fmt"
)

func main() {
	country, err := prefixes.Lookup("46485562003")
	fmt.Printf("Country: %s\n", country.Name) // Prints Sweden
}
```

Broken Examples
---------------

We're keen to hear of any examples that don't work - in this case, please raise an issue.

Credits
-------

For providing the input data, kudos goes to:

* https://github.com/mledoze/countries
* http://en.wikipedia.org/wiki/List_of_North_American_Numbering_Plan_area_codes

Please check out the terms under which you can use their data.
