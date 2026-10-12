# True Blue Blazing Melbourne — Event Lead Form

A single-file, mobile-first competition landing page designed for GitHub Pages and Salesforce Web-to-Lead.

## Before publishing

Open `index.html` and make these changes:

1. Replace `YOUR_SALESFORCE_ORG_ID` with the Salesforce Web-to-Lead Org ID (`oid`).
2. Replace `00NXXXXXXXXXXXX` with the Salesforce field ID for your event/campaign marker, or remove that hidden field.
3. Confirm the Web-to-Lead endpoint for the Salesforce org.
4. Add the official True Blue Blazing Melbourne logo/brand assets.
5. Add the final competition terms and privacy notice/link.
6. Test with a non-production/test lead before using the QR code at the event.

## Name handling

The attendee sees one `Name` field. Before submission, JavaScript splits it into Salesforce `first_name` and `last_name`.
For a single-word name, that value is submitted as `last_name` because Salesforce Lead requires Last Name.

## GitHub Pages

Upload `index.html` to a repository, then enable GitHub Pages for the repository. Once the public Pages URL is live, use that URL for the event QR code.

## Demo flow

Attendee entry → Salesforce Lead → Plinqx Agent Console skill selects winner → Xero contact/invoice workflow

Suggested Xero demo invoice:
- Contact: winner's name
- Reference: True Blue Blazing Melbourne Winner
- Description: Woolies Voucher
- Quantity: 1
- Unit amount: $150.00

## Important

The included event mark is only a temporary text/graphic lockup, not an official True Blue Blazing logo. Replace it with the approved event logo before production use.
