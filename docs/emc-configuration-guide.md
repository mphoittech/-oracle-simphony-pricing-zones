## 🧩 How to Deploy Seasonal Pricing Zones using Oracle Simphony Cloud EMC

### ✅ **Step 1: Prepare Price Level Configuration**

* Ensure all required price levels for seasonal pricing are predefined.
* These should align with the **Combo Pricing Document** and reflect all zone-specific variations.

---

### ✅ **Step 2: Log in to EMC and Navigate Hierarchy**

* Log in to **EMC**.
* Navigate to:

  ```
  Enterprise Level → [100000] - SA Master
                   → Sub-Zone [1] - SA Menu
  ```

---

### ✅ **Step 3: Zone Configuration**

* In the **'SA Master' Zone**, add the following **Seasonal Zones**:

  * `Easter`
  * `Winter`
  * `Spring`
  * `Festive & B2W` (Back to Work)

---

### ✅ **Step 4: Configure Effective Groups**

* At the **highest hierarchy level**, add the following:

  ```
  Effective Group [1] → Easter Price Increase
  Effective Group [2] → Winter Price Increase
  Effective Group [3] → Spring Price Increase
  Effective Group [4] → Festive Price Increase
  ```
* Ensure only **one active Effective Group per Seasonal Zone**.
* Set **overrides on other Effective Groups** to expire during each seasonal window.

---

### ✅ **Step 5: Seasonal Zone Override Definition Records (Menu Item Maintenance)**

* Go to:

  ```
  EMC → Menu Item Maintenance → [Seasonal Zone]
  ```
* Select **all Definition Records** (excluding Header Records).
* Use `Keep Existing Record` as your override method to preserve inherited logic.

---

### ✅ **Step 6: Distribute Price Records**

* At the **Enterprise Level**:

  * Go to `Menu Item Maintenance → Price Records`
  * Select all (excluding Header Records).
  * Distribute to each **Seasonal Zone**.
  * Update each record’s **Effective Group** to match the corresponding Seasonal Zone.

---

### ✅ **Step 7: Clean-up**

* Once distributed:

  * All **Definition and Price Records** will be removed from Enterprise Level.
  * Master (Header) records will remain intact.
  * Seasonal zones now contain targeted pricing configurations.

---

## 📌 Final Notes:

* **Deploy changes** to test outlets first (Halaal & non-Halaal) for validation.
* **Monitor trade performance**, and adjust if needed.
* Ensure each zone’s **start and end date** is configured according to the annual trading calendar.


