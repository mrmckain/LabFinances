# LabFinances

Lab finance tracker and planner for the McKain Research Group (mckainlab.org/LabFinances). Admins only.

- Single self-contained `index.html`, no build step.
- Uses the Inventory Management (Lab Orders) Supabase project (`ksqjvvojoscyfyrkzqvm`) and its sign-in. Lab Orders accounts and orders feed in automatically.
- Tables: `fin_account_details`, `fin_transactions`, `fin_budget_lines`, `fin_planned`, `fin_outputs` (migration `supabase/inventory/supabase/migrations/20261120120000_lab_finances.sql` in the systems repo). All admin-only through RLS.
- Fiscal year runs October 1 – September 30 (`FY_START_MONTH` in the page).
