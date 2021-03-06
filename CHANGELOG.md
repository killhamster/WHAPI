# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.6.2] 2020-04-15

### Changed

  - Added "stub" and "low quality" flags to article_details()

## [0.6.1] 2020-04-10

### Changed

  - integrated get_html() into parse_intro() and parse_steps() for ease of use

## [0.6.0] 2020-04-10

### Changed

- Refactored functions to take advantage of WikiHow's underlying MediaWiki API and increase efficiency
- No features rely on scraping any longer. JSON is now retrieved and parsed to provide relevant data
- Removed classes that aren't really needed with the way data is returned now

## [0.5.4] 2020-03-26

- Forking from original project to add features I want but that may not be useful to anyone else. Thanks to [OpenJarbas](https://github.com/OpenJarbas) for starting this.

## [0.5.3]  - 2020-03-23

### Added

- HowTo().intro
    - Thanks to [killhamster](https://github.com/killhamster) for this feature

### Changed

- text is now stripped of extra blank spaces

### Fixed

- Some step summaries include extra divs (pictures for example) which
poluted the text, these are now removed

## [0.5.2]  - 2020-03-22

### Fixed

At some point WikiHow has changed the class name they used for article titles. As a result, scraping and parsing failed.

Thanks to [killhamster](https://github.com/killhamster) for submitting a fix

## [0.5.0]  - 2019-12-12

Breaking Changes, api is backward incompatible

### Changed

- Refactor into individual classes
    - WikiHow
    - HowTo
    - HowToStep
- Refactor search
    - WikiHow.search is now a generator
    - search now returns HowTo objects instead of urls
- split examples in several files

### Added

- search_wikihow function
- ParseError exception

### Fixed

- handle parse errors

## [0.3.1]  - 2019-12-12

### Changed

- Transfered ownership to [OpenJarbas](https://github.com/OpenJarbas)
- Made a changelog

[unreleased]: https://github.com/OpenJarbas/PyWikiHow/tree/dev
[0.5.3]: https://github.com/OpenJarbas/PyWikiHow/tree/0.5.3
[0.5.2]: https://github.com/OpenJarbas/PyWikiHow/tree/0.5.2
[0.5.0]: https://github.com/OpenJarbas/PyWikiHow/tree/0.5.0
[0.3.1]: https://github.com/OpenJarbas/PyWikiHow/tree/0.3.1
