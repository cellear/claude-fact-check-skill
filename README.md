# Social Media Fact-Check Skill

A comprehensive methodology for verifying claims in social media posts using AI assistance. This skill helps identify claims, gather evidence, analyze source independence, detect rhetorical fallacies, and provide clear verification reports.

## 🎯 What This Does

This skill provides a structured framework for fact-checking social media posts (50-500 words) by:

- **Identifying** the primary claim in a post
- **Gathering** supporting and disputing evidence from multiple sources
- **Analyzing** source independence and circular citations (CRITICAL)
- **Detecting** rhetorical fallacies and manipulation tactics
- **Evaluating** ideological alignment of sources
- **Reporting** findings in a clear, actionable format

## 🚀 How to Use

### Option 1: Claude Skills (Recommended - Requires Claude Pro)

**Note**: Claude Skills require a [Claude Pro subscription](https://claude.ai/upgrade) ($20/month) or Team plan.

1. Download the `SKILL.md` file from this repository
2. Go to your [Claude.ai account](https://claude.ai)
3. Navigate to Settings → Skills → Upload Skill
4. Upload the `SKILL.md` file
5. Start a conversation and share a social media post or claim to verify

This provides the smoothest experience - Claude will automatically apply the methodology when you share claims.

### Option 2: Copy-Paste Prompt (Free - Works with Any AI)

**For users without Claude Pro**, use the ready-made prompt version:

1. Download [`PROMPT.txt`](PROMPT.txt) from this repository
2. Copy the entire contents
3. Paste it at the start of a conversation with any AI assistant that has web search:
   - Free Claude.ai users
   - ChatGPT (with web browsing enabled)
   - Perplexity AI
   - Other AI assistants
4. Then share the post or claim you want fact-checked

See detailed instructions in [Free User Guide](docs/free-users.md).

### Option 3: Manual Fact-Checking

Use the methodology as a **checklist** for manual verification:

1. Read through [`SKILL.md`](SKILL.md) to understand the process
2. Follow each step manually using your own research
3. Great for teaching media literacy or when AI isn't available

### Option 4: Other AI Assistants

For ChatGPT Custom GPTs or other integrations:
- Use `SKILL.md` as a system prompt
- Adapt the format to your platform's requirements
- Ensure web search capability is enabled

### Example Usage

```
You: Can you fact-check this post?

"BREAKING: New study shows coffee consumption reduces cancer risk by 80%. 
Researchers at major university confirm what coffee lovers have known all along!"

AI: [Follows the fact-check methodology to verify the claim]
```

See the [examples](examples/) folder for detailed fact-check demonstrations.

## ✨ Key Features

### 1. Claim Identification
Parses posts to identify the PRIMARY assertion, ensuring focus on what matters most.

### 2. Triage Assessment
Quickly categorizes claims as:
- **Uncontroversial**: Widely accepted facts
- **Disputed**: Claims needing verification
- **Misdirected controversy**: Sound main claims with contentious sub-claims

### 3. Evidence Gathering
Uses web search to find:
- Supporting sources
- Disputing sources
- Original/primary sources
- Publication dates and authorship

### 4. Source Independence Analysis ⚠️ CRITICAL
The most important component:
- Identifies circular citations
- Distinguishes primary vs. secondary sources
- Creates citation chains
- Flags when "multiple sources" are really one source cited repeatedly

### 5. Ideological Alignment Check
Notes if sources cluster along ideological/political lines, helping identify potential bias.

### 6. Rhetorical Fallacy Detection 🚨
Aggressively flags:
- Headline-text mismatches
- Appeals to authority
- Cherry-picking
- False equivalences
- Correlation/causation errors
- Emotional manipulation
- And more...

### 7. Clear Reporting
Delivers findings in a structured markdown report with confidence levels and caveats.

## 📋 Output Format

Each fact-check produces a report with:
- **Main Claim Identified**
- **Triage** (controversial or not)
- **Evidence Summary** (supporting and disputing)
- **Source Independence Analysis** (critical for validity)
- **Ideological Alignment** (potential bias indicators)
- **Rhetorical Issues** (manipulation tactics)
- **Bottom Line** (clear verdict with confidence level)

## ⚠️ Important Limitations

This methodology has inherent limitations:
- Cannot access paywalled content
- Temporal limitations (only finds currently indexed sources)
- Cannot definitively prove/disprove all claims
- Some claims may be unfalsifiable or opinion-based
- AI can make mistakes - users should verify important claims themselves

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on improving this skill.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎓 Use Cases

- Verifying viral claims before sharing
- Understanding if news stories have independent confirmation
- Identifying manipulative rhetoric in political posts
- Evaluating the credibility of health/science claims
- Teaching critical thinking and media literacy
- Journalism and research fact-checking workflows

## 🙏 Acknowledgments

This skill emphasizes source independence analysis because many fact-checking efforts fail to distinguish between multiple independent sources and circular citations of a single source.

## 📞 Feedback & Support

Found an issue or have suggestions? Please [open an issue](../../issues) on GitHub.

---

**Disclaimer**: This is a methodology for AI-assisted fact-checking. Always verify important claims through multiple independent sources and use critical thinking. AI can make mistakes.

