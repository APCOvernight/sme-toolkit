---
title: "About PinPoint API (PPAPI)"
permalink: /docs/about-ppapi/
excerpt: "Getting started with PinPoint API."
last_modified_at: 2020-06-30
redirect_from:
  - /theme-setup/
toc: true
---
PinPoint was originally introduced as a web page, allowing customers recieving consignments through APC Overnight to track them based on consignment and postcode.

## Walk-through using SWAGGER interface
The PinPoint API is documented using SWAGGER - a standard way of describing what an API is capable, and the expected results and structures.

__To complete this walk-through you will need :__ 

* A set of APC API Credentials with access to the PPAPI Scope
* A manifested consignment to track - 
  * either a 22 Digit long consignment number
  * or a 7 digit consignment number and delivery postcode. 

Method 

- Open a browser to [https://pinpoint.apc-overnight.com](https://pinpoint.apc-overnight.com)
- Click on the Authorize button
- Enter your client ID / Secret ID
- Click Authorize button


If you are testing using a 7 Digit short consignment number and Postcode
- Click GET on the getConsignment method (Retrieve PinPoint DepotInformation based on a Postcode and Consignment Number)
- Click on the Try it Out button
- Enter Consignment and Postcode
- Click Execute
- Server response will be shown in the page.

If you are testing using a 22 Digit long consignment number
- Click GET on the getConsignment method (Retrieve PinPoint Data based on a 22 Digit Identifier.)
- Click on the Try it Out button
- Enter 22 Digit Long consignment number
- Server response will be shown in the page.


## Walk-through using INSOMNIA REST tool
Insomnia is a desktop tool for testing REST and other API's.  To make testing PinPoint easy, we have provided an Insomnia Workspace file.

- [Download Insomnia](https://insomnia.rest/download/core/?) and install using your desktop operating system installation procedure.  Insomnia is available for Windows, Macintosh and Linux.
- This button should download and install the workspace.

[![Run in Insomnia}](https://insomnia.rest/images/run.svg)](https://insomnia.rest/run/?label=PinPointAPI&uri=https%3A%2F%2Fgithub.com%2FAPCOvernight%2Fsme-toolkit%2Fblob%2Fmaster%2Fservices%2FPinPointAPI%2FInsomnia%2FPinPointAPI.json)

Clicking on the appropriate GetPinpoint will allow the method to be called.

- Fill in your client ID / Secret ID using the OAuth2 tab
- The __Docs__ tab details which call is required
- Each call will prompt for consignment details.