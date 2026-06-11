# WooCommerce Mini CRM

A WordPress plugin that adds a lightweight customer-care CRM on top of WooCommerce. Sales teams can track leads from orders, manage follow-up calls, send SMS reminders, and report on conversion outcomes.

## Features

- Automatic lead creation from WooCommerce orders
- Call workflow with statuses: ready, calling, no buy, paid, duplicated, and more
- Row locking so agents do not work the same lead at once
- SMS pattern management and sending via Melipayamak
- Admin dashboards for records, reports, and call patterns
- Persian (Jalali) date picker support in the admin UI
- Scheduled cron jobs for paid-status checks, expiry, and duplicate detection
- Excel export support for reporting

## Requirements

- WordPress 6.3+
- PHP 7.4+
- WooCommerce (active)
- Melipayamak SMS API credentials (for SMS features)

## Installation

1. Download or clone this repository.
2. Upload the `woo-customer-retainerCall` folder to `wp-content/plugins/`.
3. Activate **Mini wp-Crm** from the WordPress plugins screen.
4. On activation, the plugin creates its database tables automatically.
5. Configure SMS API settings and call patterns from the plugin admin menu.

## Plugin structure

```
woo-customer-retainerCall/
├── assets/              # CSS, JS, fonts (Vue, Select2, Jalali datepicker)
├── inc/
│   ├── admin-call/      # Menus, AJAX handlers, CRM helpers
│   ├── admin-call-template/  # Admin page templates
│   └── cronjobs/        # Background status updates
└── woo-customer-retainerCall.php
```

## Usage

1. New WooCommerce orders can create CRM records automatically.
2. Agents open the CRM admin panel to claim and update call records.
3. Use SMS patterns for standardized follow-up messages.
4. Review reports and export data from the reporting section.

## Author

**Ayda Firouzi** — [@aydafirouzi](https://aydafirouzi.com/)

## License

GPL v2 or later (WordPress plugin standard).
