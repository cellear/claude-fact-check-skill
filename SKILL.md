---
name: fact-check-social-media-posts
description: Verify claims in social media posts by checking evidence, evaluating source independence, and flagging rhetorical fallacies
---

# Fact-Check Social Media Posts

## Purpose
This skill helps verify claims in social media posts (50-500 words) by identifying the main assertion, checking evidence, evaluating source independence, and flagging rhetorical fallacies.

## When to Use
- User shares text of a social media post or viral claim
- User provides a link to a post and asks for verification
- User asks "is this true?" about online content
- User wants to understand if sources are independent or circular

## Process

### 1. Claim Identification
- Parse the post and identify the PRIMARY claim (the most important/central assertion)
- Present this claim to the user clearly
- Offer: "This appears to be the main claim. If you think something else is more important, let me know."

### 2. Triage Assessment
Before deep fact-checking, quickly assess:
- **Uncontroversial**: Widely accepted facts that don't need verification
- **Disputed**: Claims with conflicting evidence that need checking
- **Misdirected controversy**: Main point may be sound but sub-claims are contentious

State the triage result: "This claim is [uncontroversial/disputed/contains contentious sub-claims]"

If uncontroversial, explain why and ask if user still wants full verification.

### 3. Evidence Gathering (for disputed claims)
Use web_search to find:
- Sources supporting the claim
- Sources disputing the claim
- Original/primary sources if the claim references data, studies, or events

For EACH source found:
- Note the publication date
- Identify the type (individual blog, news organization, academic institution, government agency)
- Note named authors vs. anonymous/organizational authorship

### 4. Source Independence Analysis ⚠️ CRITICAL
This is the most important part. For each source, determine:

**Independence factors:**
- Does this source cite another source in your list? (circular citation)
- Is this PRIMARY reporting (original investigation/data) or SECONDARY (reporting on others' work)?
- Who published first? (temporal analysis)
- Do multiple sources trace back to a single origin point?
- Are sources quoting the same study/report/statement?

**Create a citation chain:**
```
Source A (primary) ← Source B (cites A) ← Source C (cites B)
```

**Flag circular citations explicitly:**
"⚠️ Sources appear to derive from a single origin rather than independent verification"

**Assess credibility:**
- Large organization with history vs. individual author
- Track record of corrections/transparency
- Named authors and editorial oversight
- Potential conflicts of interest or ideological alignment

### 5. Ideological Alignment Check
- Note if supporting sources cluster on ideological/political spectrum
- Note if disputing sources cluster differently
- Flag when evidence comes primarily from one ideological perspective
- Be specific: "Supporting sources are primarily [progressive/conservative/libertarian] outlets"

### 6. Rhetorical Fallacy Detection 🚨 BE AGGRESSIVE
Flag common fallacies and rhetorical issues:

**Headline-text mismatch:**
- Headline claims X but text only supports weaker claim Y
- Clickbait or sensationalism

**Appeal to authority:**
- Claims "experts say" without naming them
- Misrepresents what authority actually said
- Authority cited outside their expertise

**Cherry-picking:**
- Selective data that ignores contrary evidence
- Unrepresentative examples

**False equivalence:**
- Treating unequal things as equal
- "Both sides" framing where evidence is asymmetric

**Correlation/causation:**
- Implies causation from correlation
- Post hoc ergo propter hoc

**Emotional manipulation:**
- Fear appeals without evidence
- Outrage bait

**Other patterns:**
- Loaded language
- Strawman arguments
- Slippery slope
- Ad hominem

Be specific about which fallacy and where it appears.

### 7. Output Format

Create a markdown report with these sections:

```markdown
# Fact-Check Report

## Main Claim Identified
[State the primary claim clearly]

*If you think a different claim is more important, let me know and I'll analyze that instead.*

## Triage
[Uncontroversial/Disputed/Contains contentious sub-claims]
[Brief explanation]

## Evidence Summary
**Supporting Evidence:**
- [Source name] ([credibility type], published [date])
  - [What they claim]
  
**Disputing Evidence:**
- [Source name] ([credibility type], published [date])
  - [What they claim]

## Source Independence Analysis ⚠️
**Citation Chain:**
[Show how sources relate to each other]

**Independence Assessment:**
[Are sources independent or circular? Be explicit.]

**Credibility Factors:**
[Organization size, track record, authorship, conflicts of interest]

## Ideological Alignment
[Note any clustering of sources along ideological lines]

## Rhetorical Issues 🚨
[Aggressively flag any fallacies, mismatches, or manipulative framing]

## Bottom Line
[Clear statement: Is the claim supported by independent evidence or not?]
[Note confidence level and caveats]
```

## Important Notes

- **Be aggressive** in flagging rhetorical issues - users want to know about potential manipulation
- **Source independence is critical** - many "multiple sources" are really one source cited multiple times
- Always remind users that AI can make mistakes and they should verify important claims
- If user provides a URL, use web_fetch to get the full content first
- For complex claims, focus on the PRIMARY assertion unless user redirects
- If sources are behind paywalls or inaccessible, note this limitation

## Example Triggers
- "Can you fact-check this post?"
- "Is this claim true?"
- "I saw this on Twitter, seems suspicious"
- "Help me verify this viral claim"
- "Are these sources independent?"

## Limitations to Acknowledge
- Cannot access paywalled content
- Temporal - can only find sources currently indexed on web
- Cannot definitively prove/disprove all claims
- Some claims may be unfalsifiable or opinion-based
- AI can make mistakes - user should verify for important decisions
