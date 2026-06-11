# Case Study: Intermittent Wi-Fi Connectivity

## Problem

Users reported intermittent Wi-Fi disconnections affecting productivity throughout the workday.

## Environment

* Multi-AP wireless environment
* Cloud-managed access points
* Windows laptops and mobile devices
* Business environment with multiple users

## Investigation

### Step 1: Identify affected devices

Collected reports from users and determined that multiple devices were experiencing similar connectivity issues.

### Step 2: Validate client configuration

Reviewed wireless adapter settings and drivers on affected devices.

Result:

* No driver or client-side issues identified.

### Step 3: Test network connectivity

Performed connectivity testing between affected devices and network resources.

Tests included:

* Ping to default gateway
* Ping to access points
* Ping to other devices on the LAN
* DNS resolution testing

Result:

* Connectivity failures appeared intermittent and inconsistent.

### Step 4: Review wireless infrastructure

Checked access point status, controller health, and signal strength metrics.

Result:

* Signal levels appeared normal.
* One access point was suspected to have an underlying connectivity issue.

### Step 5: Validate physical connectivity

To isolate the issue, the access point was temporarily connected using a new Ethernet cable rather than the existing wall cabling.

Result:

* Wireless stability improved significantly.

## Root Cause

The issue was traced to suspected degradation within the existing network path servicing the access point, likely involving the permanent cabling infrastructure.

## Resolution

A temporary Ethernet cable was deployed to bypass the suspected network path while the environment continued to be monitored.

## Lessons Learned

Wi-Fi issues are not always caused by wireless configuration problems.

When troubleshooting connectivity issues:

* Validate client devices first
* Test DNS and network connectivity independently
* Verify access point health
* Consider physical infrastructure as a potential root cause
* Use temporary bypasses to isolate faults before making permanent changes
