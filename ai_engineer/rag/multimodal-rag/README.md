# Multimodal RAG

Retrieval over mixed content types — dashboards, architecture diagrams,
and screenshots — not just chunked text.

## Why this matters
A lot of real operational and product knowledge lives in images (a
Grafana panel screenshot, an architecture diagram in a wiki) that a
text-only pipeline never sees. This is the most exploratory, least
solved topic in this repo — kept honest as a placeholder rather than
faked.

## Key concepts
- Joint text-image embedding models (e.g. CLIP-style) for cross-modal
  search
- Image captioning as a bridge into a text-only retrieval pipeline
- Chart/graph data extraction — genuinely hard; often better solved by
  pulling raw data from the source system than parsing rendered images
- Fusion ranking — combining text-chunk and image-embedding results into
  one ranked context

## Planned contents
- `image_embed.py`, `chart_parser.py`, `fusion_retriever.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — genuinely unsolved/exploratory, code
coming progressively.
