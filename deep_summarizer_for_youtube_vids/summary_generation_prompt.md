You are helping me create a high-fidelity knowledge capture from a YouTube video.

Input:
- YouTube link: <PASTE_LINK>
- Transcript or detailed notes: <PASTE_TRANSCRIPT_OR_NOTES>

Your task:
Create a dense, accurate, nuance-preserving summary of the video. Do not give a generic recap. Preserve the author’s reasoning, edge cases, tradeoffs, examples, implied assumptions, and practical implications.

Requirements:
- Do not flatten nuance into motivational fluff
- Do not omit caveats, disagreements, limitations, or uncertainty
- Distinguish clearly between:
  - core thesis
  - supporting arguments
  - examples
  - actionable advice
  - speculation / opinion
- Preserve important terminology and definitions
- Capture memorable examples, analogies, and frameworks
- Include implementation-relevant details where present
- If the speaker changes their mind, qualifies a claim, or introduces a subtle distinction, include it
- If some parts are unclear or weakly supported, explicitly mark them as uncertain
- Do not invent anything not grounded in the input

Output format in Markdown:

# Source Capture

## Metadata
- Title:
- Link:
- Speaker / Channel:
- Date if known:
- Topic areas:
- Why this matters:

## Main Thesis
Write 1–3 paragraphs explaining the central point with precision.

## Detailed Summary
Write a detailed structured summary of the content.
Break it into logical sections based on ideas, not just chronology.
For each section include:
- the claim or idea
- why it matters
- the reasoning behind it
- nuances / caveats / exceptions
- any concrete examples used

## Nuanced Insights
List the non-obvious insights, subtle distinctions, tradeoffs, and deeper observations.
These should be the parts most people would miss in a shallow summary.

## Memorable Examples and Analogies
Capture the examples, stories, metaphors, and comparisons that make the ideas stick.

## Actionable Ideas
List practical takeaways, tactics, workflows, heuristics, or decisions someone could apply.

## Claims Requiring Caution
List anything that sounds speculative, context-dependent, weakly evidenced, or likely to be misunderstood.

## Terms and Concepts Mentioned
List important terms, frameworks, tools, or named ideas with one-line explanations.

## Open Questions
List questions, unresolved tensions, or follow-up areas worth exploring.

## Reusable Notes for Knowledge System
Write 5–15 atomic note candidates in the form:
- Note title:
- Type: concept / project / source-derived insight
- One-paragraph content:
- Suggested tags:
- Possible links to other notes:

## Condensed Source Packet
End with a compact but information-dense section that can be pasted into another agent for repository updates. Format it exactly as:

### SOURCE_PACKET
Title:
Link:
Source Type: YouTube
Primary Themes:
Summary:
Key Insights:
Examples:
Actionable Ideas:
Terms:
Open Questions:
Potential Note Targets:
Suggested Tags:
###