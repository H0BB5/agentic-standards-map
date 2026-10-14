# Declaration of AI use for this map

- **Tools.** Claude (Anthropic), used through claude.ai and Claude Code, for drafting entries under the author's direction, editing, source retrieval and checking quotes, dates and states against the sources; Claude in separate sessions, ChatGPT (OpenAI) and Perplexity as adversarial reviewers, with outputs retained.
- **Uses** (STM categories): writing or drafting content; refinement and editing of text; assisting with gathering references. Not in the STM list: checking quotes and dates against the sources; adversarial review.
- **Parts concerned:** all entries, seams, appendices and the calendar. The introduction and the README were drafted with assistance and revised by the author.
- **Who directed the work:** the author, who chose the scope and the rules, decided every change and checked every statement against its source.
- **As of:** 2026-10-14.
- **Version covered:** version 1.0; `map-bundle.md` at tag v1.0.0, sha256 ec30d2ee7f3961b8cad357604652109c8a4b1df4aa726350174c9c043694a594.
- **Record:** drafts, prompts, research outputs, reviews and the change log, retained by the author.
- No pass to remove traces of machine assistance was applied to this text.

The same declaration in a machine-readable form follows. It is illustrative, not a specification: field names and structure are not proposed as a standard.

```json
{
  "illustrative_only": true,
  "work": {
    "title": "Agentic Standards Map",
    "version": { "file": "map-bundle.md", "sha256": "ec30d2ee7f3961b8cad357604652109c8a4b1df4aa726350174c9c043694a594", "tag": "v1.0.0" }
  },
  "as_of": "2026-10-14",
  "tools": [
    { "name": "Claude", "provider": "Anthropic", "interfaces": ["claude.ai", "Claude Code"] },
    { "name": "ChatGPT", "provider": "OpenAI" },
    { "name": "Perplexity", "provider": "Perplexity AI" }
  ],
  "uses": [
    { "category": "Writing or drafting content", "tools": ["Claude"], "parts": "all entries, seams, appendices and the calendar; the introduction and the README drafted with assistance and revised by the author", "directed_by": "author" },
    { "category": "Refinement and editing of text", "tools": ["Claude"], "parts": "all entries, seams, appendices and the calendar; the introduction and the README", "directed_by": "author" },
    { "category": "Assisting with gathering references", "tools": ["Claude"], "parts": "all entries and appendices", "directed_by": "author" },
    { "category": "Checking quotes and dates against the sources (not in the STM list)", "tools": ["Claude"], "parts": "all entries and appendices", "directed_by": "author" },
    { "category": "Adversarial review (not in the STM list)", "tools": ["Claude", "ChatGPT", "Perplexity"], "parts": "all entries, seams, appendices and the calendar", "directed_by": "author" }
  ],
  "not_done": [
    "No pass to remove traces of machine assistance was applied to this text."
  ],
  "record": {
    "held_by": "author",
    "contents": ["drafts", "prompts", "research outputs", "reviews", "change log"],
    "access": "on request, as far as needed"
  },
  "categories_source": "STM, Recommendations for a Classification of AI Use in Academic Manuscript Preparation, September 2025"
}
```
