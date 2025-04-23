Inventory Item Numbering System
This project introduces a **semi-automated item coding system** designed to streamline the categorization and tracking of donated inventory items in a nonprofit setting.
The goal is to replace inconsistent manual labeling with a structured, scalable, and filterable numbering system that reflects:

- **Item category** (e.g., meals, clothing, hygiene)
- **Program destination** (Drop-In, Outreach, Pantry)
- **Building location**
- **Item type classification**
Each item is assigned a code using this format:


Example:  
`0301.4-266`  
= Pantry department, Drop-In program, dry goods (type 4), stored in Main Building (266)

### Breakdown:
- **DepartmentCode** – Indicates the general category (e.g., 030 = Pantry)
- **ProgramCode** – Identifies the program (1 = Drop-In, 2 = Outreach, etc.)
- **ItemTypeCode** – Specifies sub-category (meals, dry goods, etc.)
- **BuildingCode** – Identifies storage location (266, 260, 151)

---

## 🔁 How It Works

- Uses a Python script that scans each item's:
  - `Name`
  - `Type`
  - `Tags`
- Matches against a **keyword mapping** dictionary
- Assigns the appropriate numeric codes
- Automatically generates the final formatted item number

---

## 📦 File Outputs

- `cleaning_workbook.xlsx` → Full dataset with assigned codes
- `needs_manual_review.xlsx` → Items that couldn't be categorized
- `category_keywords_for_hr.xlsx` → Approved keyword list for volunteers
- `mapped_inventory_report.xlsx` → Cleaned inventory with unmapped rows removed

---

## 👥 For Volunteers

Please refer to `category_keywords_for_hr.xlsx` when entering or tagging items. Only use approved keywords to ensure accurate mapping.

---

## 📂 Folder Structure (Suggested)

