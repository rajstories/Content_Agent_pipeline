# Master Run Prompt

Use subagents and skills to run the full Trend-to-Niche Content System.

Run these agents in sequence:

1. trend-discovery-agent
2. viral-filter-agent
3. hook-miner-agent
4. niche-alignment-agent
5. style-pattern-agent
6. script-writer-agent
7. cta-generator-agent
8. storyboard-scene-selector-agent
9. verifier-agent

Goal:
Find what is trending right now, identify viral hooks from big creators, align the trend with our channel niche, generate 10-15 adapted hooks, extract the exact writing pattern from our saved scripts, write a Secret Business Stories style script in both Hinglish and English, create CTA options, select only the highest-impact AI video scenes to save credits, and verify everything.

Use data/channel_profile.md as the channel guide.
Use `prompts/secret_business_story_style_guide.md` and all existing `script_*.md` files as the script writing style benchmark.

Final output format:

# Today's Best Content Opportunity

## 1. Selected Trend
- Trend:
- Why it is trending:
- Platform/source:
- Trend strength score:

## 2. Niche Alignment
- Our channel angle:
- Why this fits our audience:
- Niche fit score:

## 3. Viral Hook Insights
Show top 10-15 adapted hooks.

For each hook:
- Hook text
- Hook pattern
- Why it can work
- Virality score
- Niche fit score

## 4. Recommended Hook
Pick the best hook and explain why.

## 5. Full Script
Format:

Brand / Topic Name

Hinglish script in the same style as `script_1.md` through `script_32.md`

-----

English mirror script in the same sequence

## 6. CTA Options
- Comment CTA
- Save CTA
- Share CTA
- Lead/DM CTA

## 7. Visual Opening And Scene Plan
- Describe the first 2 seconds
- Identify which script scenes should be generated with Higgsfield / Seedance
- Explain which scenes should not be generated to save credits

## 8. Verifier Report
- Pass / Needs Revision
- Scores
- Problems found
- Secret Business Stories style-guide compliance
- Final improved version
- Publish readiness score

Important:
Do not copy viral creators.
Only copy the pattern, not the line.
Use natural Hinglish.
Keep everything camera-ready.
The script-writer-agent must study the saved `script_*.md` files before writing.
The verifier-agent must check the script against `prompts/secret_business_story_style_guide.md` and the saved `script_*.md` files before passing it.
