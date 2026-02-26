Product Design Approach
Caribbean HRMS (Human Resource Management System)
1. Product Framing & Alignment (Before Any Screens)
Objective

Establish a shared understanding of the product’s purpose, operational value, and scope before interface design begins.

This system is not simply an HR record-keeping platform.
It is an operational decision-support tool that prevents administrative errors, compliance risks, and organizational downtime.

The product must support real-time administrative decision making across mobile, desktop, and WhatsApp interfaces.

Activities

Define Core Users

CEO/Admin (non-technical decision maker)

Supervisor/Manager (approver)

Employee (mobile-first, WhatsApp-first)

Payroll Officer (compliance-driven operator)

Define Core Problems

Manual leave tracking causes operational conflicts

Payroll compliance risk and calculation errors

Attendance data exists but is unusable

Employees lack visibility into entitlements

Administrators must make decisions without complete information

Define Non-Goals (v1)

Advanced analytics dashboards

Enterprise HR planning tools

Recruitment management

Performance prediction AI

Define Success Metrics

Leave request completed in < 60 seconds

Approval via WhatsApp in < 30 seconds

Payroll run completed in < 30 minutes

First-time admin setup without training

(These are usability targets defined for the system 

HR Solution

)

Deliverables

Product problem statement

User role definitions

MVP scope definition

Measurable usability success metrics

Why This Matters

Prevents:

Misaligned expectations

Feature creep

Building a generic HR tool instead of an operational system

2. Role-Based Journey Mapping (Foundation Layer)
Objective

Design workflows based on real human behavior across roles and approvals before designing screens.

Activities

For each role, map:

Entry points

Mobile app

Desktop dashboard

WhatsApp bot

Primary journeys
Admin → Setup → Add employees → Monitor → Approve → Payroll
Employee → Check balance → Request leave → Track status
Supervisor → Review → Decide → Notify
Payroll → Validate → Calculate → Publish

Identify Decision Moments

Leave conflict detection

Signing officer availability

Payroll exceptions

Attendance alerts

Identify Failure Points

Internet connectivity loss

Missing documents

Policy violations

Conflicting approvals

Map Emotional States

Admin anxiety (operational risk)

Employee uncertainty (leave balance)

Payroll fear (penalties)

Supervisor urgency (quick approvals)

Deliverables

4 role-based journey maps

Cross-role dependency map

Approval chain visualization

Why This Matters

Administrative software fails when handoffs between humans are unclear.

The HRMS relies heavily on approvals and notifications; therefore interactions between users are more important than individual screens.

3. Information Architecture & Screen Strategy
Objective

Convert real workflows into a scalable system structure across mobile and desktop.

Activities

Define Platforms

Mobile app (primary interface)

Desktop dashboard (management interface)

WhatsApp (approval interface)

The system must support approvals and notifications through WhatsApp 

HR Solution

.

Define Navigation Structure

Mobile navigation:

Home

Leave

Attendance

Payroll

More

Desktop navigation:

Dashboard

Employees

Approvals

Reports

Settings

Define Screen Categories
Core operational screens:

Leave management

Approval queue

Attendance monitoring

Payroll processing

Secondary screens:

Settings

Reports

Policy configuration

Deliverables

System sitemap (mobile + desktop)

Screen inventory with priority levels

Role-based navigation rules

Why This Matters

Prevents:

Deep confusing navigation

Duplicate features

Overloaded dashboards

4. Interaction Design & UX Logic
Objective

Define how the system behaves under every condition before visual design.

Activities

Specify:

Validation Rules

Leave balance checks

Notice period checks

Policy enforcement

Decision Logic

Conflict detection

Signing officer enforcement

Approval escalation

The system must warn when approval would leave insufficient signing officers 

HR Solution

.

State Transitions

Submitted

Pending approval

Approved

Denied

Escalated

Error Handling

Offline mode

Sync conflicts

Duplicate entries

Notification Logic

WhatsApp approvals

Reminders

Alerts

Deliverables

UX behavior documentation

State diagrams

Edge-case handling list

Why This Matters

Developers implement behavior exactly as specified.
If logic is unclear, the system becomes inconsistent and unreliable.

5. System Behavior & Event Modeling
Objective

Design the underlying operational system that connects people, policies, and events.

Activities

Model system entities:

Employee

Department

Leave policy

Attendance record

Payroll record

Approval

Model system events:

Leave request

Clock-in

Approval

Payroll run

Model automated decisions:

Conflict detection

Attendance alerts

Policy violations

The system queues actions offline and syncs later 

HR Solution

.

Deliverables

Entity relationship diagram

Event flow diagrams

Decision logic map

Why This Matters

Without modeling the system, UI flows will contradict business logic and require redesign during development.

6. UI Design System & Component Strategy
Objective

Create a consistent interface usable by non-technical administrators.

Activities

Define:

Color tokens

Typography scale

Spacing system

Accessible contrast

Design reusable components:

Form inputs

Approval cards

Status badges

Notifications

Calendars

The system must be readable outdoors and accessible 

HR Solution

.

Deliverables

Figma design system

Component library

Usage guidelines

Why This Matters

Prevents UI inconsistency and developer interpretation differences.

7. High-Fidelity Screen Design
Objective

Design production-ready screens only after system behavior is defined.

Priority Order

Onboarding & employee creation

Leave request & WhatsApp approval

Conflict detection

Attendance monitoring

Payroll run

KPI performance

Deliverables

High-fidelity UI

Mobile and desktop responsive designs

Interactive prototypes

Why This Matters

Ensures critical workflows are tested first, not secondary features.

8. Accessibility & Offline Support Pass
Objective

Ensure reliability across low connectivity and varying digital literacy.

Activities

Verify:

Offline usage

Sync behavior

Error messages

Screen reader support

Large text support

The system must function without internet and sync later 

HR Solution

.

Deliverables

Accessibility checklist

Offline behavior annotations

Why This Matters

The product targets environments with unstable connectivity.

9. Developer Handoff & Implementation Support
Objective

Make development predictable and reduce rework.

Activities

Provide:

Annotated Figma files

API expectations

State documentation

Edge case notes

Support:

Clarification sessions

Iteration reviews

Deliverables

Developer handoff documentation

Dev-ready prototypes

Open issues tracker

Why This Matters

Many software projects fail during handoff, not design.

10. Pre-Launch Validation
Objective

Identify operational risks before real users depend on the system.

Activities

Simulate:

Leave conflicts

Payroll run

Offline submission

Approval delays

Run usability tests:

Admin setup

Employee leave request

WhatsApp approval

Deliverables

Validation report

Final revision list

Launch readiness confirmation