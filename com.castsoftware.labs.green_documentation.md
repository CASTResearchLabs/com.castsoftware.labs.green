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

* GreenIT - focus on "pipe leaks"
* GreenIT - focus on "pipe ruptures"

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

* GreenIT - focus on "pipe leaks"
* GreenIT - focus on "pipe ruptures"

## Business Criteria

List of new Business Criteria

* GreenIT index

# Limitations

N\/A

# Appendix

## Selected Quality Rules


