# Trend-to-Niche Content Agent System

Multi-agent content workflow for finding current trends, mining viral hook patterns, adapting them to a Hinglish creator niche, writing short-form scripts, generating CTAs, and verifying the final content package before publishing.

## Structure

- `AGENTS.md` - repo-level operating rules for the content system.
- `data/channel_profile.md` - audience, voice, content buckets, and CTA style.
- `skills/*/SKILL.md` - reusable agent workflows.
- `prompts/master_run_prompt.md` - end-to-end orchestration prompt.
- `outputs/` - generated trend, hook, script, and recommendation files.

## Workflow

Run the master prompt and follow the agents in order:

1. Trend discovery
2. Viral filtering
3. Hook mining
4. Niche alignment
5. Style pattern extraction
6. Script writing
7. CTA generation
8. Storyboard / AI scene selection
9. Verification

Final output should always include the trend, adapted hook pattern, script, CTA options, verifier report, and recommended best version.

The script writer uses `combined_scripts_1_32.md`, `script_*.md`, and `prompts/secret_business_story_style_guide.md` as the reference style library. The storyboard scene selector recommends only the few highest-impact scenes worth generating with Higgsfield / Seedance so creators do not waste credits.
