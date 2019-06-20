# GDPR Data request template
---

This document is licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

---

> **DISCLAIMER:** WE ARE NOT LAWYERS. THIS IS PROVIDED AS IS, WITHOUT ANY WARRANTY OF ANY KIND. IN DOUBT, REACH OUT TO YOUR NATIONAL DATA PROTECTION SUPERVISORY AUTHORITY OR CONSULT A LAWYER.

**IMPORTANT: This is living document. It is recommended to check if this template changed regularly.**

## Purpose

We are not aware of any GDPR data request template for Matrix users which we believe is a problem. Based on the research document, leaks can happen in various and complex ways, usually tied to identifiers that are hard to find or are rapidly changing - device IP address, HTTP headers, etc. Users might not know how to gather such personal identifiers accurately.

This effort will attempt to document:
1. A GDPR data request template, based on [datarequests.org template](https://www.datarequests.org/blog/sample-letter-gdpr-access-request/) licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
2. How a user can identify which services they are using.
3. How a user can collect as many personal identifiers as possible to include them in the request.
4. Any other steps specific to Matrix concerning GDPR data requests.

**NOTE:** It is important for The Data controller/processor to be able to identify the requester, but equally able to protect against providing data that actually belong to other users. Because it is usually not possible to provide *all* the used personal identifier, The Data controller/processor would not be able to identify you for all the data. Take contact with your Data controller/processor to know how you can be identified more accurately. **You have the right to be informed about and access data which has been identified and tied to you even if the data does not directly contain a private identifier.**

## How to use
- Edit the information to identify you at the bottom.
- Sign the request with your full name.

For Push server Identifiers, you can get your App ID and Push key at `/_matrix/client/r0/pushers`. 

Example `curl` request:
```
curl -sH 'Authorization: Bearer <YOUR API TOKEN HERE>' https://<YOUR CLIENT API HOSTNAME HERE>/_matrix/client/r0/pushers
```
Set `<YOUR API TOKEN>` and `<YOUR CLIENT API HOSTNAME HERE>` to their appropriate values.

## Template
---

To Whom It May Concern:

I am hereby requesting access according to Article 15 GDPR. Please confirm whether or not you are processing personal data (as defined by Article 4(1) and (2) GDPR) concerning me.

In case you are, I am hereby requesting access to the following information pursuant to Article 13, 14 and 15 GDPR:

1. *all* personal data concerning me that you have stored, which is processed by at least all services referenced in this document: https://gist.github.com/maxidorius/5736fd09c9194b7a6dc03b6b8d7220d0;
2. The lawful basis under which you are processing the data;
3. If required for the processing, the data that proves my explicit informed consent to the service as well as the IP address, date, time, and mean of collection of my explicit informed consent of the processing;
4. the purposes of the processing;
5. the categories of personal data concerned;
6. the recipients to whom the personal data have been or will be disclosed;
7. where possible, the envisaged period for which the personal data will be stored, or, if not possible, the criteria used to determine that period;
8. where the personal data are not collected from the data subject, any available information as to their source;
9. the existence of automated decision-making, including profiling, referred to in Article 22(1) and (4) GDPR and, at least in those cases,  meaningful information about the logic involved, as well as the significance and the envisaged consequences of such processing for me.

If you are transferring my personal data to a third country or an international organisation, I request to be informed about the appropriate safeguards according to Article 46 GDPR concerning the transfer.

[Please make the personal data concerning me, which I have provided to you, available to me in a structured, commonly used and machine-readable format as laid down in Article 20(1) GDPR.]

My request explicitly includes any other services and companies for which you are the controller as defined by Article 4(7) GDPR.

As laid down in Article 12(3) GDPR, you have to provide the requested information to me without undue delay and in any event within one month of receipt of the request. According to Article 15(3) GDPR, you have to answer this request without cost to me.

I am including the following information necessary to identify me:
- This Matrix ID
- My E-mail addresses:
  - `<VALUE IN SETTINGS OR POTENTIALLY SHARED WITH THE SERVICES BY OTHER USERS. YOU MAY DELETE THIS LINE IF NOT NEEDED>`
  - `<VALUE IN SETTINGS OR POTENTIALLY SHARED WITH THE SERVICES BY OTHER USERS. YOU MAY DELETE THIS LINE IF NOT NEEDED>`
- My Phone numbers:
  - `<VALUE IN SETTINGS OR POTENTIALLY SHARED WITH THE SERVICES BY OTHER USERS. YOU MAY DELETE THIS LINE IF NOT NEEDED>`
  - `<VALUE IN SETTINGS OR POTENTIALLY SHARED WITH THE SERVICES BY OTHER USERS. YOU MAY DELETE THIS LINE IF NOT NEEDED>`
- My Push Identifier:
  - My App ID: - `<SEE USAGE ABOVE>`
  - My Push Key: `<SEE USAGE ABOVE>`

If you do not answer my request within the stated  period, I am reserving the right to take legal action against you and to  lodge a complaint with the responsible supervisory authority.

Yours sincerely,  
**<PUR YOUR NAME HERE>**