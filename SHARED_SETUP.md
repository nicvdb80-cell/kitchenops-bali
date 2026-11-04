# KitchenOps shared version

Source branch: kitchenops-shared. The standalone application is index.html at repository root.

## Vercel
Import nicvdb80-cell/kitchenops-bali as a NEW project named kitchenops-shared. Select branch kitchenops-shared. Framework preset: Other. Root directory: repository root. No build command or install command. Serve the repository root as static output. Keep the existing kitchenops-bali project unchanged.

## Shared orders
The initial sample workspace uses localStorage and does not synchronize across devices. Each person must use Connect live data and authenticate to the existing Supabase project. Live edits write to tenant central_office. Separate authorized database accounts must be provisioned for Nic and Yuli; do not share passwords. Database access and row-level policies have not been verified by this implementation.

## Claude handover
Edit index.html on kitchenops-shared. This version includes searchable order entry with supplier prices, event orders, combined purchase CSV, supplier and price management, and read-only recipe/dish costing. New events open ingredient search immediately. Monthly is planned purchasing only. Pricing shown in sample mode is illustrative. No supplier orders are transmitted automatically; adding items builds the purchase list.

Production authentication and multi-user access must be tested before operational use. Do not expose service-role keys or embed passwords in the frontend.
