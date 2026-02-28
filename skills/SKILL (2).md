# Skill: Systematic Debugging

Structured 4-phase debugging workflow for complex issues.  
Goal: eliminate random guessing and identify the real root cause with evidence.

---

## When to Use
Use this skill when:
- A bug is unclear or intermittent
- The issue spans multiple files or systems
- Quick fixes failed
- Root cause is unknown

---

## 4-Phase Debugging Process

### 1. Reproduce
Before fixing anything, confirm the issue can be reproduced.

#### Reproduction Steps
1. [Exact step to reproduce]
2. [Next step]
3. [Expected result]
4. [Actual result]

#### Reproduction Rate
- Always (100%)
- Often (50–90%)
- Sometimes (10–50%)
- Rare (<10%)

If the bug cannot be reproduced reliably, continue investigation before attempting a fix.

---

### 2. Isolate
Narrow down where the issue originates.

Key questions:
- When did this start happening?
- What changed recently?
- Does it happen in all environments?
- Can it be reproduced with minimal code?
- What is the smallest trigger?

Use:
- File search
- Code history
- Logs

---

### 3. Understand (Root Cause Analysis)

Focus on the real cause, not symptoms.

#### The 5 Whys Method
1. Why did this happen?
2. Why did that occur?
3. Why is that possible?
4. Why wasn't it prevented?
5. Root cause identified

Document the root cause clearly.

---

### 4. Fix & Verify

After applying a fix, verify thoroughly.

#### Verification Checklist
- Bug no longer reproduces
- Related features still work
- No new issues introduced
- Regression test added

---

## Debugging Workflow Checklist

### Before Starting
- Issue reproduced
- Expected behavior understood
- Minimal reproduction case created

### During Investigation
- Check recent commits
- Review logs
- Add temporary logging if needed
- Use debugger or breakpoints

### After Fix
- Root cause documented
- Fix validated
- Regression test added
- Similar code reviewed

---

## Useful Debugging Commands

Recent changes: