# Runbook: High CPU Utilization

## 1. Purpose

This runbook describes the initial investigation of a server
reporting unusually high CPU utilization.

## 2. Symptoms

- CPU utilization remains above the expected operating range.
- Application response times increase.
- Monitoring systems generate CPU utilization alerts.
- Users report slow application performance.

## 3. Initial Checks

1. Confirm the alert and affected host.
2. Check whether the condition is persistent or temporary.
3. Review CPU utilization trends.
4. Check for recent deployments or configuration changes.
5. Identify affected applications and business services.

## 4. Investigation Notes

Record the following information:

- Incident ID:
- Affected host:
- First observed time:
- Current CPU utilization:
- Recent changes:
- User impact:

## 5. Escalation

Escalate to the responsible application or infrastructure
team if the issue persists or the business impact increases.

## 6. Safety

Do not terminate processes or restart production services
without authorization and impact assessment.

## 7. Diagnostic Commands

Use only commands approved for your operating system and
organizational environment.

### Linux examples

Check overall system load:

    uptime

Identify CPU-intensive processes:

    ps -eo pid,comm,%cpu,%mem --sort=-%cpu | head

Review memory usage:

    free -h

These commands are examples for Linux systems. Interpret
their output in the context of the affected workload.

## 8. Recovery Checklist

- [ ] Confirm the suspected cause.
- [ ] Check whether a recent deployment contributed to the issue.
- [ ] Obtain the required authorization before remediation.
- [ ] Apply an approved corrective action.
- [ ] Verify that CPU utilization and application response times improve.
- [ ] Record the resolution and relevant evidence.

## 9. Post-Incident Review

Document the root cause, customer impact, corrective action,
and preventive measures after the incident is resolved.
