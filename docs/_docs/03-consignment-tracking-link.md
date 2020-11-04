---
title: "Consignment Tracking - Direct URL Link"
permalink: /docs/tracking-direct-link/
excerpt: "Providing a simple link to your customer allowing an APC Consignment to be tracked."
last_modified_at: 2020-11-04
redirect_from:
  - /theme-setup/
toc: true
---
This functionality has been provisioned to facilitate our retail partners so that they are able to send the tracking link to consignees at the time of order dispatch. The URL link comprises the 22 digit APC consignment number as well as the consignee’s postcode. It allows consignees to access tracking information without having to enter details on APC’s main tracking page or the need to pass the CAPTCHA test.

**URL Format**
https://apc-overnight.com/track-parcel.php?id=[22 DIGIT IDENTIFIER]&postcode=[POSTCODE]

**Example**
https://apc-overnight.com/track-parcel.php?id=2018073110099660003021&postcode=WS11+8LD

The outward and inward codes in the postcode argument should always be separated by a single ‘+’, e.g. ‘S9+5JF’. The postcode is not case sensitive.

**Successful Response**

**Troubleshooting**
1. If the format of the postcode or identifier is invalid, the user is redirected to https://apc-overnight.com/receiving-a-parcel/track-your-parcel/exception and the following error message is displayed.
2. If the format of the postcode and identifier is valid but the identifier does not exist, the user is redirected to https://apc-overnight.com/receiving-a-parcel/track-your-parcel/exception and the following error message is displayed.
3. If the postcode and identifier format is valid but the identifier is for a consignment that was booked on the current date and has not yet had any scans, the user is redirected to https://apc-overnight.com/receiving-a-parcel/track-your-parcel/exception and the following error message is displayed.
