# Salesforce SOQL and Apex Triggers

# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is a query language used in Salesforce to retrieve data from objects.

It is similar to SQL but designed specifically for Salesforce objects and records.

SOQL helps developers:
- Fetch records
- Filter data
- Retrieve specific fields
- Work with relationships between objects

---

## Example SOQL Query

```sql
SELECT Name, Email FROM Student__c
```

### Explanation
This query retrieves the Name and Email fields from the Student object.

---

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that automatically executes before or after events occur in Salesforce records.

Triggers respond to actions such as:
- Insert
- Update
- Delete
- Undelete

Triggers help automate backend business logic.

---

# 3. Difference Between

## Flow vs Trigger

| Flow | Trigger |
|---|---|
| No-code automation tool | Apex programming automation |
| Easy to create | Requires coding |
| Best for simple logic | Best for complex logic |
| Drag-and-drop interface | Written in Apex code |
| Limited customization | Highly customizable |

---

## Before Trigger vs After Trigger

| Before Trigger | After Trigger |
|---|---|
| Runs before record is saved | Runs after record is saved |
| Used for validation and updating fields | Used for related records and notifications |
| Faster processing | Used when record ID is needed |
| Can modify record values directly | Cannot directly modify same record |

---

# 4. Trigger Use Cases

## 1. Automatic Student ID Generation

When a new student record is created, a unique student ID is generated automatically.

---

## 2. Attendance Warning Trigger

If attendance falls below 75%, a warning email is automatically sent.

---

## 3. Fee Due Notification

When fee due date approaches, triggers send reminder notifications.

---

## 4. Course Enrollment Update

When students enroll in a course, the total student count updates automatically.

---

## 5. Faculty Assignment Notification

When a faculty member is assigned to a course, a notification email is sent automatically.

---

# 5. Query Examples

## Example 1

### English Query
Get all student names and email addresses.

### SOQL Query
```sql
SELECT Name, Email__c FROM Student__c
```

---

## Example 2

### English Query
Find students whose attendance is below 75%.

### SOQL Query
```sql
SELECT Name, Attendance__c FROM Student__c
WHERE Attendance__c < 75
```

---

## Example 3

### English Query
Retrieve all courses under the Computer Science department.

### SOQL Query
```sql
SELECT Name FROM Course__c
WHERE Department__c = 'Computer Science'
```

---

## Example 4

### English Query
Get all faculty members with more than 5 years of experience.

### SOQL Query
```sql
SELECT Name, Experience__c FROM Faculty__c
WHERE Experience__c > 5
```

---

# 6. Reflection

Enterprise systems react automatically to data changes because organizations need fast, accurate, and real-time processing. Manual monitoring becomes difficult when large amounts of data are involved.

Salesforce uses triggers, flows, and automation tools to respond instantly whenever records are created, updated, or deleted. This improves efficiency, reduces errors, and ensures smooth business operations.

Automatic reactions help enterprise systems become scalable, intelligent, and reliable.
