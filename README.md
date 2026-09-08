# OffPay UPI

OffPay UPI is a lightweight static web app that helps users scan a UPI QR code, verify the recipient details, and continue the payment through a supported USSD or bank flow when mobile data is unavailable.

## Features

- Scan a UPI QR code directly from the browser
- Validate the scanned or manually entered UPI ID
- Preview merchant and amount details before continuing
- Automatically copy the UPI ID to the clipboard for quick use
- Continue the payment using a supported bank/USSD flow
- Works without requiring a mobile data connection for the QR/payment preparation step

## How it works

1. Open the site in a browser.
2. Scan the merchant QR or manually enter the UPI ID.
3. Review the detected recipient and payment details.
4. Continue to the supported payment flow in the bank or USSD channel.
5. Enter the amount and UPI PIN only in the bank-approved payment flow.

## Important note

OffPay does not collect or store your UPI PIN. The payment is still handled by your bank or supported payment flow. Cellular signal and bank/operator support are required for the actual payment step.

## Run locally

Because this is a simple static site, you can open the file directly in a browser or host it with any static server.

Example using Python:

```bash
cd /workspaces/OffPay-UPI
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Files

- `index.html` — Application markup, styling, and JavaScript
- `README.md` — Project overview and usage notes

## Disclaimer

This project is for demonstration and informational use. Payment availability depends on your bank, operator, and local network configuration.
