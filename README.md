# AWS DynamoDB – Student Management

A simple AWS DynamoDB project to manage student data using Create, Read, Update, and Delete operations.

## Project Overview

This project demonstrates basic student data management using **Amazon DynamoDB** and the **AWS Management Console**.

## AWS Service Used

- Amazon DynamoDB
- AWS Management Console

## DynamoDB Table

**Table Name:** `student-management`

**Partition Key:** `Student-ID`

| Attribute | Type | Key |
|---|---|---|
| Student-ID | String | Partition Key |
| Student-Name | String | - |
| Course | String | - |
| City | String | - |
| Age | Number | - |

## Operations Performed

### 1. Create
Created the `student-management` DynamoDB table and added student records.

### 2. Read
Retrieved a student record by using the `Student-ID` value.

### 3. Update
Updated the student record with `Student-ID = 102`.

- City changed from `Mumbai` to `Dhule`
- Course changed from `DevOps` to `Data Science`

### 4. Delete
Deleted the student record with `Student-ID = 101`.

### 5. Final Verification
Checked the table after the delete operation. The final table contains 3 records.

## Architecture Diagram

![AWS DynamoDB Architecture](architecture-diagram.png)

## Project Structure

```text
aws-dynamodb-student-management/
│
├── screenshots/
│   ├── 01_Create_DynamoDB_Table.png
│   ├── 02_Table_Created.png
│   ├── 03_Create_Student_Record.png
│   ├── 04_All_Student_Records.png
│   ├── 05_Query_Input.png
│   ├── 06_Query_Result.png
│   ├── 07_Before_Update.png
│   ├── 08_After_Update.png
│   ├── 09_Delete_Action.png
│   └── 10_Final_Table_After_Delete.png
│
├── architecture-diagram.png
└── README.md
```

## Screenshot Sequence

| No. | Screenshot | Purpose |
|---|---|---|
| 01 | `01_Create_DynamoDB_Table.png` | Create table and set partition key |
| 02 | `02_Table_Created.png` | Confirm table creation |
| 03 | `03_Create_Student_Record.png` | Create a student record |
| 04 | `04_All_Student_Records.png` | View all student records |
| 05 | `05_Query_Input.png` | Enter Student-ID for query |
| 06 | `06_Query_Result.png` | View the retrieved student record |
| 07 | `07_Before_Update.png` | Open record before update |
| 08 | `08_After_Update.png` | Show updated values |
| 09 | `09_Delete_Action.png` | Select the delete action |
| 10 | `10_Final_Table_After_Delete.png` | Verify final records after deletion |

## Result

The project successfully demonstrates basic DynamoDB student data management:

- Table creation
- Student record creation
- Record retrieval
- Record update
- Record deletion
- Final data verification

## Author

**AWS Cloud & DevOps Practice Project**
