# Beauty Parlour Billing Software - Setup Guide

## Quick Start

Your beauty parlour billing software is now ready to use! Here's what's included and how to get started.

## Database Connection

The application is connected to a Supabase database with the following tables:

- **Categories** - Product categories (Skincare, Makeup, Haircare, etc.)
- **Products** - Cosmetics inventory with SKU, barcode, pricing
- **Services** - Beauty services with duration and pricing
- **Stock Movements** - Track all inventory changes
- **Invoices** - Sales records with payment details
- **Invoice Items** - Line items for each invoice
- **Settings** - Store configuration and preferences
- **Users** - User management and audit trail

## Pre-loaded Sample Data

The database comes with 5 sample categories:
- Skincare
- Haircare
- Makeup
- Fragrances
- Tools

## Features Available

### 1. **Billing** (Main Dashboard)
- Create invoices with products and services
- Barcode scanner support
- Apply discounts (percentage or fixed amount)
- Automatic tax calculation
- Multiple payment methods
- Print invoices

### 2. **Products Management**
- Add/edit/delete products
- SKU and barcode tracking
- Purchase and sale pricing
- Tax rate per product
- Stock quantity management
- Low stock alerts
- Product categorization
- Product images

### 3. **Categories Management** (New!)
- Create and organize product categories
- Edit category details
- Delete unused categories
- Search categories

### 4. **Services Management**
- Add/edit/delete beauty services
- Set duration and pricing
- Apply tax rates
- Activate/deactivate services

### 5. **Stock Management**
- Add stock purchases
- Track stock movements
- View stock history
- Low stock alerts
- Stock value calculation

### 6. **Reports & Analytics**
- Daily/periodic sales reports
- Profit calculation
- Top-selling products
- Low stock product list
- Date range filtering
- CSV export

### 7. **Settings**
- Store information (name, address, phone)
- Invoice numbering prefix
- Default tax rate
- Logo upload support

## How to Use

### Adding a Product

1. Go to **Products** menu
2. Click **Add Product**
3. Fill in the details:
   - **SKU**: Unique product identifier
   - **Barcode**: Optional, for scanner support
   - **Category**: Select from pre-created categories
   - **Prices**: Purchase and sale prices
   - **Tax Rate**: Applied at checkout
   - **Stock**: Current quantity
   - **Image**: Product image URL
4. Click **Add Product**

### Creating an Invoice

1. Go to **Billing** menu
2. Search for products/services or scan barcode
3. Add items to cart by clicking on them
4. Adjust quantities using +/- buttons
5. Apply discount if needed
6. Select payment method
7. Click **Checkout & Print**
8. Preview and print invoice

### Managing Categories

1. Go to **Categories** menu
2. View all existing categories
3. **Add Category**: Click "Add Category", enter name and description
4. **Edit**: Click "Edit" on any category card
5. **Delete**: Click "Delete" (products won't be affected, just uncategorized)
6. **Search**: Find categories by name or description

### Viewing Reports

1. Go to **Reports** menu
2. Select date range
3. View sales metrics, top products, and low stock alerts
4. Export to CSV for spreadsheet analysis

## Important Notes

- All data is saved to Supabase in real-time
- Stock is automatically decremented when invoices are created
- Low stock alerts appear when inventory falls below threshold
- Invoice numbers are auto-generated based on settings
- Tax is calculated per item at checkout

## First Steps

1. Go to **Settings** and update store information
2. Go to **Categories** and review/add more categories as needed
3. Go to **Products** and start adding your products
4. Go to **Services** and add your beauty services
5. Go to **Billing** and create your first invoice

## Support

For database or technical issues, check:
- Database connection in `.env` file
- Supabase dashboard for table status
- Browser console for error messages

All features are production-ready and tested!