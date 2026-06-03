# PRAVAAH UI STYLE GUIDE

## 1. Mandatory Template Rule

Every page must extend:

{% extends 'base.html' %}

Do NOT create:

* New Navbar
* New Sidebar
* New Footer

---

## 2. Official Color Palette

Primary Orange:
#ff5c1a

Hover Orange:
#d94400

Primary Black:
#0a0a0a

Background:
#f5f5f0

Navy Accent:
#0f1e45

Use only these colors.

---

## 3. Typography

Page Titles:
Class: pg-title

Section Titles:
Class: mod-title

Descriptions:
Class: mod-desc

---

## 4. Buttons

Primary Button:

class="btn-p"

Secondary Button:

class="btn-p-outline"

Do NOT use:

* btn-primary
* btn-success
* btn-danger

---

## 5. Cards

Use:

mod-card

or

p-card

Do not create custom card styles.

---

## 6. Tables

Use:

p-table-wrap
p-table

No custom table designs.

---

## 7. Forms

Labels:

p-label

Inputs:

p-input

---

## 8. Icons

Only Font Awesome Icons are allowed.

---

## 9. Layout

Use Bootstrap Grid:

row
col-md-*
col-lg-*

Avoid custom positioning.

---

## 10. Final Rule

If a page does not follow the PRAVAAH UI standard, it might be modified during integration.
