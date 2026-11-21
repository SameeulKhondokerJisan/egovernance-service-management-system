# Government E-Governance Service Management System

## Overview
The Government E-Governance Service Management System is a console-based application written in C that simulates digital government services. The system allows administrators to manage citizen service requests, process tax records, and analyze tax data.

The system also includes authentication, activity logging, and file-based data storage to maintain government service records.

## Features

### Authentication System
- Admin login with username and password
- Passwords stored as djb2 hashes (a simple teaching hash, not secure for real credentials)
- Automatic admin account initialization

### Service Request Management
- Submit new citizen service requests
- View submitted requests
- Update request status (Pending, Approved, Rejected)

### Tax Management
- Record citizen income
- Automatically calculate tax (15% rate)
- Store tax records

### Tax Analytics
The system analyzes tax data and provides statistics including:
- Total tax records
- Average tax amount
- Variance
- Standard deviation

### Activity Logging
All system operations are logged including:
- Admin login
- Service request submission
- Request status updates
- Tax calculation
- Analytics generation
- System exit

## Technologies Used
- C Programming Language
- Standard C Libraries
- File-based persistent storage

## System Data Files

| File | Purpose |
|-----|-----|
| service_requests.dat | Citizen service request records |
| tax_records.dat | Tax calculation records |
| egov_users.dat | User authentication data |
| egov_logs.txt | System activity logs |

## Build and Run

Needs a C compiler (gcc or clang).

```bash
gcc egovernance_system.c -o egovernance_system -lm
./egovernance_system
```

On macOS, `-lm` is optional. The program creates its `.dat` data files and log file on first run.

## Project Report

Design and feature walkthrough: [docs/EGSMS-project-report.pdf](docs/EGSMS-project-report.pdf)

## Default Admin Login

Created automatically on first run.

Username: admin  
Password: admin123

## Program Menu

1. Submit Service Request  
2. View Requests  
3. Update Request Status  
4. Calculate Tax  
5. Tax Analytics  
6. Exit  

## Learning Objectives

This project demonstrates:

- File handling in C
- Government service system simulation
- Authentication using hashing
- Logging systems
- Data management structures
- Statistical analytics
- Console-based management systems

## Author
Jisan
