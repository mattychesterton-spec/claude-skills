# natural-writing

**A Claude skill that kills the AI smell.**

Based on [Wikipedia's AI Cleanup project](https://en.wikipedia.org/wiki/Wikipedia:AI_Cleanup) research into patterns observed across thousands of LLM-generated texts. This skill trains Claude to avoid the statistical tells that make AI prose instantly recognisable.

---

## The Problem

LLMs regress to the mean. They omit specific, unusual, nuanced facts (statistically rare) and replace them with generic, positive descriptions (statistically common). The result: text that's simultaneously less specific and more exaggerated.

You know it when you see it. Sentences that end with "...marking a pivotal moment in the industry." Paragraphs about "rich tapestries" and "unique blends." The word "delve" appearing three times in 500 words.

## What This Skill Does

Triggers on any writing request—blog posts, articles, marketing copy, essays, reviews, reports, social posts, emails—and applies anti-pattern rules to produce prose that sounds like a person wrote it.

### Structural Patterns It Catches

| Pattern | Example | Why It's a Tell |
|---------|---------|-----------------|
| Trailing participles | "...underscoring its commitment to innovation" | Vague significance claims are LLM comfort food |
| False ranges | "from casual users to enterprise clients" | No meaningful scale between endpoints |
| Rule of three | "insights, strategies, and solutions" | Statistical default, not deliberate choice |
| Elegant variation | "the company... the firm... the organisation" | Synonym-swapping sounds robotic |
| Despite/challenges formula | "Despite its success, X faces challenges typical of..." | Rigid hedge pattern |
| False contrasts | "You don't need X—you need Y" | Creates artificial tension between non-opposites |

### Vocabulary It Flags

High-alert words that co-occur in LLM output:

```
delve, tapestry, multifaceted, underscore, pivotal, intricate, 
landscape (abstract), testament, showcase, foster, garner, 
vibrant, enhance, crucial, additionally, interplay, enduring
```

One or two may be coincidental. Multiple appearances = strong tell.

### Tone Traps It Avoids

**TV commercial voice:** nestled, in the heart of, boasts a, breathtaking, world-class, cutting-edge, seamlessly, rich tapestry, unique blend, continues to captivate

**Vague attribution:** "Experts argue...", "Industry reports suggest...", "Some critics note..."

**Over-claiming significance:** "stands as a testament to", "plays a pivotal role", "reflects broader trends"

## Installation

Add to your Claude skill folder as `SKILL.md`. The skill triggers automatically on writing requests.

```
/skills/
└── natural-writing/
    ├── SKILL.md
    └── references/
        ├── vocabulary.md
        └── structural-tells.md
```

## The Self-Check

The skill includes a 10-point review process:

1. Search for trailing "-ing" clauses about significance—cut all of them
2. Search for "pivot", "crucial", "vital", "testament", "underscore", "tapestry", "landscape", "foster", "delve"—rewrite or cut
3. Count triads—break most of them
4. Check for "Despite... challenges" formula
5. Check for false ranges ("from X to Y")
6. Check for vague attributions ("experts say", "some argue")
7. Check for false contrasts ("you don't need X, you need Y")
8. Check for vague backward references—repeat the noun if unclear
9. Verify every paragraph advances the argument
10. Read aloud: does it sound like a person or a brochure?

## Core Principles

**Concrete over abstract.** Not "comprehensive landscape"—name the thing.

**Short over Latinate.** "Use" not "utilize". "Help" not "facilitate".

**Specific over generic.** "Inventor of the first train-coupling device" beats "revolutionary titan of industry."

**Commit to positions.** Avoid the equivocation seesaw. Take a stance.

## Contributing

Found a pattern that screams AI? Open an issue or PR. The goal is comprehensive coverage of statistical tells without becoming so restrictive that Claude can't write anything.

## Acknowledgements

Built on research from [Wikipedia's AI Cleanup project](https://en.wikipedia.org/wiki/Wikipedia:AI_Cleanup), which identified these patterns through analysis of thousands of LLM-generated edits.

---

*The test: could someone read this and not know an AI wrote it?*
