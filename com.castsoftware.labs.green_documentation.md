# _com.castsoftware.labs.green_ Description

This extension provides computation of the following new assessment indicator\(s\)

* the _GreenIT index_
* supporting Technical Criteria

## Problem Statement

More and more software and websites are so "obese" they create performance issues and increase costs for companies. Scalability becomes a real challenge to continue to operate them. Some applications require inordinate amounts of computing resources - memory, CPU, cycles, storage space, bandwith, etc to operate.

Most of efforts to fight against these issues are focused on hardware. More and more servers or new servers optimized. More and more CPUs, virtualization is also a start of solution but not totally well managed for now.

One of the ideas is to think differently. Rather than being reactive and to stack workaround about a situation that is really difficult to maintain, why not focus on software design in a continuous approach.

Energy can be saved by making Software more efficient

## Research Labs proposal

To identify pieces of Software that could be optimized to withstand unexpected workload, increased "scrutiny" from hackers, "seamless" evolution of execution environment, the Research Labs offer a solution based on CAST AIP Assessment Model.

* The _GreenIT Index_ is a Business Criterion that aggregates Quality Rules from existing high-impact Efficiency-related Technical Criteria
* as well as from most-severe Robustness-related Technical Criteria to account for wasted resources when application functioning has been compromised and require a restart\/recovery
* grouped into new dedicated Technical Criteria

The Research Labs released this first version of the GreenIT Index to leverage the expertise and experience of customers in order to fine-tune its exact composition and collect feedback.

## Formula

The GreenIT Index is based on the following Technical Criteria

* GreenIT - focus on "pipe leaks" - data access efficiency
* GreenIT - focus on "pipe leaks" - algorithmic costs
* GreenIT - focus on "pipe leaks" - resource economy
* GreenIT - focus on pipe ruptures - avoiding failure

The Technical Criteria have been populated with Quality Rules with aggregate weight greater or equal to 5 of the following existing Technical Criteria:

* Efficiency - Expensive Calls in Loops
* Efficiency - Memory, Network and Disk Space Management
* Efficiency - SQL and Data Handling Performance
* Complexity - Dynamic Instantiation
* Complexity - SQL Queries
* Programming Practices - Error and Exception Handling
* Programming Practices - Unexpected Behavior
* Secure Coding - Time and State

Please refer to the appendix for the explicit list of Quality Rules.

# In what situation should you install this extension?

If you are interested in getting a preview of what the GreenIT index would be and are willing to share the results to help the CAST Research Labs validate them.

# Release notes

## 2.0.0

Release 2.0.0 changes the organization and composition of the index, via dedicated Technical Criteria, to better map the type of issues at hand, and refine selection.

# _com.castsoftware.labs.green_ technology support

All technologies supported out-of-the-box by CAST AIP are supported.
In case of technologies supported by some AIP extensions, contact the Research Labs to build a compatible GreenIT index.

# Function Point, Quality and Sizing support

This extension is designed to bring new quality indicator aside existing ones.

# CAST AIP compatibility

This extension is compatible with:

* 8.1.x out-of-the-box \(AIP release used for the tests\)
* 8.0.x after changing the nuspec file \(there is no reason the extension would not work but it was not tested\)
* 7.x.x after changing the nuspec file \(there is no reason the extension would not work but it was not tested\)

# Supported DBMS servers

This extension is currently supported on CAST databases installed on any supported RDBMS.

# Prerequisites

* An installation of any compatible release of CAST AIP \(see table above\)

# Bug Fix List

N\/A

# Download and installation instructions

