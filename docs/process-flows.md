# Process Flows

### 🔄 **Seasonal Pricing Zone Process Flow (Oracle Simphony Cloud via EMC)**

---

#### 1. 🗓 **Identify Seasonal Periods & Define Zones**

* Define the upcoming seasonal cycle (e.g., moving from **Easter ➝ Winter**).
* Create or update **Seasonal Zones** in EMC:

  * Example: `ZONE_EASTER`, `ZONE_WINTER`, `ZONE_SPRING`, `ZONE_FESTIVE`

---

#### 2. 🧾 **Menu Item Maintenance**

* Navigate to **Menu Item Maintenance** → **Definition Records** (exclude Header Records).
* Highlight and select all items applicable to the seasonal campaign.
* Assign records to the **identified seasonal zone** using EMC's zone management.

---

#### 3. 🛠 **Update Effective Groups**

* Modify the **Effective Groups** in EMC:

  * Link them to the new **Seasonal Zone**
  * Align menu items, price levels, and combo structures with current campaign pricing strategy.

---

#### 4. 🧪 **Deploy Test Properties**

* Select appropriate **test outlets** within each zone:

  * Ensure representation by **Halaal** and **non-Halaal** sites.
* Push updates to these test properties only, using EMC's drag test outlets via Zone Configuration.

---

#### 5. 💸 **Configure Price Levels (Combo Pricing)**

* Refer to the **Combo Pricing Document**
* Configure:

  * Base price levels , all channels
  * Combo logic (e.g., add-A-Drink&SAVE, negative/positive bundled pricing)
  
---

#### 6. ✅ **Validate Pricing Updates**

* Use test POS transactions at each test outlet:

  * Confirm prices reflect updated zone and combo logic
  * Verify combo and individual item behavior at POS

---

#### 7. 📊 **Monitor & Adjust**

* Monitor trading performance and pricing behavior

  * Look for discrepancies, configuration-defacts, or pricing issues
* Adjust EMC configuration as needed

  * Finalize for full deployment once testing is successful

---

## Example Flow

![Oracle Simphony Cloud (EMC) X](https://github.com/user-attachments/assets/fdab3a3d-9d52-46fd-9a54-8a0df24104d4)


