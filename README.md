# 🚗 WhatNext Vision Motors
### Driving the Future of Mobility through Innovation and Excellence

**Developer:** Hans Edwin Y. Maybituin  
**Institution:** Asia Pacific College  
**Course:** BS – Information Technology (MI-221)

---

## 📘 Overview

**WhatNext Vision Motors** is a Salesforce-based application designed to simplify and automate vehicle management operations for automotive businesses.  
It enables efficient handling of vehicles, dealers, customers, test drives, and service requests — all within a unified platform powered by **Salesforce Lightning**, **Apex triggers**, **batch jobs**, and **automation flows**.

The project highlights Salesforce’s capabilities in creating **custom objects**, **workflow automation**, and **scheduled background processes** to enhance productivity and business accuracy.

---

## ⚙️ Key Features

### 🧱 1. Custom Objects
The system includes multiple **custom objects** to represent real-world entities:

- **Vehicle__c** – Stores vehicle details such as model, price, and stock quantity.  
- **Vehicle_Dealer__c** – Contains information about partner dealerships.  
- **Vehicle_Order__c** – Manages customer vehicle purchase records.  
- **Vehicle_Customer__c** – Stores customer information and contact details.  
- **Vehicle_Test_Drive__c** – Tracks and schedules customer test drives.  
- **Vehicle_Service_Request__c** – Logs customer service or maintenance requests.

---

### ⚡ 2. Lightning App
A **Salesforce Lightning App** was created to integrate all the system components into a single, intuitive interface.  
Users can easily navigate between custom objects and perform key operations such as managing vehicles, dealers, and orders.

---

### 🔄 3. Automation Flows
Automation flows ensure smoother business operations by reducing manual effort:

- **Auto Assign Dealer** – Automatically assigns the correct dealer when a vehicle or order record is created.  
- **Test Drive Reminder** – Sends alerts or reminders for scheduled customer test drives.

---

### 🧠 4. Apex Classes and Triggers
Custom **Apex code** was implemented to handle backend logic and automated processes.

| Component | Description |
|------------|-------------|
| `VehicleOrderTriggerHandler` | Contains reusable methods to manage vehicle order logic. |
| `VehicleOrderTrigger` | Trigger that calls the handler when a `Vehicle_Order__c` record is created or updated. |
| `VehicleOrderBatch` | Batch Apex job for processing large sets of vehicle order data. |
| `VehicleOrderBatchScheduler` | Scheduler class that runs batch jobs automatically at defined intervals. |

---

### 🧾 5. Batch and Trigger Jobs
These jobs help maintain system accuracy and automate stock or order-related updates.

**Example Logic:**
> When a vehicle order is created, the system checks if the stock quantity is available.  
> - If **stock quantity = 0**, it prevents over-ordering and can initiate restock notifications.  
> - The batch process ensures data remains consistent and up to date.

---

## 🧩 Technology Stack

- **Platform:** Salesforce (Lightning Experience)  
- **Language:** Apex  
- **Automation Tools:** Salesforce Flows & Scheduled Batch Jobs  
- **Database:** Salesforce Object Storage (Custom Objects)  
- **Interface:** Salesforce Lightning App

---

## 🚀 Setup and Deployment

1. **Log in** to your Salesforce Developer Org.  
2. **Create the following Custom Objects:**
   - `Vehicle__c`
   - `Vehicle_Dealer__c`
   - `Vehicle_Order__c`
   - `Vehicle_Customer__c`
   - `Vehicle_Test_Drive__c`
   - `Vehicle_Service_Request__c`
3. **Develop the Lightning App** and include all relevant tabs.  
4. **Upload and deploy Apex classes:**
   - `VehicleOrderTriggerHandler`
   - `VehicleOrderTrigger`
   - `VehicleOrderBatch`
   - `VehicleOrderBatchScheduler`
5. **Set up the Flows:**
   - Auto Assign Dealer  
   - Test Drive Reminder  
6. **Test the system** using sample vehicle and customer records.

---

## 🌱 Future Improvements

- Integration with third-party APIs for live vehicle data.  
- Dashboard analytics for sales, customer behavior, and service tracking.  
- Email and SMS notification integration for service updates and test drive confirmations.  
- Enhanced error handling for large-scale data operations.

---

## 👨‍💻 Author

**Hans Edwin Y. Maybituin**  
Bachelor of Science in Information Technology  
Asia Pacific College – MI-221

---

