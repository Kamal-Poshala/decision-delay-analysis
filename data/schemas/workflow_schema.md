# Workflow Log Schema

This document defines the schema for synthetic human approval workflow logs
used in the Decision Delay Analysis project.

## Overview

Each record represents a single approval request progressing through
a sequence of human decision-makers.

## Fields

- request_id  
  Unique identifier for each approval request.

- submitted_at  
  Timestamp when the request was initially submitted.

- request_type  
  Category of the request (e.g., internship, funding, access).

- priority_level  
  Encoded urgency of the request (low, medium, high).

- num_approvers  
  Total number of required approvers.

- approver_sequence  
  Ordered list of approver roles involved in the workflow.

- decision_times_per_stage  
  Time taken by each approver to act on the request.

- num_reminders_sent  
  Number of automated reminders triggered during processing.

- escalated  
  Boolean indicating whether escalation occurred.

- final_outcome  
  Approved / rejected / expired.

- total_resolution_time  
  End-to-end time from submission to final decision.
