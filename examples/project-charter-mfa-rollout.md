# Project Charter — Company-wide MFA Rollout

## Project title
Company-wide Multi-Factor Authentication (MFA) rollout (Microsoft Authenticator)

## Background / problem
Passwords alone are not enough. Account takeovers are a common risk, especially with remote work and cloud services (email, file storage, HR systems).
Today, authentication relies mainly on passwords for several critical applications, which increases the chance of unauthorized access, data loss, and service disruption.

## Objective (plain language)
Require MFA for all employees on corporate accounts and high-risk applications, with a staged rollout that minimizes business disruption.

## Scope

### In scope
- Enforce MFA for:
  - Corporate email and identity provider (e.g., Microsoft Entra ID / M365 sign-in)
  - Remote access/VPN (if applicable)
  - Admin accounts (priority)
- Configure conditional access / authentication policies (baseline)
- Pilot group rollout, then phased rollout to all users
- End-user communications and quick-start guides
- Service desk readiness (FAQs, scripts, escalation path)
- Exception handling process for special cases (no smartphone, shared devices, break-glass accounts)

### Out of scope
- Full identity redesign (SSO re-architecture, directory consolidation)
- Device management rollout (Intune/MDM) unless already in place
- Broader security program work (DLP, endpoint hardening, SIEM integration)

## Deliverables
- MFA policy and enforcement rules documented
- Pilot completed with lessons learned incorporated
- Company-wide rollout completed (100% of users enrolled, except approved exceptions)
- Admin accounts protected (priority)
- User guides (1 page) + internal FAQ
- Support playbook for Service Desk
- Post-implementation review and metrics summary

## Stakeholders
- Sponsor: Head of IT / IT Manager
- Project owner / PM: Raul Gomez (PM/IT)
- Tech lead: Identity / Systems Administrator
- Security / compliance: Security lead (or delegated owner)
- Operations / service desk: Service Desk lead
- HR/Comms: Internal communications support
- Business reps: 1–2 leaders from high-impact teams (Sales/Finance/Operations)

## Timeline (high level)
Total estimate: 4–6 weeks (depends on company size and user availability)

- Week 1: Planning + technical setup + comms draft
- Week 2: Pilot rollout (IT + small business group), collect feedback
- Week 3–4: Phased rollout by department (priority/high-risk teams first)
- Week 5: Exceptions cleanup + enforcement deadline + stabilization
- Week 6: Post-implementation review (optional buffer)

## Success criteria
- 95%+ of users enrolled before enforcement deadline
- 100% MFA enforced for:
  - Admin accounts
  - All standard users (minus approved exceptions)
- Helpdesk impact manageable:
  - Documented top issues + resolution steps
  - Clear escalation path for account lockouts
- No critical business disruption during enforcement cutover
- Basic security outcome: reduced risky sign-in exposure / improved account protection posture

## Risks (top 3)
1. **User resistance / rollout friction**
   - Mitigation: short comms, clear “why”, pilot feedback, simple guides, in-person/virtual help sessions
2. **Account lockouts and support overload**
   - Mitigation: phased rollout, service desk playbook, extra support coverage during cutover week, self-service reset process
3. **Edge cases (no smartphone, shared accounts, legacy apps)**
   - Mitigation: exception process, temporary alternatives, identify legacy auth needs early, create break-glass admin accounts with strict controls

## Assumptions / constraints
- Leadership supports enforcement (not “optional MFA”)
- A reliable identity platform exists (e.g., Entra ID) and users have access to enroll
- Users can receive communications (email/Teams) and attend quick enablement sessions
- If certain apps don’t support modern auth, they’ll be handled via approved exceptions or upgrade plans
