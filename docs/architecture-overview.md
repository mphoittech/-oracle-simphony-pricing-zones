# 🧭 Seasonal Pricing Zones Strategy – Oracle Simphony Cloud (EMC)

This project documents a scalable strategy for implementing seasonal pricing zones using **Oracle Simphony Cloud's Enterprise Management Console (EMC)**. The strategy aligns pricing updates with business campaigns to ensure operational efficiency and pricing accuracy across all Nando's outlets.

---

## 🧱 High-Level Zones Architecture

The seasonal pricing model is structured into four defined zones:

- ✅ **[1] Easter Zone** *(Active)*
- ⬜ **[0] Winter Zone**
- ⬜ **[0] Spring Zone**
- ⬜ **[0] Festive Zone**

Each zone connects directly to:
- **Menu Item Definitions** (for item availability, descriptions, etc)
- **Price Levels** (for zone-specific pricing structures)

🔁 Only **one zone** is active at a time, ensuring pricing consistency and reduced conflict.

![A_flowchart_diagram_illustrates_a_Seasonal_Pricing](https://github.com/user-attachments/assets/6b465d36-baca-40a4-89d7-4e5b2cdaf8bd)

---

## ⚙️ System Components

| Component | Description |
|----------|-------------|
| **Oracle Simphony Cloud (EMC)** | Central platform for managing pricing zones, menu items, and deployment across outlets |
| **Menu Item Definitions** | Logic and metadata defining each item across zones |
| **Zone Pricing Logic** | Business rules applied to define prices per zone |
| **Simphony Clients & POS** | Deployment targets that consume the configured logic for live pricing at stores |

---

## 📌 Deployment Flow

1. **Prepare price level configuration** according to the Combo Pricing document.
2. **Log into EMC** → `Enterprise Level → [100000] SA Master → Sub-Zone [1] SA Menu`.
3. **Add Seasonal Zones**: Easter, Winter, Spring, Festive.
4. **Create Effective Groups**:
5. **Override and distribute Menu Item Records**:
- Use the 'Keep Existing Record' method.
- Assign seasonal Effective Groups.
6. **Test deployments** to selected Halaal/non-Halaal outlets.
7. **Validate transactions** and monitor behavior across POS clients.

---

## 📁 Repository Structure

```bash
/
├── docs/
│   └── architecture-overview.md
│   └── emc_configuration_guide.md
│   └── process-flows.md
├── zone_config-samples/
│   ├── emc-config-checklist.md
│   ├── seasonal_zone_with_effective_groups.xml
│   ├── pricing_levels_config.xml
│   └── menu_definitions.xml
├── .gitgnore
├── LICENSE
├── README.md


