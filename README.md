# alfred-npms

> Alfred 3 workflow for [npms.io](https://npms.io)

![screenshot](https://cldup.com/MIxtMSbnsL.png)

## Commands

- `npm <query>`: Search npms.io with `query`; open package on `npmjs.com`.
  Example: `npm socket` will return a list of packages matching name "socket", keyword "socket", etc.

  Modifiers:
  - `⌘`: Open package repository.
  - `⌥`: Open package homepage (this often roughly the same as the repository URL).

- `npms cleardb`: Clears internal cache.  By default, search results are cached for one (1) day.

## Environment Variables

These are set within the workflow configuration and can be altered to better suit your usage.

- `NPMS_CACHE_EXPIRATION`: Number of seconds to keep search results.  Defaults to `86400` (one day).
- `NPMS_SEARCH_SCORE_THRESHOLD`: Packages having a "search score" lower than this number will be ignored.  Defaults to `0.01`.

## License

Copyright 2016 [Christopher Hiller](https://boneskull.com).  Licensed MIT.
