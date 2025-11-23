# SAP SD – Availability Check (Explained in Super Simple Language)

This repository contains a beginner-friendly explanation of **Availability Check in SAP SD**.  
I created this guide so clear and simple that even a school student can understand how SAP checks stock before confirming a Sales Order.

---

## 📘 What You Will Learn

- What Availability Check means  
- Why it is important for Sales  
- How SAP decides availability  
- How Material Availability Date is calculated  
- What all stock types SAP includes  
- How complete & partial deliveries work  
- How Transfer of Requirements (TOR) goes to MRP  

---

## 🧠 What is Availability Check?

When a customer places an order, SAP must answer a simple question:

👉 **“Is the material available in the warehouse or not?”**

SAP checks:
- How much stock is available  
- When we can deliver  
- If customer’s requested date is possible  

---

## 🏭 Where Does SAP Check?

SAP checks stock at the **Plant level**.

Plant is determined from:
1. Customer-Material Info Record  
2. Ship-to Party Master  
3. Material Master  

You can also enter plant manually.

---

## 📅 Material Availability Date

SAP uses scheduling (delivery + transport time) to calculate:

**Material Availability Date**  
Stock must be available on this date.

---

## 📦 What Stock Types Does SAP Include?

SAP considers many elements like:

- Safety Stock  
- Stock in Transfer  
- Stock in Quality  
- Purchase Orders  
- Production Orders  
- Other Sales Orders  
- Reservations  

These settings come from customizing.

---

## 🔄 Transfer of Requirements (TOR)

When a Sales Order is created, SAP sends requirements to **MRP**.

MRP decides:
- Should we purchase material?
- Should we produce material?

---

## 🚚 Complete vs Partial Delivery

Customers may want:

### ✔ Only Complete Delivery  
Everything in one delivery.

### ✔ Partial Delivery  
Deliver whatever is available.

This can be controlled from:
- Customer Master  
- Customer-Material Info Record  
- Sales Order  

---

## 📝 Final Summary (Ultra Simple Words)

- Availability Check = checking stock before confirming the order  
- SAP decides rules from Material Master + Customizing  
- Check happens at plant level  
- Many stock types and orders are considered  
- Delivery preferences (full/partial) affect the result  
- MRP uses Sales Order requirements to plan stock  

---

## 🙋 About the Author

**Maharshi Shukla**  
SAP SD Learner | Building simple SAP content for everyone  
