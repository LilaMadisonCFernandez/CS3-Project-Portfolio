# WORKSHEET 2
## Identify Objects, Classes, and Relationships

**Instructions:** Use the process and proposed system from Worksheet 1 to complete this worksheet.

---

## Part 1. Identify the Objects

Identify the important people, things, records, transactions, or concepts that your proposed system needs to represent.

**Guide Question:**

If you were going to create a program for this process, what things would the program need to represent?

| No. | Object | Description |
|:---:|---|---|
| 1 | Class Monitor | In charge of taking attendance and reporting of students who are absent/tardy/OB |
| 2 | Subject Teacher | Views and confirms the attendance during their subject |
| 3 | Class Adviser | Assigns class monitor and views attendance |
| 4 | Attendance Record | Contains information (date, time, subject, student name, type of infraction) |


### Object Evaluation

For each identified object, ask:

- Does it play an important role in the process?
- Does it contain information?
- Does it perform an action?
- Does it interact with another object?
- Does the proposed system need to keep track of it?

**Reminder:** Remove objects that are not necessary for your proposed system.

---

## Part 2. Analyze Object Interactions

Determine how your identified objects interact with one another.

**Example:** `Student → submits → Request`

| No. | Object 1 | Interacts | Object 2 |
|:---:|---|---|---|
| 1 | Class Monitor | Records and updates the attendance for the day. | Attendance Record |
| 2 | Class Adviser or Subject Teacher | Sees and checks the attendance record if it is accurate. | Attendance Record |
| 3 | Class Adviser | Updates the student monitor when needed. | Student Monitor |


---

## Part 3. Identify Possible Classes

Determine which objects can become classes in your proposed system.

Not every object needs to become a class. Choose only the objects that are important to your proposed system.

| No. | Class | What does it represent? |
|:---:|---|---|
| 1 | Person | General person in school |
| 2 | Attendance_Record | Contains a section’s attendance record |
| 3 | Class_Monitor | Student who is responsible for taking attendance |
| 4 | Subject_Teacher | Teacher who will review Class Monitor’s records |
| 5 | Class_Adviser | The teacher who is in-charge of a section; they keep attendance records and assigns a class monitor |

---

## Part 4. Class Analysis

Analyze the attributes and methods of each identified class.

### Class No. 1

**Class Name:** Person

**Purpose:**  
Generalizes a person in school

#### Attributes

| Attribute | Description |
|---|---|
| Name | Person’s name (for identification) |
| Age | Person’s age |
| Gender | Person’s gender |

#### Methods

| Method Name | What does it do? |
|---|---|
| None | None |

---

### Class No. 2

**Class Name:** Attendence_Record

**Purpose:**  
Contains information regarding the attendance

#### Attributes

| Attribute | Description |
|---|---|
| Student_Name | Student’s name (for identification) |
| Date | Date of attendance |
| Time | Time of attendance |
| Subject | Current subject |
| Type of Infraction | Type of infraction committed by student |

#### Methods

| Method Name | What does it do? |
|---|---|
| N/A | N/A |

---

### Class No. 3

**Class Name:** Class_Moniter

**Purpose:**  
Student who notes who is absent/tardy/OB in their class

#### Attributes

| Attribute | Description |
|---|---|
| Name | Monitor’s name (for identification) |
| Age | Monitor’s age |
| Gender | Monitor’s gender |
| Section | Monitor’s section |

#### Methods

| Method Name | What does it do? |
|---|---|
| Attendance_Check() | Identifies information of student (date, time, subject (optional), student name, type of attendance infraction) |
| Perfect_Attendance() | Records a perfect attendance for the class |

---

### Class No. 4

**Class Name:** Subject_Teacher

**Purpose:**
Teacher who will review Class Monitor’s records

#### Attributes

| Attribute | Description |
|---|---|
| Name | Subject Teacher’s name (for identification) |
| Age | Subject Teacher’s age |
| Gender | Subject Teacher’s gender |
| Section | Subject Teacher’s subject |

#### Methods

| Method Name | What does it do? |
|---|---|
| Display_Attendance() | Displays attendance record |
| Assign_Monitor() | Assigns who is in charge of checking the attendance |

---

**Additional Classes:** Add another copy of the Class Analysis section for each additional class you identify.

**Reminder:** Keep your project simple. Avoid creating unnecessary classes.

---

### Class No. 5

**Class Name:** Class_Adviser

**Purpose:**
Teacher who can display attendance records and assign a class monitor


#### Attributes

| Attribute | Description |
|---|---|
| Name | Class Adviser’s name (for identification) |
| Age | Class Adviser’ age |
| Gender | Class Adviser’ gender |
| Section | Class Adviser’ section |


#### Methods

| Method Name | What does it do? |
|---|---|
| View_Attendance() | Reviews attendance record in case of mistakes |

---
**Additional Classes:** Add another copy of the Class Analysis section for each additional class you identify.

**Reminder:** Keep your project simple. Avoid creating unnecessary classes.

## Part 5. Identify Class Relationships

Determine how your identified classes are related to one another.

| No. | Class 1 | Relationship | Class 2 | Why are they related? |
|:---:|---|---|---|---|
| 1 | Person | Inheritance | Class_Monitor | The Class_Monitor inherits the personal attributes from the person class. |
| 2 | Person | Inheritance | Subject_Teacher | The Subject_Teacher inherits the personal attributes from the person class. |
| 3 | Person | Inheritance | Class_Adviser | The Class_Advisor inherits the personal attributes from the person class |
| 4 | Class_Monitor | Association | Attendance_Record | The Class_Monitor records and updates the attendance record for the day. |
| 5 | Subject_Teacher | Association | Attendance_Record | The Subject_Teacher reviews the attendance records to check its accuracy. |

### Relationship Types

| Relationship | Description |
|---|---|
| **Association** | Two classes interact with one another. |
| **Aggregation** | One class groups or contains objects that can exist independently. |
| **Composition** | One class strongly owns another object. |
| **Inheritance** | One class is a specialized version of another class. |

**Reminder:** Use only the relationship types that make sense for your proposed system. Not all relationship types are required.
