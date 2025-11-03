### 📞 Maintaining Condition Master Data for Pricing

#### 🏁 Lesson Objective

After this lesson, you will be able to:

* Create and maintain **Condition Master Data** for pricing in SAP.

---

### 💡 What is Condition Master Data?

Condition Master Data helps SAP decide the **price**, **discount**, **freight**, and **taxes** for each sale.

You can think of it like a rulebook that tells SAP:

> When you sell this product to this customer, this is the price, and this is the discount.

Examples:

* A price specific to one customer
* A discount depending on both **customer** and **material group**

---

### ⚙️ How Condition Master Data Works

Every condition (price, discount, or tax) has a **Condition Type**.
When creating a record, you first choose a **Condition Type.**

The Condition Type controls:

* The kind of condition (Price, Discount, Tax, etc.)
* If scales (quantity-based or value-based) are allowed
* Whether it applies to the **header** or **item** level
* The validity period (from–to dates)

Examples:

* **PR00** = Basic Price
* **K007** = Customer Discount
* **KF00** = Freight

---

### 🔍 How Pricing Happens

When you create a **Sales Order**, SAP automatically finds the right **Condition Records** using a process called **Condition Technique.**

It checks:

* Which condition types are active
* If any master record exists for that customer/material
* Copies the correct price or discount into the order automatically

If allowed, you can even change the value **manually** (for example, to give an extra discount to a loyal customer).

---

### 🧠 In Simple Words

Condition Master Data = The rules that tell SAP how to calculate prices and discounts for each sale.

---

### 🔖 Example

If Customer A buys Product X → Price = ₹1000
If Customer B buys Product X → Price = ₹950
➡ This difference comes from **Condition Master Data.**

---

### 🔧 T-Codes

* **VK11** → Create Condition Record
* **VK12** → Change Condition Record
* **VK13** → Display Condition Record

---

### 📚 Summary

* Helps SAP find the correct price, discount, freight, and tax
* Uses predefined condition types like **PR00**, **K007**
* Works automatically during sales document creation
* Can be changed manually (if allowed)

---

### 🏷️ Hashtags

#SAP #SAPSD #SAPS4HANA #Pricing #ConditionMasterData #SAPLearning #SAPTraining #ERP #SalesAndDistribution #LearnSAP #SAPCommunity #BusinessProcess
