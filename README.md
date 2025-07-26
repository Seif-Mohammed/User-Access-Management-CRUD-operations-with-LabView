# User-Access-Management-CRUD-operations-with-LabView
A complete user management system built in LabVIEW with SQLite database integration, featuring role-based access control and encrypted password storage.

# LabVIEW User Access Management System

A complete user management system built in LabVIEW with SQLite database integration, featuring role-based access control and encrypted password storage.

## Features

- **Multi-page GUI**: Login, Main Menu, Add/Delete/Query/Edit User pages
- **SQLite Database**: Secure user credential storage
- **Password Encryption**: MD5 hashing for password security
- **Role-based Access**: Admin vs Normal user permissions
- **Input Validation**: Age verification, duplicate username prevention
- **Industrial GUI**: Clean interface with hidden LabVIEW menus

## User Data Structure

- Username (unique)
- Password (encrypted)
- Title
- Email
- User Level (Admin/Normal)
- Birthdate

## System Requirements

- LabVIEW 2020 or later
- SQLite LabVIEW Toolkit
- Windows OS

## File Structure

```
├── src/
│   ├── Main.vi                 # Main application entry point
│   ├── Userdata.ctl               # User data

├── data/
│   └── users.db              # SQLite database file
├── Executable file/
│   └── UserManagement.exe    # Compiled executable
└── README.md
```


```

## Key Implementation Features

- **State Machine Architecture**: Each page implemented as separate state
- **Error Handling**: Comprehensive validation with user-friendly messages
- **UI/UX**: Role-based menu visibility, form reset mechanisms
- **Age Validation**: Automatic 18+ age verification from birthdate

## Installation & Usage

1. Install LabVIEW SQLite Toolkit
2. Run `DatabaseInit.vi` to create initial database
3. Build executable or run `Main.vi`
4. Default admin login: admin/admin (change after first login)

## Access Levels

- **Admin**: Full CRUD operations on all users
- **Normal User**: Can only add new users and query existing users

## Security Features

- Encrypted password storage
- Session management with logout functionality
- Input sanitization
- Duplicate username prevention
- Age verification (18+ required)

---

*Built for LabVIEW Course Exam - Industrial User Management System*
