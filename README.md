# LaunchGuard

### Cross-functional product launch risk detection and what-if simulation

LaunchGuard is a lightweight decision-support prototype that detects hidden dependencies between teams before a product launch.

A product can appear "ready" when individual teams report high readiness, while dependencies between those teams create serious launch risks.

For example:

> Marketing is 95% ready, but only 31% of expected inventory is available.

Both teams may look healthy in their own dashboards, but together they create a launch risk.

LaunchGuard makes these cross-functional dependencies visible.

---

## 🚀 The Problem

Product launches involve multiple teams working together:

**Vendor / Product → Production → Inventory → Channel / Resellers → Marketing → Sales → Support**

Traditional team dashboards often measure each function independently.

This creates a blind spot:

- Marketing may be ready to launch
- Production may be operating normally
- Sales may be partially prepared
- Support may have limited capacity

Individually, these metrics may not look catastrophic.

But when the teams interact, their dependencies can create a launch failure.

LaunchGuard detects these conflicts before they become real-world problems.

---

## 💡 Our Solution

LaunchGuard combines cross-functional readiness metrics with dependency-based rules to identify launch risks.

Instead of asking:

> "Is each team ready?"

LaunchGuard asks:

> "Are the teams ready **for each other**?"

Each detected risk includes:

- What triggered the risk
- Why the dependency matters
- Severity
- Affected teams
- Recommended action

---

## ✨ Key Features

### 1. Cross-functional Risk Detection

LaunchGuard evaluates relationships between teams instead of isolated readiness scores.

Examples:

- Marketing readiness vs. inventory availability
- Marketing readiness vs. sales readiness
- Expected demand vs. support capacity
- Production capacity vs. expected demand
- Marketing readiness vs. channel readiness
- Quality readiness vs. launch timeline

---

### 2. Live What-If Simulator

Users can adjust launch metrics using interactive sliders.

For example:

**Increase inventory → inventory risk decreases**

**Increase expected demand → production/support risks may appear**

**Increase sales readiness → sales/support dependency risks may activate**

The risk analysis recalculates immediately as conditions change.

This allows decision-makers to explore:

> "What needs to change for this launch to become safer?"

---

### 3. Launch Risk Summary

The dashboard provides an immediate overview of the current launch condition.

It highlights:

- Critical risks
- High risks
- Medium risks
- Overall launch status

The summary updates dynamically when the underlying metrics change.

---

### 4. Product Lifecycle View

LaunchGuard visualises the dependency chain:

```text
Vendor / Product
       ↓
Production
       ↓
Inventory
       ↓
Channel / Resellers
       ↓
Marketing
       ↓
Sales
       ↓
Support
