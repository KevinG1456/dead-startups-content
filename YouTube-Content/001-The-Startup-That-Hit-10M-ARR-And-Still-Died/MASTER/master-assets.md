# Master Assets — Sprig

Assets to build once and reuse across all six language cuts. Do not recreate identical visual
assets six times — only text overlays and voice/subtitle tracks are language-specific.

## Shared, Reusable Across All 6 Languages
- Revenue-vs-loss contrast graphic (numeral overlay swaps per language)
- Funding timeline graphic (label overlay swaps per language)
- "Who bears the cost" diagram (label overlay swaps per language)
- Growth-rate flip graph (label overlay swaps per language)
- Shutdown/headcount distinction graphic (label overlay swaps per language)
- Autopsy Report Card end-graphic template (label overlay swaps per language)
- All generic B-roll/stock footage (kitchen, delivery-bag, laptop/dashboard imagery)
- All AI-generated background/illustration/infographic images from `../ai-image-prompts.md`
  (none render real text, so none need regeneration per language)
- Thumbnail base composition/imagery (see `master-thumbnail.md` — only text layer changes)

## Language-Specific, Must Be Created Per Language
- Voice narration (HeyGen Avatar V, localized script)
- Subtitle track
- On-screen quote-card text (translated, not just the graphic frame)
- Lower-third labels and chapter titles
- Thumbnail text layer (composition/imagery shared, text localized)
- Title, description, tags, hashtags, SEO keywords
- Shorts, community posts, social copy

## Production Note
Build the shared graphics ONCE at a resolution/format that supports text-layer swaps in the
editor (e.g., text on a separate layer/track from the base graphic), so localizing for a new
language is a text-swap task, not a re-render task.
