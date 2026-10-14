# Odoo Functional fieldnotes

A visual, interactive learning notebook for Odoo 19 and 20. Follow a fictional chair maker from customer inquiry through sales, purchasing, production, inventory, invoicing, cash collection, HR, payroll, and period close.

**Repository description:** Learn Odoo 19 & 20 functionally through 100 visual business stories, animated workflows, quizzes, practical configuration checklists, and live business labs covering Sales, Purchase, CRM, Accounting, Inventory, Manufacturing, Website, POS, HR, and Payroll.

## Open the course

Double-click `index.html`, or serve this folder's `dist` directory with any static web server. For example, run `python3 -m http.server 5173 --directory dist` and open http://localhost:5173.

No dependency installation, database, account, or build step is required. The website can operate locally; web fonts and official references need internet access, with local font fallbacks provided.

## Learning experience

- 100 lessons across 14 chapters and 300 topic-specific worked animation snapshots.
- Play/pause, pace control, next/back, timeline scrubbing, and keyboard-accessible object inspection.
- Every lesson has a familiar analogy, fictional story, functional explanation, prerequisite setup, role/menu starting point, three-step walkthrough, evidence checks, a pitfall, and a practical exercise with revealed reasoning.
- Prediction checks, reorder-the-steps puzzles, three quiz checks per lesson, feedback, retries, and recall prompts.
- Five live models: ordered/delivered invoicing, min/max replenishment, BoM scaling/material shortage, balanced invoice entries, and employee net/employer payroll cost.
- Odoo 19/20 selector with persistent browser preference, edition-specific official references, and contextual version/configuration notes. Core workflows common to both are explicitly identified as shared; differences are not invented.
- Search, bookmarks, personal notes, browser-local progress, exported progress JSON, and printable revision notes.
- Responsive layouts, keyboard controls, and reduced-motion support.

## Version and accounting scope

General accounting principles are used rather than any one country's tax or payroll law. Menu paths are starting points; actual screens and behavior depend on installed apps, edition, localization, settings, and access rights.

The course specifically covers the Odoo 19-and-later valuation model: Inventory reflects physical movement valuation; Accounting uses configured periodic-at-closing or perpetual-at-invoicing valuation, stock closing, and appropriate accrual review. It does not repeat the pre-19 blanket rule that every receipt/delivery posts a journal entry. Payment states and entries are also explained as configuration-sensitive.

Payroll lessons require the appropriate payroll localization and approved employment terms, salary structures, working calendars, and work entries. All wages, deductions, tax rates, and accounting amounts in examples are fictional arithmetic. They are not statutory setup recommendations.

## What the labs model

The live labs are small teaching models, not a full Odoo emulator. They do not connect to a database or create business records. Their simplified assumptions are stated on screen. Real dates, rounding, multiple components, partial returns, currencies, and localized salary rules must be verified in a configured training database.

Progress and notes are private to the current browser and site origin. Version switching preserves them. Clearing browser data removes them. JSON export is a backup of learning progress, not a cross-device synchronization feature.

## Curriculum

### 01. The connected business

Understand the records before clicking buttons.

- One business, connected apps
- Companies, currencies & fiscal context
- Contacts, invoice addresses & delivery addresses
- Products, variants & tracked goods
- Units of measure & conversion
- Roles, access rights & audit trails

### 02. CRM: from interest to opportunity

Qualify demand and organize the next conversation.

- Leads versus opportunities
- Pipeline stages & probability
- Activities, ownership & follow-up
- Teams, assignment & attribution
- From opportunity to quotation
- Won, lost & pipeline analysis

### 03. Sales: promise, delivery, invoice

Know exactly what has been sold and what can be billed.

- Build a complete quotation
- Confirm orders & linked documents
- Ordered versus delivered invoicing
- Pricelists, discounts & margin
- Down payments & final invoicing
- Service delivery, timesheets & milestones
- Returns, refunds & credit notes
- Sales analysis & document status

### 04. Purchase: buy with control

Connect vendor promises, receipts, and bills.

- RFQ versus confirmed purchase order
- Vendor prices, units & lead times
- Partial receipts & purchase backorders
- Vendor bill control & matching
- Supplier returns & vendor credits
- Dropshipping & alternative supply routes

### 05. Inventory: follow every unit

Locations, reservations, traceability, and replenishment.

- Warehouses, locations & ownership
- On-hand, forecast & reserved quantities
- Reservation methods & shortages
- Deliveries & backorders
- Lots, serials & traceability
- Min/max reordering rules
- MTO, Buy & Manufacture routes
- Physical counts & adjustments
- Standard, AVCO & FIFO costing
- Multi-step routes, barcode & landed costs

