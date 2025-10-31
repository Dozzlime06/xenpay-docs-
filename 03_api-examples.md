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
Query Event

GET /api/events/12345

Query User Bets

GET /api/user/0xUserWalletAddress/bets

---

### **8. events.md**

```markdown
# Events

- Event ID, Name, Start Date, End Date  
- Example:  
  - 12345, World Cup Final, 2025-11-30 18:00 UTC, 2025-12-01 18:00 UTC
- All events are resolved on-chain, with outcomes automatically calculated
