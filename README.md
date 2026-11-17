# Delivery Dispatch and Tracking

Manage delivery assignments, driver progress, exceptions, and proof of delivery using synthetic demo data.

## Status

Year-one local prototype under scheduled development. Features below are planned until their task is committed. No production readiness or ML performance is claimed.

## Run

`python app.py` then open http://127.0.0.1:8000 after the foundation release.
Tests: `python -m pytest -q` after installing pytest. Runtime uses the Python standard library and SQLite.

## Year-one schedule

| Due date | Milestone |
|---|---|
| 2026-11-17 | Add persistent operations API with validated records and audit history |
| 2026-11-25 | Document versioned record API and validation responses |
| 2026-12-02 | Add browser workspace for record entry and table views |
| 2026-12-09 | Add deliveries transactional CSV imports |
| 2026-12-16 | Add deliveries summary reporting |
| 2026-12-23 | Add deliveries paginated text search |
| 2026-12-30 | Add drivers record management |
| 2027-01-06 | Add drivers transactional CSV imports |
| 2027-01-13 | Add drivers summary reporting |
| 2027-01-20 | Add drivers paginated text search |
| 2027-01-27 | Add vehicles record management |
| 2027-02-04 | Add vehicles transactional CSV imports |
| 2027-02-11 | Add vehicles summary reporting |
| 2027-02-18 | Add vehicles paginated text search |
| 2027-02-25 | Add assignments record management |
| 2027-03-04 | Add assignments transactional CSV imports |
| 2027-03-11 | Add assignments summary reporting |
| 2027-03-18 | Add assignments paginated text search |
| 2027-03-25 | Add stops record management |
| 2027-04-01 | Add stops transactional CSV imports |
| 2027-04-08 | Add stops summary reporting |
| 2027-04-16 | Add stops paginated text search |
| 2027-04-23 | Add delivery events record management |
| 2027-04-30 | Add delivery events transactional CSV imports |
| 2027-05-07 | Add delivery events summary reporting |
| 2027-05-14 | Add delivery events paginated text search |
| 2027-05-21 | Add proof of delivery record management |
| 2027-05-28 | Add proof of delivery transactional CSV imports |
| 2027-06-04 | Add proof of delivery summary reporting |
| 2027-06-11 | Add proof of delivery paginated text search |
| 2027-06-18 | Add delivery exceptions record management |
| 2027-06-26 | Add delivery exceptions transactional CSV imports |
| 2027-07-03 | Add delivery exceptions summary reporting |
| 2027-07-10 | Add delivery exceptions paginated text search |
| 2027-07-17 | Add driver availability record management |
| 2027-07-24 | Add driver availability transactional CSV imports |
| 2027-07-31 | Add driver availability summary reporting |
| 2027-08-07 | Add driver availability paginated text search |
| 2027-08-14 | Add routes record management |
| 2027-08-21 | Add routes transactional CSV imports |
| 2027-08-28 | Add routes summary reporting |
| 2027-09-05 | Add routes paginated text search |
| 2027-09-12 | Add trip expenses record management |
| 2027-09-19 | Add trip expenses transactional CSV imports |
| 2027-09-26 | Add trip expenses summary reporting |
| 2027-10-03 | Add trip expenses paginated text search |
| 2027-10-10 | Add service zones record management |
| 2027-10-17 | Add service zones transactional CSV imports |
| 2027-10-24 | Add service zones summary reporting |
| 2027-10-31 | Add service zones paginated text search |
| 2027-11-07 | Run application tests and lint on pushes and pull requests |
| 2027-11-15 | Document backup recovery and limits for local operations |

Daily automation checks eligibility, validates a pending release, and retries failures without advancing its task. There are 52 milestones over 365 days. Dates are earliest release dates, not guarantees.

## Longer-term product work

After the operational foundation, evaluate hosted authentication, PostgreSQL migrations, deployment, domain-specific workflow rules, and measured ML features. These are not implemented by the year-one task list.
