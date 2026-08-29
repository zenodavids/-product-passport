# Product Passport
EU DPP 2027-compliant digital product passport platform for textiles, electronics, and consumer goods.

Live demo: https://productpassport-wo.vercel.app/

### What it does:
Brands create digital passports for their products. Each passport gets a dynamic QR code that updates in real time without reprinting. Supports tiered access so manufacturers, auditors, and consumers see different data.


#### Stack
Next.js 14, TypeScript, Node.js, Firebase


### One hard decision
I chose Firebase over PostgreSQL for the real-time QR updates because I needed sub-second propagation to the QR resolver without managing WebSocket infrastructure. For audit trails and relational compliance data, I would use PostgreSQL in a v2.
