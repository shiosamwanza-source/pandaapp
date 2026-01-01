# PANDA Backend

The backend will power the PANDA MVP.

We start very simple:

1️⃣ Authentication (login, users)
2️⃣ RFQs (Request for Quote)
3️⃣ Orders + timeline
4️⃣ Documents uploads (links only, not files in DB)
5️⃣ Live Verification scheduling (not video yet)

Important rule:

❌ No wallet
❌ No escrow
❌ No payments handling

We only store:

✔ data
✔ history
✔ proof
✔ organization
## API Structure (MVP)

The backend exposes a simple REST API.

### 1️⃣ Auth
- POST /auth/register
- POST /auth/login
- GET  /auth/me

### 2️⃣ RFQs (Request for Quote)
- POST /rfqs
- GET  /rfqs
- GET  /rfqs/{id}

### 3️⃣ Orders + Timeline
- POST /orders
- GET  /orders
- GET  /orders/{id}

### 4️⃣ Documents
- POST /documents (upload + attach to order)
- GET  /documents/{id}

### 5️⃣ Live Verification Scheduling
- POST /verification/request
- GET  /verification/my-requests
