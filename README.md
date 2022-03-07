# web-vgs-collect
Web based Solid-VGS Collect integration sample code

## Table of contents

- [Overview](#overview)
- [Run the app](#run-the-app)
- [Parameters](#Parameters)
- [Internals](#internals)

## Overview
The purpose of this app is to show how to use the VGS Collect JavaScript SDK.For complete information about the API, head to the [docs](https://www.verygoodsecurity.com/docs/vgs-collect/overview).

## Run the app
To Run the app run `npx serve`. then open `http://localhost:5000` in browser.


## Parameters
### Parameters for set pin
| Parameters    | Description   |
| ------------- | ------------- |
| VGS-Vault-Id  | vgs vault id |
| card-Id       | solid card id |
| pin-token     | Pin token you can get it from api |
| VGS-env       | mode - live or sandbox |

### Parameters for debit pull link card
| Parameters    | Description   |
| ------------- | ------------- |
| VGS-Vault-Id  | vgs vault id |
| contact-Id    | solid contact id |
| token         | Token you can get it from api |
| VGS-env       | mode - live or sandbox |

## Internals

- The `submit` function collects all information from input fields.and it will start submit the details.
- In a real-life integration, the `pin-token`  would have to be requested from `pintoken` api.
