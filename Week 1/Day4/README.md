# 🏫 College Management System – Automation & Flow Design

## 🃣 Automation Thinking

### 1. Auto Email After Registration

* When a student registers, the system automatically sends a confirmation email.
* It can include student details, login information, and course details.

🐠 **Why automation helps:**
Saves staff time and gives instant confirmation to students.

---

### 2. Auto Update Remaining Seats

* When a student joins a course, available seats reduce automatically.
* If a student cancels, seats increase automatically.

🐠 **Why automation helps:**
Avoids manual counting mistakes and keeps data accurate.

---

### 3. Notify Faculty When Course is Full

* When maximum students are enrolled, the system sends an alert to faculty/admin.

🐠 **Why automation helps:**
Faculty can quickly decide whether to open a new batch or stop registrations.

---

### 4. Generate Student ID Automatically

* After admission approval, the system creates a unique student ID automatically.

🐠 **Why automation helps:**
Reduces manual work and prevents duplicate IDs.

---

### 5. Send Reminder Before Fee Deadline

* Students receive automatic SMS/email reminders before fee due dates.

🐠 **Why automation helps:**
Improves fee collection and reduces late payments.

---

# 🃣 Flow Design Thinking

## Automation Chosen: Fee Reminder Automation

```text
          [Trigger]
   Fee due date is near
                │
                ▼
      Check student status
                │
      ┌─────────┴─────────┐
      │                   │
   Fees Paid?          Fees Not Paid
      │                   │
      ▼                   ▼
   Stop Flow        Send Reminder Email/SMS
                            │
                            ▼
                    Update reminder status
                            │
                            ▼
                       Final Action
```

---

# 🃣 Manual vs Automated Process

## Process: Student Fee Payment Reminder

### 🔹 Manual Process

* Staff checks student fee records manually.
* Staff prepares reminder messages.
* Emails/SMS are sent one by one.

### 🔹 Problems in Manual Process

* Takes too much time.
* Human errors may happen.
* Some students may miss reminders.
* Difficult when student count is high.

### 🔹 How Salesforce Automation Improves It

* Salesforce automatically checks due dates.
* Reminder emails/SMS are sent automatically.
* Records update instantly.
* Saves time and improves accuracy.

---

# 🃣 Reflection Task

## 🐠 Why should companies automate repetitive business processes?

Companies should automate repetitive business processes because automation:

* Saves time and reduces manual work.
* Improves accuracy and reduces human errors.
* Increases productivity.
* Gives faster service to customers/students.
* Helps employees focus on important tasks instead of repeating the same work.
* Improves overall business efficiency and performance.

