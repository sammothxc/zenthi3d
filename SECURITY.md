# Security Policy

Zenthi is a free, community-run project. There's no security team and no bounty budget, but reports are taken seriously and handled as fast as a volunteer project can manage.

## Reporting a vulnerability

**Do not open a public issue for a security problem.**

Report privately through either:

- **GitHub Security Advisories**: use the `Report a vulnerability` button under the repo's **Security** tab (Preferred)
- **Email**: `your_email_or_smthn@email.com`

Please include:

- What the issue is and where (URL, endpoint, table, storage bucket, or file)
- Steps to reproduce, or a minimal proof of concept
- What an attacker could actually do with it
- Anything you think we'd get wrong about the impact

## What to expect

| Stage | Target |
| --- | --- |
| Acknowledgement | 72 hours |
| Initial assessment | 7 days |
| Fix or mitigation for confirmed high-severity issues | 30 days |
| Public disclosure | After a fix ships, coordinated with you |

If a deadline passes, you'll get an explanation rather than silence. Reporters are credited in the advisory unless they'd rather not be.

## In scope

The hosted Zenthi site and this repository, including:

- **Row-Level Security bypass**: any path that reads or writes another user's data, especially private request fulfillments
- **Supabase Storage access control**: reading, overwriting, or deleting files you shouldn't have access to
- **Authentication and session handling**: email/password, GitHub OAuth, Google OAuth, token handling, account takeover
- **File upload handling**: path traversal, content-type confusion, stored XSS via uploaded SVG or PDF, resource exhaustion through malformed CAD/mesh files
- **Injection**: SQL, XSS, template injection, or anything that crosses a trust boundary
- **Server-side request forgery**: the Brave Search integration or any other outbound fetch
- **Secret exposure**: leaked API keys, service-role credentials, or anything in client bundles that shouldn't be there
- **Privilege escalation**: particularly any path to admin that doesn't go through admin approval

## Out of scope

- Reports from automated scanners with no demonstrated impact
- Missing security headers or weak TLS configuration with no exploit path
- Rate limiting on endpoints where abuse causes no real harm
- Social engineering of users, contributors, or admins
- Denial of service through raw traffic volume
- Vulnerabilities in Supabase, Lovable, Brave, or other upstream providers: report those to the vendor
- Anything requiring physical access or a compromised user device

## Not security issues

Some things get misfiled as security reports. These have their own routes:

- **Copyright, licensing, or takedown requests**: (need to add a page for this)
- **Files with wrong or missing attribution**: flag the upload in-app
- **website looks off, or a page is broken**: open a normal issue
- **A part you think is unsafe to run**: see the safety framing in the README. Safety-critical parts are fitment reference only; that's a documented design decision, not a vulnerability.

## Safe harbor

Testing is fine, within limits. Please:

- Only test against accounts and data you own
- Don't access, modify, or destroy other users' files or data
- Don't degrade the service for other people
- Stop and report as soon as you've confirmed a vulnerability; don't keep digging into real data to prove the point
- Give a reasonable window to fix before disclosing publicly

Good-faith research that follows the above won't be pursued legally or reported. If you're unsure whether something crosses a line, please ask first.

## Supported versions

Only the currently deployed version of the hosted site is supported. There are no maintained release branches or backported fixes.
