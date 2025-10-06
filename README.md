# Integrating Different School Systems into a Unified School Management Application

You are developing a school management application that helps administrators manage various school systems such as attendance, grading, and library management. Each system has different interfaces and methods. To ensure compatibility and seamless integration, you need to create adapters for different systems to allow them to connect to the unified school management application.

## Adaptee Objects

- **AttendanceSystem**  
  Represents an attendance tracking system that needs to be integrated.  
  Method: `markAttendance()`

- **GradingSystem**  
  Represents a grading system that requires integration.  
  Method: `recordGrades()`

- **LibrarySystem**  
  Represents a library management system that needs to be integrated.  
  Method: `manageBooks()`

## Target Object

- **SchoolManagementApp**  
  Represents a unified school management application with a common interface for integrating systems.  
  Method: `integrateSystem()`

## Adapter Objects

- **AttendanceSystemAdapter**  
  An adapter for integrating the attendance system into the school management application.  
  Adapts `AttendanceSystem` to the `SchoolManagementApp` interface, translating `integrateSystem()` to `markAttendance()`.

- **GradingSystemAdapter**  
  An adapter for integrating the grading system into the school management application.  
  Adapts `GradingSystem` to the `SchoolManagementApp` interface, translating `integrateSystem()` to `recordGrades()`.

- **LibrarySystemAdapter**  
  An adapter for integrating the library management system into the school management application.  
  Adapts `LibrarySystem` to the `SchoolManagementApp` interface, translating `integrateSystem()` to `manageBooks()`.