# API Examples

## Place a Bet

```http
POST /api/bet HTTP/1.1
Host: xenpay.io
Content-Type: application/json
402-Payment-Required: true

{
  "userAddress": "0xUserWalletAddress",
  "eventId": "12345",
  "outcome": "TeamA",
  "amountUSDC": 10
}