### 06. Manufacturing: make the promise real

Components, work, output, costs, and exceptions.

- Bill of materials: the recipe
- Manufacturing order lifecycle
- Component availability & shortages
- Work centers & capacity
- Work orders & shop-floor execution
- Actual consumption & flexible recipes
- Partial production & backorders
- Quality checks & scrap
- Estimated versus actual MO cost
- Subcontracting & unbuild

### 07. Accounting: build the foundation

Accounts, journals, taxes, terms, and balanced entries.

- Chart of accounts & account types
- Journals, sequences & documents
- Debits & credits without mystery
- Taxes & fiscal positions
- Payment terms & due dates
- Analytic accounts & cost attribution
- Opening balances & historical items
- Draft, posted, locks & access

### 08. Accounting: daily operations

Invoices, bills, payments, bank matching, and corrections.

- Customer invoices & receivables
- Vendor bills & payables
- Register payments & residuals
- Bank reconciliation
- Credit notes, reversals & refunds
- Payment differences & write-offs
- Aging, follow-ups & collection
- Expenses & reimbursement

### 09. Accounting: explain the period

Accruals, valuation, assets, currencies, and closing.

- Trial balance, P&L & balance sheet
- Inventory valuation in Odoo 19/20
- Receipts, deliveries & accruals
- Deferred expense & revenue
- Assets & depreciation
- Foreign currency & exchange differences
- Budget, analytics & management review
- Period close & audit trail

### 10. Website & eCommerce

Publish, sell online, and connect the order lifecycle.

- Website pages, editor & publication
- Online products, variants & catalogs
- Checkout, delivery & payment providers
- Online pricing, promotions & tax display
- Online orders, portal & returns
- SEO, forms & conversion analysis

### 11. Point of Sale

Operate the till and reconcile the retail day.

- POS configuration & products
- Sessions & opening cash
- Retail orders & split payments
- POS refunds & customer invoices
- Closing cash & session accounting
- POS resilience, restaurant & reporting

### 12. Employees & HR

People, permissions, recruitment, time, and leave.

- Employee records & private information
- Departments, managers & approvals
- Recruitment & onboarding
- Attendance, schedules & timesheets
- Time Off allocations & approvals
- Appraisals, equipment & offboarding

### 13. Payroll & payslips

Contracts, work entries, salary rules, and payment control.

- Employment terms & salary structures
- Work entries & conflict resolution
- Salary rules, allowances & deductions
- Payslip generation & review
- Pay runs, batches & payment control
- Payroll accounting, privacy & correction

### 14. Implementation & acceptance

Migrate, verify, train, and own the outcome.

- Discovery & process mapping
- Master-data migration & imports
- Integrations & automation boundaries
- User acceptance & exception testing
- Cutover, training & support ownership
- Oak & Co: the whole business capstone

## Content and maintenance

`dist/curriculum.js` contains the lesson data, exercises, references, and worked snapshots. `dist/config.js` defines chapters and site identity. `dist/subject.js` implements the Odoo version context and live business labs. `dist/notebook.js` implements the visual notebook; `dist/app.js` handles shared navigation and progress. Styles are in the three CSS files.

All text and diagrams are original. The visual teaching approach is inspired by notebook-style educational books, including the Head First series; no book text, pages, or brand assets are reproduced. This is an independent educational project, not an official Odoo or Head First publication.

## Verification

- All 100 lessons and all 300 frames rendered at 1440px and 390px widths in both version contexts without detected page errors or horizontal overflow.
- Quiz data checked for valid answers and distinct choices.
- All 72 distinct edition-specific documentation URLs returned HTTP 200 at creation.
- Live arithmetic checked for ordered/delivered policy, previous invoices, replenishment multiples and invalid settings, BoM scaling and zero output, balanced/unbalanced entries, and employee versus employer payroll amounts.

## Primary references

- [Odoo 19 documentation](https://www.odoo.com/documentation/19.0/)
- [Odoo 20 documentation](https://www.odoo.com/documentation/20.0/)
- [Odoo 19 accounting inventory valuation](https://www.odoo.com/documentation/19.0/applications/finance/accounting/get_started/inventory_valuation.html)
- [Odoo 20 valuation cheat sheet](https://www.odoo.com/documentation/20.0/applications/inventory_and_mrp/inventory/inventory_valuation/cheat_sheet.html)
- Each lesson links directly to its selected edition's relevant official reference.
