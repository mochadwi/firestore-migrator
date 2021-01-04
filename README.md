You can check for [author README.md for detailed usage](https://github.com/codediodeio/firestore-migrator)

This repo contains a data migration from CSV/JSON is supported by default (HTML still not supported).

If you're using HTML (crawling data/didn't have API or BE access), you can convert from `<table>` to CSV/JSON

1. [HTML Table to JSON](https://www.convertjson.com/html-table-to-json.htm)
1. [HTML Table to CSV](https://www.convertcsv.com/html-table-to-csv.htm)

What's Changes:

1. Ability to detect `true` or `false`, the original repo using `1` (true) or `0` (false), see [BooleanFH](https://github.com/codediodeio/firestore-migrator/blob/master/src/shared.ts#L82)
1. Ability to parse `timestamp` string to `epoch`, see [TimeStampFH](https://github.com/mochadwi/firestore-migrator/blob/master/src/shared.ts#L92)