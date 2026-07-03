---
title: "Operators"
product: "vone"
doc_type: "userguide"
source_url: "https://helpcenter.veeam.com/docs/one/userguide/operators.html"
last_updated: "6/24/2026"
product_version: "13.0.2.6723"
---

# Operators


To manipulate values in grouping expressions, you can use the following operators:

Operators

| Operator | Return Data Type | Description | Example |
| + | Text (string)  Numeric | Joins two string values to one string.  Adds two numeric values. | For a VM included in a replication job, expression "Replication Job: " + ReplicationJob retuns a string similar to Replication Job: Webserver Daily Replication.  Expression 2 + 2 returns 4. Expression 2.05 + 1 returns 3.05. |
| \* | Numeric | Multiplies numeric values. | Expression 2 \* 2 returns 4. Expression 100 \* 0.5 returns 50. |
| / | Numeric | Divides first numeric value into the second. | Expression 2 / 2 returns 1. Expression 100 / 50 returns 2. |
| - | Numeric | Subtracts the second numeric value from the first. | Expression 2 - 1 returns 1. Expression 100 - 0.5 returns 99.5. |
| < | Boolean | Less than.  Returns True if the value of left operand is less than the value of right operand. Otherwise, returns False. | For a VM, expression Memory < 2048 returns True if the amount of memory configured for a VM is less than 2048 MB. |
| <= | Boolean | Less than or equal to.  Returns True if the value of left operand is less than or equal to the value of right operand. Otherwise, returns False. | For a VM, expression Memory <= 2048 returns True if the amount of memory configured for a VM is less than or equal to 2048 MB. |
| > | Boolean | Greater than.  Returns True if the value of left operand is greater than the value of right operand. Otherwise, returns False. | For a VM, expression Memory > 2048 returns True if the amount of memory configured for a VM is greater than 2048 MB. |
| >= | Boolean | Greater than or equal to.  Returns True if the value of left operand is greater than or equal to the value of right operand. Otherwise, returns False. | For a VM, expression Memory >= 2048 returns True if the amount of memory configured for a VM is greater than or equal to 2048 MB. |
| = | Boolean | Equal.  Returns True if the value of left operand is the same as the value of right operand. Otherwise, returns False. | For a VM, expression Memory = 2048 returns True if the amount of memory configured for a VM is equal to 2048 MB.  For a VM, expression Name = "vdi001" returns True if the VM name is vdi001. |
| <> | Boolean | Not equal.  Returns True if the value of left operand is not the same as the value of right operand. Otherwise, returns False. | For a VM, expression Memory <> 2048 returns True if the amount of memory configured for a VM is less or greater than 2048 MB.  For a VM, expression Tag(department) <> "support" returns True if a tag of the department category assigned to a VM is other than support. |
| and | Text (string) | Joins conditions with a logical AND operator. | For a VM, expression Memory = 2048 and Name = "vdi001" returns True if the amount of memory configured for a VM is equal to 2048 MB and the VM name is vdi001. |
| or | Text (string) | Joins conditions with a logical OR operator. | For a VM, expression Memory = 2048 or Name = "vdi001" returns True if the amount of memory configured for a VM is equal to 2048 MB or the VM name is vdi001. |


