---
title: "Keywords"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/logical.html"
last_updated: "8/7/2025"
product_version: "13.0.1.6168"
---

# Keywords


The logical operator CASE represents an if-else statement. It is used to evaluate a certain condition and execute an expression if this condition is true. If the condition is false, another expression is executed.

The CASE operator has the following syntax:

|  |
| --- |
| CASE  WHEN "Value" = "1" THEN "Expression 1"  ELSE "Expression 2"  END |

Here:

* WHEN statement represents a condition that must be evaluated.
* THEN statement specifies a group to which an object must be placed if the condition is true.
* ELSE specifies a group to which an object must be placed if the condition is false.

You can include multiple WHEN statements to evaluate multiple conditions:

|  |
| --- |
| CASE  WHEN "Value" = "1" THEN "Expression 1"  WHEN "Value" = "2" THEN "Expression 2"  WHEN "Value" = "3" THEN "Expression 3"  ELSE "Expression 4"  END |

Limitations

You cannot nest one CASE expression within another CASE expression. However, you can include methods to define values in a CASE statement.

Example

Business View includes a number of predefined categories that use CASE grouping expressions. You can use these predefined categories to understand how the CASE operator works.

For example, the VMs with Snapshot category uses the following grouping expression.

|  |
| --- |
| CASE  WHEN HasSnapshots = "No" THEN "No snapshots"  WHEN SnapshotCreateTime < DateAdd(Today, -30, "d") THEN "Older than 30 days"  WHEN SnapshotCreateTime < DateAdd(Today, -7, "d") THEN "Older than 7 days"  WHEN SnapshotCreateTime < DateAdd(Today, -1, "d") THEN "Older than 1 day"  ELSE "Recent snapshots"  END |

Here:

* The first WHEN statement checks whether a VM has any snapshots. If a VM has no snapshots, this VM is included in the No snapshots group.

* The second, third and fourth WHEN statements check VM snapshot age. If the age more than 30 days, a VM in included in the Older than 30 days group. If the age more than 7 days, a VM in included in the Older than 7 days group. If the age more than 1 day, a VM in included in the Older than 1 day group.
* The ELSE statement includes in the Recent snapshots group all VMs with snapshots not older than 1 day.


