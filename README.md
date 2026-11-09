# mini-project
# 🚜 Tractor Fleet Flow — Cloud Agri-Fleet & Financing Platform
A unified, multi-tenant agricultural machinery fleet, subsidy, and loan financing management platform with full relational integrity and multi-role authentication.
## 🌟 Key Features
1. **Relational Database Integrity & Foreign Key Linking**:
   - **`Farmers` (Core Anchor)**: When a farmer is registered, a unique primary key (e.g. `FARM-001`) is issued.
   - **`Purchases` (Junction Table)**: Links `farmer_id` (FK) + `tractor_id` (FK) + `dealer_id` (FK) + optional `scheme_id` (FK). Dynamically calculates subsidy discount and net payable balance.
   - **`Loans` (Financing Link)**: Connected via `farmer_id` (FK) and `purchase_id` (FK). Automatically calculates monthly EMI across various tenures and interest rates.
   - **`Farmer 360° Dossier`**: Click any farmer to instantly inspect their full history: all tractors owned, government subsidies availed, and active bank loans with repayment status.
2. **Multi-Role Authentication & Regional Workflows**:
   - **Admin Portal**: Master clearance across all territories, fleet analytics, scheme configuration, and regional distribution heatmap.
   - **Dealer Portal**: Scoped to assigned region (North, West, Central, South). Enables regional inventory stocking and direct tractor sales to farmers.
   - **Farmer Portal**: Self-service portal for farmers to track tractor purchases, status of loan approvals, and subsidy disbursements.
3. **Real-Time Cloud Synchronization**:
   - Employs the HTML5 `BroadcastChannel` and persistent client storage.
   - Any transaction logged in one browser tab (e.g., as a Dealer) instantly synchronizes across all open windows (e.g., the Admin dashboard) with a live activity feed.
---

Website link:
https://shahunikam22.github.io/mini-project/
