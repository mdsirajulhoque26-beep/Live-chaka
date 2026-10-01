# Chaka Live Spin — Real Core Version

Core real functionality added:
- Server-side registration/login with scrypt password hashing and signed session tokens.
- Persistent JSON database in `data/db.json` (replace with PostgreSQL/MySQL before high-scale production).
- Real server-side wallet balance and bet ledger.
- Six betting slots with server-side balance deduction.
- Deposit requests and withdrawal requests with admin approval/rejection.
- Admin authentication, user list and transaction controls.
- Demo audience/feed sections intentionally omitted from the core screen.

## Run
1. `cp .env.example .env`
2. Set a strong `SESSION_SECRET` and `ADMIN_PASSWORD`.
3. `npm install`
4. `npm run dev`

## Important
No payment gateway was present in the supplied source. Deposit is therefore an admin-approved deposit request, not a connected mobile-banking/card gateway. Connect a verified payment provider before accepting real-world payments.
