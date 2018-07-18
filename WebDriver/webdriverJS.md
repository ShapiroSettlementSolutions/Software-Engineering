# Timeout

## 1. Value in the method overwrites other definition
## 2. System default value in the config file (index.js)


# Verify elements exist

## link exists
      return driver.wait(until.elementsLocated(by.partialLinkText(keywords)));
      
      return driver.wait(until.elementsLocated(by.className("base-data-table__col search-result__no-matches-found")));

## elements exist
        return driver.wait(until.elementsLocated(by.css('div.g'))).then(function() {
            return driver.findElements(by.css('div.g'));
        })
        .then(function (elements) {
            expect(elements.length).to.not.equal(0);
        });
