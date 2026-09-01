# Worked Examples

These examples are original and fictional. They demonstrate information hierarchy, not a required voice or word count.

## Example 1: Project status

### Source draft

> We wanted to provide an update on the Atlas migration. The team has continued to make progress and held several productive meetings with the infrastructure group this week. We have completed 78% of account migrations, but the vendor export tool failed on several of the remaining large accounts. The original target was October 14, 2026, and the current forecast is October 21, 2026. That change would leave Customer Support one week instead of two for launch readiness. Engineering and the vendor are testing a patched exporter and expect to confirm the forecast on October 10, 2026. It would be helpful if Customer Success could review the affected-account list by October 8, 2026, and flag any contractual deadlines.

### Revised

```markdown
# Atlas migration likely to slip one week

The Atlas migration is now forecast for October 21, 2026, one week later than planned, after the vendor export tool failed on several large accounts.

**Why it matters:** The delay affects the customers with the highest data volumes and compresses the support-readiness window before launch.

**Current state:**

- **Migrated:** 78% of accounts are complete.
- **Remaining risk:** Most unfinished accounts are large customers affected by the export defect.
- **Mitigation:** Engineering and the vendor are testing a patched exporter.

**Action:** Customer Success must review the affected-account list by October 8, 2026, and flag contractual deadlines.

**Next checkpoint:** We will confirm or revise the October 21 forecast on October 10, 2026.
```

### Why the revision works

- It converts activity into the forecast change.
- It explains the audience consequence rather than calling the meetings “productive.”
- It keeps the evidence, owner, and dates needed to act.
- It uses “likely” and a checkpoint because the date is still a forecast.

## Example 2: Decision announcement

### Source draft

> After a long process and input from many people, leadership has been considering how to handle the two analytics tools that are currently available. The review found that maintaining both creates duplicate licensing costs and inconsistent definitions for shared metrics. There are good arguments for both tools, and we appreciate everyone's flexibility. Leadership has decided that Northstar will become the standard analytics platform on January 1, 2027. Beacon will remain available in read-only mode through March 31, 2027. New dashboards should be built in Northstar beginning January 1, business-critical Beacon dashboards must move by December 15, 2026, and each analytics owner should submit a migration plan by September 30, 2026. More information will be shared later.

### Revised

```markdown
# Northstar becomes our analytics standard January 1, 2027

Leadership has selected Northstar as the company-wide analytics platform effective January 1, 2027. Beacon will remain available in read-only mode through March 31, 2027.

**Why it matters:** A single platform reduces duplicate licensing and gives teams one governed source for shared metrics.

**What changes:**

- **New work:** Build new dashboards in Northstar beginning January 1, 2027.
- **Existing dashboards:** Migrate business-critical Beacon dashboards by December 15, 2026.
- **Historical access:** Beacon stays read-only through March 31, 2027.

**Action:** Each analytics owner must identify critical Beacon dashboards and submit a migration plan by September 30, 2026.

**Go deeper:** See the migration guide and approved metric catalog.
```

### Why the revision works

- The final decision and effective date are immediate.
- The impact statement is concrete and supported by the stated rationale.
- The transition is split into observable changes.
- The action has an owner class and deadline.

## Example 3: Customer incident update

### Source draft

> Our teams became aware at 9:12 a.m. ET on September 1, 2026, that some customers could not save new orders, though existing saved orders remained available. We immediately began investigating and paused the most recent deployment. We believe the issue may be related to a database change, but the root cause is not yet confirmed. We are validating the rollback and monitoring save success rates. Customers should keep entered order details open, retry after the next update, and avoid submitting duplicate orders. We apologize for the disruption and hope to have this fixed very soon. We will provide the next update by 10:30 a.m. ET today, even if the status has not changed.

### Revised

```markdown
# Order saves failing for some customers

Since September 1, 2026, at 9:12 a.m. ET, some customers have been unable to save new orders. We are mitigating the issue and have paused the most recent deployment.

**Why it matters:** Affected customers cannot complete new order entry; existing saved orders remain available.

**What we're doing:** We are validating the rollback and monitoring save success rates. The root cause is not yet confirmed.

**What you can do:** Keep entered order details open and retry after our next update; do not submit duplicate orders.

**Next update:** September 1, 2026, at 10:30 a.m. ET, even if the status is unchanged.
```

### Why the revision works

- It leads with customer impact and time, not the investigation chronology.
- It removes an unconfirmed causal claim and unsupported promise.
- It preserves the important limit: existing saved orders are available.
- It gives customers a verified action and a concrete update time.

## Example 4: Preserve a material qualifier

### Unsafe compression

```markdown
The pilot reduced fulfillment time by 18%.
```

### Accurate compression

```markdown
In the 12-clinic pilot, median fulfillment time fell 18% versus the prior four-week baseline; the result has not yet been tested at larger sites.
```

The second version is longer because the sample, metric, comparison, and limitation are decision-relevant. Smart Brevity removes waste, not evidence boundaries.
