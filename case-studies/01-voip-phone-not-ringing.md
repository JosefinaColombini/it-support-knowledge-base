# Case Study: VoIP Phone Not Receiving Calls

## Problem

A newly deployed cordless VoIP phone could successfully place outbound calls but was not receiving inbound calls.

## Environment

* RingCentral
* Shared call queue
* SIP-based cordless phone
* Multi-device phone environment

## Investigation

### Step 1: Verify device registration

Confirmed the phone could place outbound calls.

Result:

* SIP registration appeared healthy.

### Step 2: Test direct extension dialing

Called the extension directly.

Result:

* Calls routed directly to voicemail.

### Step 3: Review call routing configuration

Verified call queue membership and call handling rules.

Result:

* User was not assigned to the active call queue.

## Root Cause

The phone was correctly registered but was not included in the inbound call routing configuration.

## Resolution

Added the user to the appropriate call queue and validated inbound call delivery.

## Lessons Learned

When troubleshooting VoIP devices, verify:

* SIP registration
* Extension assignment
* Call queue membership
* Call handling rules

before replacing hardware.
