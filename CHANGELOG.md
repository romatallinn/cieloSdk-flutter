## 0.0.6

- Skip mod10 validation for test cards in sandbox mode.
- Add tests for card number validation of test cards in sandbox mode. 

## 0.0.5

- Fix validation for pre-defined test card numbers in sandbox mode.
  Learn more: https://braspag.github.io/en/manual/braspag-pagador#test-cards-(simulado)

## 0.0.4

- Allow localized character sets for cardholder names

## 0.0.3

Quickfix for incorrect API URL for Braspag's Silent Order Post in production.

## 0.0.2

The release mostly meant to improve Pub scoring of the package.

- Longer project description
- Example project
- More dartdoc for public API
- Dart formatting

*Breaking change:* 
- Fix method signature: `Cielo.sop.sendCard(CieloCard card, {required String accessToken})`.

## 0.0.1

The first public release of the package.
It integrates the most basic features of Cielo.

#### Features
- SDK's core initialization with options (supports Cielo and Braspag, and sandbox and production environments)
- Client-side validation of card data (mod10, brand-based, etc.)
- Silent Order Post (SOP) integration: `Cielo.initSOP()` and `Cielo.sop.sendCard(card, accessToken=accessToken)`
- Profound testing of basic features

