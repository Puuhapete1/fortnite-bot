# Changelog for Fortnite Bot

## [Unreleased]
- /compare command to compare users delimited by commas
- /rating command to quickly see user's TRN rating

## [3.6.4] - 2018-05-22
### Added
- Link to Fortnite Tracker for the bot's response to /user command
- Added changelog to repository

## Changed
- Changed error logging to use console.error() instead of console.log()

## [3.6.3] - 2018-05-21
### Added
- Temporary cache
- /help command to also get command info (same functionality as /start and /info)

### Changed
- Account for extra whitespace in command input by matching for whitespace instead of splitting by spaces

## [3.6.2] - 2018-05-16
### Added
- Test cases for the various commands

### Fixed
- Fixed /recent error message when Markdown can't parse the username correctly

## [3.6.1] - 2018-05-15
### Fixed
- Fixed /season command getting the correct season number

## [3.6.0] - 2018-05-14
### Added
- Optional platform flags (pc, xbox, ps4) to add at the end of commands to specify the platform to search in

## [3.5.0] - 2018-05-08
### Added
- Demo of /set to README
- TRN rating data to modes commands

### Changed
- Used season 3 data from Fortnite Tracker instead of cache to make command not deprecated anymore

## [3.4.1] - 2018-05-07
### Changed
- Switched package manager from npm to yarn

### Fixed
- Fixed sending the start/info message for /start and /info commands

## [3.4.0] - 2018-05-04
### Added
- /set command to link messaging platform user ID with Fortnite username
- /rold command to show recent matches the old way without Markdown

### Changed
- Modified how table looks for /recent

## [3.3.0] - 2018-05-04
### Changed
- Changed bot's response to /recent to show matches in a Markdown style table

## [3.2.0] - 2018-05-04
### Changed
- Moved methods into different files for better readability
- Replaced instances of var with let and const to fix style

## [3.1.2] - 2018-05-01
### Fixed
- Fixed parsing command input when username has multiple words

## [3.1.1] - 2018-05-01
### Fixed
- Fixed getting text for message object in Telegram message handler

## [3.1.0] - 2018-05-01
### Added
- Telegram bot capability to respond to forwarded messages

## [3.0.1] - 2018-05-01
### Fixed
- Fixed the bot's response for /season to display the correct season

## [3.0.0] - 2018-05-01
### Added
- /season4 and /s4 commands to get season 4 data

### Deprecated
- /season3 command because of Fortnite Tracker giving season 4 data, uses cache to get season 3 data for the limited users in it

## [2.2.1] - 2018-04-25
### Fixed
- Maps the username's hashcode to Fortnite data in cache to account for characters that the cache can't parse

## [2.2.0] - 2018-04-25
### Added
- Caching of season 3 data that the bot gets from the commands to prepare for season 4

### Fixed
- Fixed the config setup in the README

## [2.1.3] - 2018-04-24
### Fixed
- Fixed kills/game stat when player has 0 games

## [2.1.2] - 2018-04-22
### Fixed
- Fixed the formatSeconds method to make it not exported to other files

## [2.1.1] - 2018-04-22
### Fixed
- Fixed times in top 6, 12, and 25 for /season3 command

## [2.1.0] - 2018-04-21
### Added
- /season3 command to combine data from season 3 modes

## [2.0.0] - 2018-04-19
### Changed
- Use configuration tokens from .env instead of config.json
- Merged heroku branch into master branch to remove the need for two branches

## [1.0.0] - 2018-02-04 - 2018-04-17 (Didn't update version number for changes)