# MigrationGuard

Prevent production incidents caused by unnoticed database changes.

MigrationGuard is a GitHub App that automatically detects database schema changes in Pull Requests and warns reviewers before risky merges happen.

Many deployment failures are not caused by application code, but by hidden operational changes — especially database migrations.  
MigrationGuard helps teams catch these issues during code review.

---

## What it does

When a Pull Request is opened or updated, MigrationGuard:

- Scans changed files
- Detects database migrations (SQL, Flyway, Liquibase)
- Warns reviewers automatically
- Adds operational awareness to code reviews

Example warnings include:

- new tables or columns
- schema modifications
- destructive operations (drop/alter)
- hidden SQL scripts

---

## Why this matters

Database changes are different from code changes:

- harder to rollback
- depend on real production data
- can lock tables
- often bypass normal review attention

MigrationGuard makes operational risk visible inside the Pull Request — where developers already work.

---

## Planned features

- Jira change request automation
- Release checklist enforcement
- Slack notifications
- Impacted service detection
- Automated release notes

---

## Status

Early development.

We are currently looking for early adopters and feedback from teams running production systems.

👉 Join early access: (link coming soon)

---

## Who is this for?

Teams using:

- relational databases (PostgreSQL, MySQL, Oracle, SQL Server)
- CI/CD pipelines
- Pull Request based workflows
- controlled releases

Especially helpful for monoliths and multi-module backends.

---

## License

MIT
