# Arcade

Full-Stack Engineer specializing in TypeScript/Next.js frontends and Python/PostgreSQL backends.

Most projects are commercial and closed-source; the projects below are presented as technical summaries.

---

### StokaFlow — Multi-Tenant Inventory SaaS

**Next.js 14 · TypeScript · Tailwind CSS · Supabase/PostgreSQL · Docker · Google Cloud Run**

Live: [stokaa.com](https://stokaa.com) · Case study: [stokaflow-showcase](https://github.com/Arcade0101/stokaflow-showcase)

- Designed multi-tenant data isolation using PostgreSQL Row Level Security (RLS), scoped by `company_id`
- Implemented a three-tier role system: Admin, Manager, and Employee, with a Manager-grantable elevated permission
- Built hybrid authentication supporting email-based staff invitations and username + company-code authentication for staff without email
- Implemented in-browser camera-based barcode scanning

### Orin — Flight Booking Engine `private`

**Duffel API · REST APIs**

- Integrated the Duffel API for flight search, offer selection, and order creation against live airline inventory

### Peyaa — Payment Processing `private`

**Payment APIs · Backend Integration**

- Built payment-processing workflows and supporting backend integration

### OrinPrime — Shift Management Backend `private`

**Python · REST API · Scheduling**

- Developed a backend API for scheduling and shift-management workflows

---

### Technical Stack

**Languages** TypeScript · Python · SQL · C#
**Frontend** Next.js · React · Tailwind CSS
**Backend & Data** Node.js · Python · Supabase · PostgreSQL · Row Level Security · Database Triggers · Migrations · REST APIs
**Infrastructure & Cloud** Docker · AWS · Google Cloud Run · Google Cloud Build · Artifact Registry
