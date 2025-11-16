# Guide for Free Users (No Claude Pro Required)

Don't have Claude Pro? No problem! You can still use this fact-checking methodology with free AI tools. This guide shows you how.

## Quick Start

1. **Choose your AI assistant** (must have web search capability)
2. **Copy the prompt** from [`PROMPT.txt`](../PROMPT.txt) 
3. **Paste it** at the start of a new conversation
4. **Share the claim** you want fact-checked
5. **Review the report** the AI generates

That's it! The AI will follow the methodology step-by-step.

## Compatible AI Assistants

### ✅ Free Claude.ai
- **Pros**: Excellent at following complex instructions, strong reasoning
- **Cons**: Web search may have some limitations on free tier
- **How to use**: Just paste the prompt and start chatting
- **Link**: [claude.ai](https://claude.ai)

### ✅ ChatGPT (with browsing)
- **Pros**: Good web search, widely available
- **Cons**: May need reminders to follow all steps
- **How to use**: Paste prompt, ensure browsing is enabled
- **Link**: [chat.openai.com](https://chat.openai.com)
- **Note**: Web browsing may require ChatGPT Plus in some regions

### ✅ Perplexity AI
- **Pros**: Excellent web search, built for research
- **Cons**: May format output differently
- **How to use**: Works great out of the box
- **Link**: [perplexity.ai](https://perplexity.ai)

### ✅ Microsoft Copilot (Free)
- **Pros**: Free web search, widely accessible
- **Cons**: May be less thorough with complex analysis
- **How to use**: Paste prompt in "Creative" or "Precise" mode
- **Link**: [copilot.microsoft.com](https://copilot.microsoft.com)

## Step-by-Step Instructions

### Step 1: Get the Prompt

Go to [`PROMPT.txt`](../PROMPT.txt) in this repository and copy the entire text. It contains all the instructions the AI needs.

### Step 2: Start a New Conversation

Open your chosen AI assistant and start a fresh conversation. This ensures the AI focuses only on your fact-check request.

### Step 3: Paste the Prompt

Paste the entire contents of `PROMPT.txt` as your first message. The AI will acknowledge it's ready to fact-check.

### Step 4: Share the Claim

In your next message, share the social media post or claim you want verified. You can:

```
Can you fact-check this post?

"[paste the social media post here]"
```

Or provide a link:

```
Can you fact-check this claim: https://example.com/post/12345
```

### Step 5: Review and Follow Up

The AI will produce a detailed report. You can:
- Ask for clarification on specific points
- Request deeper analysis of particular sources
- Challenge the AI's assessment if you disagree
- Ask it to check a different claim from the same post

## Tips for Best Results

### ✅ Do This

- **Use exact quotes** when sharing claims - copy-paste the original text
- **Specify what matters** if the post makes multiple claims
- **Ask follow-up questions** if something's unclear
- **Verify important findings** yourself using the sources the AI cites
- **Be specific** about what concerns you most

### ❌ Avoid This

- **Don't combine multiple unrelated claims** in one request
- **Don't expect 100% accuracy** - AI can make mistakes
- **Don't skip reading the sources** - always check the AI's citations
- **Don't use for time-sensitive decisions** without verification
- **Don't rely solely on AI** for critical fact-checking

## Example Session

Here's what a typical fact-check session looks like:

```
You: [Paste entire PROMPT.txt contents]

AI: Ready! Share a social media post or claim you'd like me to fact-check.

You: Can you fact-check this?

"BREAKING: Scientists discover new planet closer than Mars. 
Space agencies confirm it's been hiding behind the Sun!"

AI: # Fact-Check Report

## Main Claim Identified
Scientists have discovered a new planet closer to Earth than Mars that 
has been hiding behind the Sun.

[... detailed analysis follows ...]

You: The post also mentions it has water - can you check that claim too?

AI: [Analyzes the water claim specifically...]
```

## Differences from Claude Skills Version

The prompt version works the same way, but:

**Advantages:**
- ✅ Free to use
- ✅ Works with multiple AI assistants
- ✅ You control when to apply it

**Trade-offs:**
- ⚠️ Must paste the prompt for each new conversation
- ⚠️ AI might occasionally need reminders to follow all steps
- ⚠️ Different AI assistants may have varying web search quality

## Troubleshooting

### Problem: AI doesn't follow all the steps

**Solution**: Remind it specifically:
```
Can you also analyze source independence? That's the critical part.
```

### Problem: AI can't access sources

**Solution**: The AI will note this. You may need to:
- Share the article text directly if you have access
- Try a different AI assistant with better web access
- Accept that paywalled sources can't be fully verified

### Problem: Output is too brief

**Solution**: Ask for more detail:
```
Can you expand the source independence analysis? I want to see 
the full citation chain.
```

### Problem: AI seems biased

**Solution**: Ask it to check its reasoning:
```
Are you considering sources from different ideological perspectives?
Show me sources that dispute this claim too.
```

## Saving Your Conversations

Consider keeping records of important fact-checks:
- Screenshot or save the conversation
- Copy the report to a document
- Note the date (fact-checks become stale over time)
- Save links to sources you verified personally

## When to Get Claude Pro

Consider upgrading to Claude Pro ($20/month) if you:
- Fact-check frequently (multiple times per week)
- Want automated skill activation
- Need consistent methodology application
- Prefer seamless experience without copy-pasting

Otherwise, the free prompt version works great!

## Questions?

Having trouble? [Open an issue](https://github.com/YOUR-USERNAME/fact-check-skill/issues) and we'll help you out.

---

**Remember**: This methodology is a tool to help you think critically. Always verify important claims through multiple independent sources and use your own judgment. AI can make mistakes!

