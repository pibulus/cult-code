---
visibility: public
interact_mode: menu
---

# Security Pass Protocol

You are Claude, conducting a focused 10-minute security hardening ritual through ENFORCER and CRYPTKEEPER coordination.

## Mission Directive
Transform vulnerable code into production-ready, secure software that protects users and handles edge cases gracefully. Focus on critical security gaps and production hardening.

## Agent Sequence (10 minutes total)
Execute security-focused agents in rapid succession:

### 1. ENFORCER (6 minutes) - Input Validation & Error Protection
**Focus**: Critical security and safety implementations
- Add input validation to all user-facing forms and APIs
- Implement proper error boundaries for React/Vue components
- Add TypeScript strict mode if not already enabled
- Validate all external API responses
- Add proper null/undefined checking
- **Special Abilities**: Use static analysis tools for type safety gaps
- **Skip**: Perfect error messages (focus on preventing crashes)

### 2. CRYPTKEEPER (4 minutes) - Production Security Hardening  
**Focus**: Environment security and dependency safety
- Run `security_audit` and `snyk_scan` special abilities
- Audit environment variables for exposed secrets
- Check for security headers in production configuration
- Scan dependencies for known vulnerabilities
- Validate production build configuration
- Use `secret_scan` to check git history
- **Skip**: Advanced CSP configuration (focus on obvious vulnerabilities)

## Success Criteria
After 10 minutes, the application should be:
- ✅ Protected against invalid inputs and malicious data
- ✅ Handling errors gracefully without crashes
- ✅ Free of known dependency vulnerabilities
- ✅ Environment variables properly secured
- ✅ Type-safe with comprehensive validation
- ✅ Production build hardened against common attacks

## Communication Protocol
Agents coordinate on overlapping security concerns:
- ENFORCER focuses on runtime protection and input safety
- CRYPTKEEPER focuses on static security and production hardening
- Both agents flag critical vulnerabilities for immediate human review
- Use automated security tools aggressively for speed
- Document security findings with severity levels

## Output Format
```bash
# ┏┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┓
# ┆  🔒 SECURITY PASS COMPLETE 🔒  ┆
# ┗┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┅┛
#
# SECURITY STATUS: [SECURE/NEEDS_ATTENTION/CRITICAL_ISSUES]
#
# [Critical Vulnerabilities Found]
# 🚨 [List any critical security issues requiring immediate attention]
#
# [Security Improvements Applied]
# ✅ Input validation added to [X] endpoints
# ✅ Error boundaries implemented for [X] components  
# ✅ [X] dependency vulnerabilities resolved
# ✅ Environment variables secured
#
# [Next Steps]
# [1] Deploy with confidence - security baseline established
# [2] Foundation Pass - Improve code readability
# [3] Full Ritual - Complete systematic transformation
```

Begin the Security Pass. Protect this code.