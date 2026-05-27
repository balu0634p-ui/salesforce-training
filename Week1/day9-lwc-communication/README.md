# Component Communication

Component Communication in LWC is used to share data between different components inside a Salesforce application. Components can communicate from parent to child, child to parent, or between unrelated components.

## Types of Component Communication

### 1. Parent to Child Communication
Data is passed using public properties with @api decorator.

### 2. Child to Parent Communication
Events are used to send data from child components to parent components.

### 3. Communication Between Unrelated Components
Publish-Subscribe model or Lightning Message Service (LMS) is used.

Component communication helps applications become modular, reusable, and organized.

---

# Dashboard Design

The dashboard is designed to display important business information in a simple and interactive way.

## Dashboard Features

- Total Customers
- Total Opportunities
- Recent Activities
- Reports and Charts
- Notifications
- Navigation Menu

## Dashboard Components

| Component | Purpose |
|-----------|---------|
| Header | Navigation and branding |
| Sidebar | Menu options |
| Statistics Cards | Shows quick data summary |
| Charts Section | Visual representation of reports |
| Recent Activity Panel | Displays latest updates |
| Footer | Additional information |

The dashboard provides users with quick access to important CRM data and improves decision-making.

---

# Data Flow Explanation

Data flow explains how information moves inside the Salesforce system.

## Step-by-Step Flow

1. User enters data through the UI screen.
2. LWC component captures the data.
3. JavaScript handles frontend processing.
4. Data is sent to Apex backend methods.
5. Apex communicates with Salesforce database.
6. Database stores or retrieves records.
7. Updated data is returned to the LWC component.
8. UI refreshes and displays updated information.

## Example

Customer Form → LWC Component → Apex Class → Salesforce Database → Updated Dashboard

This process ensures smooth communication between frontend and backend systems.

---

# Aura vs LWC

| Feature | Aura Components | Lightning Web Components (LWC) |
|---------|----------------|-------------------------------|
| Technology | Salesforce-specific framework | Standard web technologies |
| Performance | Slower | Faster |
| Complexity | More complex | Simpler |
| Coding Style | Event-based | Modern JavaScript |
| Reusability | Moderate | High |
| Learning Curve | Difficult | Easier |
| Security | Good | Improved security |
| Development Speed | Moderate | Faster |

## Conclusion
LWC is preferred over Aura because it provides better performance, cleaner code, and modern development standards.

---

# Reflection

This topic helped me understand how Salesforce components communicate and how data moves through the system. I learned the importance of dashboard design in CRM applications and how frontend and backend are connected using LWC and Apex. Comparing Aura and LWC made it clear why Salesforce recommends LWC for modern application development. The practical understanding of component communication and data flow improved my knowledge of Salesforce architecture.
