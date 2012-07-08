check_procurve_loop
===================

Use SNMP to check if a HP ProCurve switch has activated loop protection.

Usage: check_procurve_loop -H <host> -C <snmp community name>

The script will report SUCCESS if no loop is found, followed by the number of ports checked, or CRITICAL in case of a loop with the affected ports specified.

Examples taken from a HP ProCurve 2510G-24.

No loop found:
OK - No loops detected (24 ports checked)

Loop found, ports 8 and 19 detected:
CRITICAL - found a loop on the following ports: 8 19 (24 ports checked) 

