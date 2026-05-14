# Salesforce Data Modeling and Automation

## 1. Difference Between App, Object, Record, and Field

| Term | Definition | Example |
|---|---|---|
| App | A collection of tools, objects, tabs, and features designed for a specific business process. | College Management App |
| Object | A database table used to store related information. | Student Object |
| Record | A single entry stored inside an object. | One student's details |
| Field | A single piece of information inside a record. | Student Name, Roll Number |

---

## Simple Understanding

- **App** = Complete system  
- **Object** = Table  
- **Record** = Row in the table  
- **Field** = Column in the table  

---

## 2. Standard vs Custom Objects

| Standard Objects | Custom Objects |
|---|---|
| Already available in Salesforce | Created by users |
| Used for common CRM tasks | Used for organization-specific needs |
| Example: Account | Example: Student |

---

## 3. College Data Model

### Objects

- Student
- Faculty
- Course
- Department
- Attendance

### Relationships

| Parent | Child | Relationship |
|---|---|---|
| Department | Faculty | One-to-Many |
| Department | Course | One-to-Many |
| Student | Attendance | One-to-Many |

### Diagram

```text
Department
   |
   ├── Faculty
   ├── Course
            |
         Student
            |
       Attendance
```

---

## 4. Formula Fields

### Example 1: Total Marks

```text
Maths + Science + English
```

Automatically calculates total marks.

### Example 2: Percentage

```text
(Total_Marks / 300) * 100
```

Calculates percentage automatically.

---

## 5. Validation Rules

### Phone Validation

```text
LEN(Phone) <> 10
```

Ensures phone number has 10 digits.

### Email Validation

```text
NOT(CONTAINS(Email, "@"))
```

Checks valid email format.

---

## 6. Reflection

Structured enterprise data helps organizations store and manage information efficiently. It improves accuracy, reporting, automation, and decision-making.