Please see:  [Extension Link Installation](http://doc.castsoftware.com/display/DOCEXT/Extension+download+and+installation)

The installation steps are the following:

* download the extension through the CAST Extension Downloader using the https://extend.castsoftware.com:443/labs download server
* open Server Manager 8.1+
* select the existing set of databases to update \/ install a new set of databases
* manage extensions of the existing set of database \/ follow the installation wizard up to the manage extension pane
* select _com.castsoftware.labs.green.2.0.0_
* run the update \/ the installation  
* open CAST Management Studio
* import the Assessment Model from the Dashboard Service processed in steps \#3 to \#6 above; this is a _Mandatory_ step to start computing the new indicator, one MUST import and use the Assessment Model from the Dashboard that was updated with the extension

# Packaging, delivering and analyzing your source code

Packaging, delivering and analyzing your source code is performed the same way as usual.

To get results:

* run a new snapshot \(if not possible, contact the Research Labs for alternative procedure\)

# What results can you expect?

## Objects

N\/A

## Links

N\/A

## Quality rules

N\/A

## Technical Criteria

List of new Technical Criteria

* GreenIT - focus on "pipe leaks" - data access efficiency
* GreenIT - focus on "pipe leaks" - algorithmic costs
* GreenIT - focus on "pipe leaks" - resource economy
* GreenIT - focus on pipe ruptures - avoiding failure

## Business Criteria

List of new Business Criteria

* GreenIT index

# Limitations

N\/A

# Appendix

## Selected Quality Rules

GreenIT - focus on pipe leaks - data access efficiency
* 1116 Avoid Functions with a complex SELECT clause (C Lang.)
* 7660 Never use SQL queries with a cartesian product on XXL Tables
* 6612 Avoid Functions/Procedures with a complex SELECT clause (DB2 Server)
* 5132 Avoid Programs with a Complex SELECT Clause (Cobol)
* 7904 Avoid SQL queries on XXL tables that no index can support
* 7656 Avoid SQL queries on XXL Tables that no index can support (AllTechno)
* 4092 Avoid using Cursors (SQL Server)
* 5060 Avoid using MERGE
* 7866 Avoid SELECT ... BYPASSING BUFFER
* 7810 Avoid Artifacts with a Complex SELECT Clause
* 660 Avoid Functions/Methods with SQL statement including Subqueries (C++)
* 658 Avoid Functions/Methods with SQL statement using Group By clause (C++)
* 662 Avoid Functions/Methods with a complex SELECT clause (C++)
* 656 Avoid Functions/Methods with queries on too many Tables (C++)
* 664 Avoid Functions/Methods with High RAW SQL Complexity (C++)
* 680 Avoid Dynamic SQL Objects With Queries on more than 4 Tables (C++)
* 1108 Avoid Functions with queries on too many Tables (C Lang.)
* 1110 Avoid Functions with SQL statement including Subqueries (C Lang.)
* 1112 Avoid Functions with SQL statement using Group By clause (C Lang.)
* 1114 Avoid Functions with High RAW SQL Complexity (C Lang.)
* 1126 Avoid Dynamic SQL Objects With Queries on more than 4 Tables (C Lang.)
* 1580 Avoid using execute immediate
* 1598 Avoid Rule HINT  /*+ rule */ or --+ rule in PL/SQL code
* 1578 Avoid using LONG & LONG RAW datatype for Table Columns
* 1644 Avoid Functions/Procedures/Triggers with a complex SELECT clause (PL/SQL Oracle)
* 1646 Avoid Functions/Procedures with SQL statement using Group By clause (PL/SQL Oracle)
* 1642 Avoid Functions/Procedures with queries on too many Tables (PL/SQL Oracle)
* 1648 Avoid Functions/Procedures with SQL statement including Subqueries (PL/SQL Oracle)
* 1650 Avoid PL/SQL Artifacts with High RAW SQL Complexity (PL/SQL Oracle)
* 4052 Avoid tables not involved in a Foreign Key (SQL Server)
* 4084 Avoid nested Stored Procedures using temporary Tables
* 4138 Avoid Functions/Procedures with queries on too many Tables (SQL Server)
* 4144 Avoid Functions/Procedures with SQL statement using Group By clause (SQL Server)
* 4142 Avoid Functions/Procedures with High RAW SQL Complexity (SQL Server)
* 4140 Avoid Functions/Procedures with a complex SELECT clause (SQL Server)
* 4146 Avoid Functions/Procedures with SQL statement including Subqueries (SQL Server)
* 4772 Avoid SQL Artifacts with SQL statement including Subqueries (JEE)
* 4770 Avoid SQL Artifacts with queries on too many Tables (JEE)
* 4774 Avoid SQL Artifacts with High RAW SQL Complexity (JEE)
* 4778 Avoid SQL Artifacts with SQL statement using Group By clause (JEE)
* 4776 Avoid Artifacts with a complex SELECT clause (JEE)
* 5058 Avoid using SORT
* 4794 Avoid Dynamic SQL Objects With Queries on more than 4 Tables (JEE)
* 5056 Avoid using SEARCH without the ALL addition
* 5124 Avoid Programs With Queries on more than 4 Tables (Cobol)
* 5126 Avoid Programs with High RAW SQL Complexity (Cobol)
* 5130 Avoid Programs with Group By (Cobol)
* 5128 Avoid Programs with subqueries (Cobol)
* 5552 Avoid using queries with too many Tables in record groups (Forms)
* 5554 Avoid having SQL code in Triggers named pre-record
* 6176 Avoid Artifacts With Queries on more than 4 Tables (PowerBuilder)
* 6180 Avoid Artifacts with High RAW SQL Complexity (PowerBuilder)
* 6178 Avoid Artifacts with a Complex SELECT Clause (PowerBuilder)
* 6182 Avoid Artifacts with Group By (PowerBuilder)
* 6184 Avoid Artifacts with Subqueries
* 6196 Avoid Dynamic SQL Objects With Queries on more than 4 Tables (PowerBuilder)
* 6580 Avoid using Cursors (DB2 Server)
* 6576 Avoid tables not involved in a Foreign Key (DB2 Server)
* 6608 Avoid Functions/Procedures with queries on too many Tables (DB2 Server)
* 6610 Avoid Functions/Procedures with SQL statement using Group By clause (DB2 Server)
* 6614 Avoid Functions/Procedures with SQL statement including Subqueries (DB2 Server)
* 6616 Avoid Functions/Procedures with High RAW SQL Complexity (DB2 Server)
* 7102 Avoid Artifacts With Queries on more than 4 Tables (ABAP)
* 7104 Avoid Artifacts with Subqueries (ABAP)
* 7106 Avoid Artifacts with Group By (ABAP)
* 7108 Avoid Artifacts with a Complex SELECT Clause (ABAP)
* 7110 Avoid Artifacts with High RAW SQL Complexity (ABAP)
* 7130 Avoid Artifacts with High Depth of Nested Subqueries
* 7226 Avoid Artifacts with Group By (Visual Basic)
* 7230 Avoid Artifacts With Queries on more than 4 Tables (Visual Basic)
* 7658 Avoid SQL queries on XXL Tables using Functions on indexed Columns in the WHERE clause
* 7228 Avoid Artifacts with Subqueries
* 7232 Avoid Dynamic SQL Objects With Queries on more than 4 Tables (Visual Basic)
* 7350 Avoid Tables having Indexes with a too large Index definition
* 7366 File descriptor block must be defined with 0 record
* 7344 Avoid SELECT * queries
* 7346 Avoid redundant indexes
* 7348 Avoid too many Indexes on one Table
* 7358 Avoid call to AcceptChanges in a loop
* 7386 Avoid Tables without a clustered Index
* 7420 Avoid SQL queries with implicit conversions in the WHERE clause
* 7422 Avoid SQL queries that no index can support (AllTechno)
* 7418 Avoid SQL queries using functions on indexed columns in the WHERE clause
* 7426 Never use SQL queries with a cartesian product (AllTechno)
* 7428 Avoid SQL queries not using the first column of a composite index in the WHERE clause
* 7436 Prefer UNION ALL to UNION
* 7476 Turn off Multiple SQL statements for each measure
* 7482 Do not use Cartesian products in Universe properties
* 7480 Use aggregate awareness for indicators
* 7498 Collection must be the same between getter and setter
* 7488 Use lazy fetching for collection
* 7500 Use table-per-class-hierarchy when subclasses have few properties
* 7490 Avoid UPDATE trigger firing when not necessary
* 7502 Never use array to map a collection
* 7496 Use table-per-subclass strategy when subclasses have many properties
* 7538 Avoid using SELECT ... INTO CORRESPONDING FIELDS OF
* 7544 Avoid using SELECT ... ENDSELECT statement
* 7530 Avoid SELECT * or SELECT SINGLE * queries
* 7542 Avoid using FOR ALL ENTRIES IN without emptiness check
* 7534 Avoid READ TABLE without BINARY SEARCH
* 7592 Avoid using ORDER BY in SELECTS
* 7594 Avoid using SELECT DISTINCT, use DELETE-ADJACENT
* 7634 Avoid select-before-update when the Table is not associated to an UPDATE Trigger
* 7644 Avoid executing multiple OPEN statements
* 7642 Avoid SQL queries on XXL tables not using the first column of a composite index in the WHERE clause
* 7664 Avoid using FOR ALL ENTRIES IN without emptiness check on XXL Tables
* 7666 Avoid using SELECT ... ENDSELECT statement on XXL Tables
* 7662 Avoid SQL queries on XXL Tables with implicit conversions in the WHERE clause
* 7692 Each opened file must be closed
* 7702 Use a third party connection pool
* 7738 Never use SQL queries with a cartesian product (ABAP)
* 7736 Avoid SQL queries that no index can support (ABAP)
* 7744 Avoid SQL queries on XXL tables that no index can support (ABAP)
* 7806 Avoid Artifacts with Group By
* 7808 Avoid Artifacts with SQL statement including subqueries
* 7822 Avoid Artifacts with queries on more than 4 Tables
* 7828 Avoid Artifacts with High RAW SQL Complexity
* 7820 Never use SQL queries with a cartesian product
* 7876 Avoid using SELECT ... FOR UPDATE
* 7870 Avoid using the NOT LIKE operator in WHERE clauses
* 7872 Avoid using IS [NOT] NULL in WHERE condition
* 7902 Avoid SQL queries that no index can support
* 7878 Avoid Open SQL SELECT queries without WHERE condition
* 7896 Avoid using Cursors
* 8082 Avoid Tables without Primary Key
* 8080 Avoid exists independent clauses
* 8110 Use dedicated stored procedures when multiple data accesses are needed (ASCPEM-PRF-10)


GreenIT - focus on pipe leaks - algorithmic costs
* 2586 Utilization of DoEvents inside a loop
* 7198 Avoid String concatenation in loops
* 7200 Avoid String concatenation in loops
* 7204 Avoid method invocation in a loop termination expression
* 7210 Avoid instantiations inside loops
* 7212 Avoid instantiations inside loops
* 7218 Avoid OPEN/CLOSE inside loops
* 7352 Avoid calling properties that clone values in loops
* 7424 Avoid using SQL queries inside a loop
* 7430 Avoid Cursors inside a loop (PL/SQL Oracle)
* 7432 Avoid Cursors inside a  loop (SQL Server)
* 7470 Avoid doing select on Datatable in loop
* 7532 Avoid nested SELECT ... ENDSELECT statements
* 7790 Avoid Cursors inside a loop
* 7868 Avoid Open SQL queries in loops
* 7880 Avoid nested loops
* 7894 Avoid using LOOP INTO, use LOOP ASSIGNING instead
* 7954 Avoid indirect String concatenation inside loops
* 7962 Avoid direct or indirect remote calls inside a loop


GreenIT - focus on pipe leaks - resource economy
* 1072 Avoid using memory management Functions (free/malloc/realloc)
* 1074 Avoid using signals management Functions
* 3612 Close SQL connection ASAP
* 4694 Avoid using 'System.gc'
* 4744 EJB Entity access through their local Interface
* 4746 EJB Session access through their local Interface
* 7194 Avoid large number of String concatenation
* 7196 Avoid large number of String concatenation
* 7250 Avoid String initialization with String object (created using the 'new' keyword)
* 7254 Declare as Static all methods not using instance members
* 7270 Declare as Static all methods not using instance members
* 7638 Avoid using DriverManager
* 7720 Avoid too many EJB bean
* 7936 Avoid using finalize()
* 7940 Avoid Stateful Beans not removed
* 8048 Invoke 'delete' with the same form as the matching 'new'
* 8068 Do not return a dereferenced pointer allocated inside the function
* 8100 Blocking synchronous calls should have associated timeouts
* 8104 Close database resources ASAP
* 8108 Close the outermost stream ASAP


GreenIT - focus on pipe ruptures - avoiding failure
* 592 Ensure you provide a user-defined copy constructor or disable copy when a class allocates memory in its constructor
* 678 Never throw an exception from a Destructor
* 1588 Use WHEN OTHERS in exception management
* 2232 Pages should use error handling page
* 2564 Use a single Error Handling Method
* 2590 Avoid using On error Resume Next in the Class event terminate
* 3062 Use of error handling page
* 4064 Avoid Procedures using an Insert, Update, Delete, Create Table or Select without including error management
* 4066 Avoid Stored Procedures not returning a status value
* 4070 Avoid use of truncate table
* 4612 Avoid using native Methods (JNI)
* 4620 Avoid empty catch blocks (JEE)
* 4622 Avoid empty finally blocks (JEE)
* 4624 Avoid return statements in finally blocks (JEE)
* 4626 Avoid missing default in switch statements (JEE)
* 4652 Avoid direct Class inheritance from java.lang.Throwable
* 4654 Avoid throwing an exception of type Exception (JEE)
* 4656 Avoid declaring throwing an exception and not throwing it
* 4658 Avoid catching an exception of type Exception, RuntimeException, or Throwable (JEE)
* 4696 Avoid using 'System.err' and 'System.out' within a try catch block
* 4698 Avoid using 'System.err' and 'System.out' outside a try catch block
* 4700 Avoid using 'Throwable.printStackTrace()' within a try catch block
* 4702 Avoid using 'Throwable.printStackTrace()' outside a try catch block
* 5050 Avoid using HANDLE CONDITION
* 5052 Avoid using IGNORE CONDITION
* 5054 Avoid using HANDLE ABEND
* 5092 Include a WHEN OTHER clause when using EVALUATE
* 7152 Avoid Fields in Servlet Classes that are not final static
* 7154 Avoid Fields in Action Classes that are not final static
* 7202 Check usage of '==' and '!=' on objects
* 7354 Avoid catching an exception of type Exception (C# .Net)
* 7356 Avoid throwing an exception of type Exception (C# .Net)
* 7374 Avoid empty finally blocks (C#, VB.NET)
* 7376 Avoid empty catch blocks (C#, VB.NET)
* 7438 Avoid non thread safe singleton
* 7442 Avoid to use this within Constructor in multi-thread environment
* 7446 Avoid double checked locking
* 7494 Persistent class method's equals() and hashCode() must access its fields through getter methods
* 7504 Persistent classes should Implement hashCode() and equals()
* 7506 Define equals() and hashCode() for component
* 7508 Collection-typed attributes getter must be defined with the correct interface
* 7518 Avoid missing WHEN OTHERS in CASE statements
* 7520 Avoid unchecked return code (SY-SUBRC) after OPEN SQL or READ statement
* 7528 Never use the ON CHANGE OF statement
* 7536 Avoid using AT Events in combination of LOOP AT .... WHERE constructs
* 7548 Never use incompatible statements with the CICS environment
* 7556 Avoid instanceof in Methods that override or implement Object.equals(), Comparable.compareTo()
* 7586 Avoid cyclic calls between Event and its handled Method
* 7636 Use version instead of timestamp
* 7640 Avoid catch blocks with assertion
* 7650 All types of a serializable Class must be serializable
* 7652 Avoid throwing an exception in a catch block without chaining it
* 7674 Avoid empty CATCH blocks (ABAP)
* 7688 Never truncate data in MOVE statements
* 7690 Avoid unchecked return code (SQLCODE) after EXEC SQL query
* 7698 Files should be declared with a FILE-STATUS
* 7708 Avoid using session.setFlushMode(FlushMode.COMMIT, FlushMode.NEVER or FlushMode.MANUAL)
* 7710 Avoid non serializable Entities
* 7712 Avoid public/protected setter for the generated identifier field
* 7722 Avoid using references to the id in the persistent class's method equals()
* 7724 Overriden equals() Methods in persistent Subclasses should only reference properties from the persistent base Class
* 7728 Avoid thread creation for application running on application server
* 7730 Use declarative transaction
* 7756 Avoid using READ statement without AT END clause
* 7782 Avoid empty finally blocks
* 7788 Avoid empty catch blocks
* 7824 The exception Exception should never been thrown. Always Subclass Exception and throw the subclassed Classes.
* 7850 Avoid raising an exception in a Web Dynpro Supply Function or in a Method called by a Supply Function
* 7862 Avoid catching an exception of type Exception, RuntimeException, or Throwable
* 7864 BAPIs must not cause the Program to abort or terminate
* 7884 Avoid disabling source code inspection
* 7888 Web Dynpro - Never use direct calls to routine via me->, use wd_This-> instead
* 7890 Web Dynpro - Never use INCLUDE statement
* 7892 Web Dynpro - Avoid changing the program flow
* 7910 Never exit a finally block with a return, break, continue, or throw
* 7942 Avoid EJBs using 'synchronized' qualifier, 'wait', 'notify' and 'notifyAll' Methods
* 7964 Avoid directly instantiating a Class used as a managed bean
* 7998 Avoid local variables that are not initialized at declaration time
* 8000 Avoid 'catch-all' statement
* 8002 Never perform C-style cast between incompatible Class pointers
* 8004 Avoid using 'delete this'
* 8006 Avoid Classes with a copy Constructor and the default Destructor or assignment operator
* 8010 Do not overload the ampersand, comma, logical AND or logical OR operators
* 8012 Avoid unchecked return code (SY-SUBRC) after opening and reading dataset
* 8014 Avoid unchecked return code (SY-SUBRC) after AUTHORITY-CHECK
* 8024 Avoid Classes with a non-empty Destructor and the default assignment operator or copy Constructor
* 8026 Avoid Classes with an assignment operator and the default Destructor or copy constructor
* 8028 Avoid missing default in switch statements
* 8030 Check alphanumeric data before moving it into numeric data
* 8034 Variables defined in Working-Storage section must be initialized before to be read
* 8052 Avoid setting a pointer to the address of a local variable defined in a lower scope
* 8054 Avoid calling blocking functions with an infinite timeout
* 8056 Method override fails due to mismatch of const/volatile qualifiers
* 8064 Assignment operator should assign all non-static members of the target object
* 8072 Never define collection of 'std::auto_ptr'
* 8074 Avoid using 'class' or 'struct' parameters with variadic Functions
* 8090 Avoid using NaN to test the result of an expression
* 8094 Avoid locking of Objects with weak identities
* 8096 Avoid testing floating point numbers for equality
* 8106 Avoid empty IF-ENDIF blocks
* 8112 Avoid improper processing of the execution status of data handling operations
* 8114 Avoid numerical data corruption during incompatible mutation

