# Vipps Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).

## 1.0.6 - 2020-11-19

### Fixed
- Fixed missing method error when capturing a transaction

## 1.0.5 - 2020-11-15

### Fixed
- Fixed PSR-4/Composer 2 compatibility
- Fixed some faulty namespace references

## 1.0.4 - 2020-09-10

### Added
- Added `errorFallbackUrl` so you can differentiate between payment errors/cancellation and successful payments
- Added [plugin info](https://www.vipps.no/developers-documentation/ecom/documentation/#optional-vipps-http-headers) to default request headers

### Changed
- Started initial translation work
- Removed `tightenco/collect` dependency
- Changed `craftcms/commerce` dependency to `^3.0`

### Fixed
- Added parsing of environment variable for access token request

## 1.0.3 - 2020-03-27

### Changed
- If there is a discrepancy between paid amount in Vipps and Commerce, it will now use the order total if the discrepancy is less than 0.10

### Fixed
- Fixed marking order as completed on Express callback
- Fixed class param for express checkout links 
- Fixed payment amount for successful express transactions
- Fixed missing address lines on Express payment that made status update fail silently
- Fixed JS event issue when there is multiple buttons
- Fixed error check on gateway response
- Fixed error when calling API through console commands

### Added
- Added Twig params to express button 
- Added better error handling in shipping callback

## 1.0.2 - 2019-06-10
### Fixed
- Fixed error with wrong status type in Commerce 2.1 when redirecting to Vipps

## 1.0.1 - 2019-02-26
### Fixed
- Fixed payment request when no phone number is set
- Fixed error message for payment request


## 1.0.0 - 2019-02-26
### Added
- Initial release
