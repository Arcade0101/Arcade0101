# Arcade

Full-stack engineer. I build production SaaS — TypeScript/Next.js on the front, Postgres and Python on the back.

Most of my work is commercial and lives in private repos, so what you see below is the write-up, not the source. Happy to walk through architecture or give code access on request.

---

### 🏪 StokaFlow — multi-tenant inventory SaaS
Inventory platform for small businesses in Rwanda still running stock on Excel. Sold as a hardware + software bundle (tablet kiosk + barcode scanner) on a monthly lease, which is what separates it from the software-only competition.

**Next.js 14 (App Router) · TypeScript · Tailwind · Supabase/Postgres · Docker · Google Cloud Run**

**[▶ Live at stokaa.com](https://stokaa.com)**

- Multi-tenant isolation enforced in **Postgres Row Level Security**, not the UI layer — every table scoped by `company_id` with `current_company_id()` / `current_effective_role()` policies
- Three-tier role model (Admin / Manager / Employee) plus a Manager-grantable "elevated" flag
- Hybrid auth: email-invite flow for staff with email, username + company-code login for staff without — synthetic addresses under the hood, since Supabase Auth requires an email
- In-browser **camera barcode scanning**, verified end-to-end on a physical phone
- Multi-stage Docker build → Cloud Build → Artifact Registry, Next standalone output

→ **[Read the full case study](https://github.com/Arcade0101/stokaflow-showcase)**

---

### ✈️ Orin — flight booking engine `private`
Travel booking MVP on the **Duffel** API. Built on real GDS/ticketing domain experience rather than a tutorial — search, offer selection, and order creation against live airline inventory.

### 💳 Peyaa — payments `private`
Fast-path payment flow.

### 📊 XAUUSD tooling — `Python` `private`
Trading journal and prop-firm risk tooling: rule tracking, drawdown limits, execution logging.

### 🤖 OrinPrime — shift assistant backend `private` `Python`
Scheduling and shift-management API.

---

### Stack

**Languages** TypeScript · Python · SQL · C#
**Frontend** Next.js · React · Tailwind CSS
**Backend** Node · Supabase · PostgreSQL (RLS, triggers, migrations) · REST APIs
**Infra** Docker · Google Cloud Run · Cloud Build · Artifact Registry

---

📍 Building from Japan, shipping for Rwanda.
