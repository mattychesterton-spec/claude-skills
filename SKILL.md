---
name: natural-writing
description: Anti-AI-pattern writing guide for natural, human-sounding prose. Triggers on ANY writing request including blog posts, articles, marketing copy, essays, reviews, reports, social posts, emails, or any drafted content. Based on Wikipedia's AI Cleanup project research into patterns observed across thousands of LLM-generated texts.
---

# Natural Writing

Avoid patterns that signal AI-generated prose. These tells are deeply embedded in how LLMs are trained — statistical regression to the mean produces text that is simultaneously less specific and more exaggerated.

## Core Principle

LLMs omit specific, unusual, nuanced facts (statistically rare) and replace them with generic, positive descriptions (statistically common). Counter this: be specific, be concrete, commit to positions.

## Structural Patterns to Avoid

### Trailing Participle Clauses

Never end sentences with "-ing" phrases claiming vague significance. This is one of the strongest tells.

❌ "...marking a pivotal moment in regional statistics"
❌ "...emphasizing the company's commitment to innovation"
❌ "...reflecting the continued relevance of traditional methods"
❌ "...underscoring its role as a dynamic hub"
❌ "...symbolizing its ongoing impact"

If you need to state significance, make it the main clause with evidence.

### Undue Emphasis on Legacy/Importance

Don't puff up subjects with statements about how they "represent or contribute to broader topics." This pattern appears even for mundane subjects like etymology or population data.

❌ "This initiative was part of a broader movement across Spain to decentralize administrative functions"
❌ "The etymology highlights the enduring legacy of the community's resistance"
❌ "It holds a pivotal place in... serving as a major hub with historical significance"

State facts. Let readers judge importance.

### The "Despite... Challenges" Formula

Avoid the rigid pattern: "Despite its [positive words], [subject] faces challenges..." followed by vague positive assessment or speculation about future initiatives.

❌ "Despite its industrial prosperity, X faces challenges typical of urban areas... With ongoing initiatives, X continues to thrive"

### False Ranges

Don't use "from X to Y" when no meaningful scale exists between the endpoints.

❌ "from casual users to enterprise clients" (unless range genuinely matters)
❌ "from problem-solving and tool-making to scientific discovery and artistic expression"

If you can't identify middle ground without switching scales, it's a false range.

### Negative Parallelisms

Avoid constructions designed to appear balanced and thoughtful:

❌ "Not only X, but also Y"
❌ "It is not just about X, it's Y"
❌ "X, however, took a path that..."

These are fine occasionally. Problematic when formulaic or when X and Y don't genuinely contrast.

### False Contrasts

Avoid the "You don't need X—you need Y" structure and similar constructions that create artificial tension between things that aren't really opposites.

❌ "You don't need elaborate programs—you need regular conversation"
❌ "It's not about the tools—it's about the people"

Often both parts are true, making the contrast feel forced. Just state what matters.

### Rule of Three

Don't default to three items in lists. LLMs overuse triadic structures to appear comprehensive.

❌ "keynote sessions, panel discussions, and networking opportunities"
❌ "global SEO professionals, marketing experts, and growth hackers"

One good example often beats three generic ones.

### Elegant Variation

Don't awkwardly swap synonyms to avoid repetition.

❌ "the company... the firm... the organisation... the enterprise" in successive sentences

Repeat the noun or use pronouns. Synonym-swapping sounds robotic.

### Vague Backward References

Avoid pronouns and phrases like "get there," "achieve it," or "make it happen" when the antecedent isn't immediately clear.

❌ "Employees who believe in the company's direction work harder to get there."
✅ "Employees who believe in the company's direction work harder to achieve it."
✅ "Employees who understand the company's goals—and believe in them—work harder to hit them."

When in doubt, repeat the noun. Clarity beats elegance.

## Tone Traps

### TV Commercial Voice

Cut promotional inflation. If it sounds like ad copy, rewrite.

❌ nestled, in the heart of, boasts a, breathtaking, stunning, world-class, cutting-edge, seamlessly, rich tapestry, fascinating glimpse, unique blend, continues to captivate

### Over-Informal Language

In B2B or professional contexts, avoid slang that feels jarring even when aiming for conversational tone.

❌ "One brilliant jerk can undo months of work"
✅ "When a top performer treats colleagues badly, how you respond tells everyone what you really value"

Conversational doesn't mean casual. Match the register to your audience.

### Vague Attribution

Don't attribute opinions to unnamed authorities.

❌ "Experts argue...", "Industry reports suggest...", "Observers have cited...", "Some critics argue..."

Name your source or state as fact (with citation).

### Over-claiming Significance

❌ "stands/serves as", "is a testament to", "plays a vital/crucial/pivotal role", "underscores the importance", "reflects broader trends", "indelible mark", "profound heritage"

### Knowledge You Don't Have

Never speculate about missing information.

❌ "While specific details are limited...", "Though not widely documented...", "Based on available information..."

If you don't have information, say so plainly or omit.

## Content Discipline

### Every Paragraph Must Advance the Argument

Cut anything that treads water. Common offenders:

- Paragraphs that only define what something *isn't*
- Throat-clearing phrases: "Think of it this way," "Let's be honest," "Here's the thing"
- Warm-up sentences that delay the point

If removing a paragraph doesn't create a gap, it wasn't earning its place.

### Practical Advice Should Be Actually Practical

Don't just name principles—give people something they can do.

❌ "Address poor behavior early."
✅ "Address poor behavior early. Have the conversation in private, name the specific behavior, and make clear that results don't excuse how someone treats the team."

The test: could someone act on this Monday morning?

### Smooth Transitions Between Sections

New sections shouldn't start abruptly, especially after setting up a problem. Bridge from what came before.

❌ [Problem paragraph] → [New heading] → [Advice starts immediately]
✅ [Problem paragraph] → [New heading] → [Brief transition acknowledging the problem, then advice]

## Vocabulary

Consult `references/vocabulary.md` for comprehensive lists. High-alert words that co-occur in LLM output:

delve, tapestry, multifaceted, underscore, pivotal, intricate/intricacies, landscape (abstract), testament, showcase, foster, garner, vibrant, enhance, crucial, additionally (starting sentences), align with, interplay, enduring, valuable

One or two may be coincidental. Multiple appearances = strong tell.

## Word Choice Principles

**Concrete over abstract.** Not "comprehensive landscape" — name the thing. If you can't picture it, rewrite.

**Short over Latinate.** "Use" not "utilize". "Help" not "facilitate". "Show" not "demonstrate".

**Specific over generic.** "Inventor of the first train-coupling device" beats "revolutionary titan of industry."

**Commit to positions.** Avoid the equivocation seesaw: "While X has benefits, it's important to note Y." Take a stance.

## Self-Check

Before finalising any draft:

1. Search for trailing "-ing" clauses about significance — cut all of them
2. Search for "pivot", "crucial", "vital", "testament", "underscore", "tapestry", "landscape", "foster", "delve" — rewrite or cut
3. Count triads — break most of them
4. Check for "Despite... challenges" formula
5. Check for false ranges ("from X to Y")
6. Check for vague attributions ("experts say", "some argue")
7. Check for false contrasts ("you don't need X, you need Y")
8. Check for vague backward references — repeat the noun if unclear
9. Verify every paragraph advances the argument
10. Read aloud: does it sound like a person or a brochure?

## Detailed Reference

See `references/vocabulary.md` for complete word lists organised by category.
See `references/structural-tells.md` for detailed examples of each pattern with before/after comparisons.
