✨ Features
🔹 1. Multi-Step Navigation

The form is split into multiple steps:

Personal Info

Select Your Plan

Pick Add-ons

Review Summary

Confirmation Screen

Each step updates the global form state properly using React Context + Reducer.

🔹 2. Plan Selection

Users can choose between:

Arcade

Advanced

Pro

Each plan has both monthly and yearly pricing.

The pricing system updates automatically based on the billing toggle.

🔹 3. Billing Toggle

A switch allows users to choose:

Monthly billing

Yearly billing (with discounts)

The UI updates instantly for both plans and add-ons.

🔹 4. Add-ons Selection

Users can pick optional add-ons such as:

Online Service

Larger Storage

Customizable Profile

Add-ons are priced differently for monthly and yearly billing.

🔹 5. Summary Calculation

The summary page automatically calculates:

Selected plan price

Add-ons total

Grand total (per month or per year)

No hardcoding — all values come from real state.

🔹 6. Global State Management

All form details are managed using:

React Context

useReducer

TypeScript

This ensures clean, predictable flow through every step.

🛠️ Tech Stack

React

TypeScript (TSX)

CSS Modules

React Context + Reducer

Local JSON data fetching

📂 Folder Structure
/src
  /components
  /context
  /pages
  /styles
  plans.json

📌 How It Works
1. PlanContext

Stores:

Current plan

Billing type (monthly/yearly)

Selected add-ons

Pricing tables

2. Reducer

Handles actions like:

Select plan

Toggle billing

Select add-on

Load plans/add-ons from JSON

3. Summary Page

Dynamically calculates totals using reducer state.

🚀 Setup
npm install
npm run dev
