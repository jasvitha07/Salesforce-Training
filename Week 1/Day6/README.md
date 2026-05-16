# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is used in Salesforce to get data from Salesforce objects.

### Example

```sql id="4id29d"
SELECT Name FROM Student__c
```

---

# 2. What is an Apex Trigger?

An Apex Trigger is Apex code that runs automatically when records are:

* Inserted
* Updated
* Deleted

### Example

Automatically generate Student ID after student registration.

---

# 3. Difference

## Flow vs Trigger

| Flow                       | Trigger                |
| -------------------------- | ---------------------- |
| No coding                  | Coding required        |
| Easy to create             | More powerful          |
| Used for simple automation | Used for complex logic |

---

## Before vs After Trigger

| Before Trigger            | After Trigger                  |
| ------------------------- | ------------------------------ |
| Runs before saving record | Runs after saving record       |
| Used for validation       | Used for notifications/actions |

---

# 4. Trigger Use Cases

1. Auto generate Student ID
2. Update available seats
3. Send attendance warning
4. Update fee payment status
5. Calculate exam grade automatically

---

# 5. Query Examples

### Get all CSE students

```sql id="g48sp4"
SELECT Name FROM Student__c
WHERE Department__c='CSE'
```

### Get students below 75% attendance

```sql id="l01dsh"
SELECT Name FROM Student__c
WHERE Attendance__c < 75
```

### Get paid fee records

```sql id="mnlc9h"
SELECT Name FROM Fees__c
WHERE Status__c='Paid'
```

---

# 6. Reflection

Enterprise systems react automatically to data changes to:

* Save time
* Reduce manual work
* Improve accuracy
* Provide faster updates

Example:
When fees are paid, the system automatically updates payment status and sends confirmation.

