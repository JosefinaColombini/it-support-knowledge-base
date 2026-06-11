# Procedure: Server Health Checks

## Purpose

Maintain operational continuity by proactively identifying issues before they affect users or business services.

## Scope

Routine health checks performed on Windows servers and supporting infrastructure services.

## Verification Process

### 1. Backup Verification

Review backup status and confirm successful completion of recent backup jobs.

Checks:

* Last successful backup date
* Failed backup jobs
* Recovery point availability

### 2. Disk Space Review

Inspect storage utilization on critical volumes.

Checks:

* System drive free space
* Data volume free space
* Unusual storage growth

### 3. Event Viewer Review

Review Windows Event Viewer for critical or recurring errors.

Checks:

* System events
* Application events
* Service-related warnings
* Hardware-related alerts

### 4. Critical Services Validation

Verify that essential services are running normally.

Examples:

* Backup services
* Database services
* Application services
* Remote access services

### 5. Infrastructure Validation

Confirm supporting infrastructure is functioning correctly.

Checks:

* Internet connectivity
* Network availability
* DNS resolution

### 6. Documentation

Record findings and identify any required follow-up actions.

Examples:

* Create tickets for unresolved issues
* Document recurring warnings
* Escalate critical findings when necessary

## Outcome

Regular server health checks help identify potential issues early, improve service reliability, and reduce unplanned downtime.
