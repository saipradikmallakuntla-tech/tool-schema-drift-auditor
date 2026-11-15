# Tool Schema Drift Auditor

A standalone Batch 99 browser utility for conservative **version-to-version input-schema drift**, not provider dialect portability. **Live:** https://saipradikmallakuntla-tech.github.io/tool-schema-drift-auditor/

Open `index.html` or run `python3 -m http.server 8000`. Paste previous/current JSON Schema objects or booleans for the same tool. Common `{name, parameters}` and `{type: "function", function: {name, parameters}}` wrappers are accepted. Load one of three synthetic examples, audit, review findings, and optionally export JSON. The interface is English-only.

## Model and boundaries
The direction is old accepted inputs toward new acceptance. Models types (including integer-to-number widening), required additions/removals, scalar enums, numeric/string/array bounds, nested properties, simple items and boolean additionalProperties. Reports potentially breaking, widening, review and annotation findings. Optional properties are conservatively reviewed because they may constrain formerly unrestricted unknown inputs. Reports do not claim compatibility.

**Not a full JSON Schema validator or payload validator.** No provider support profiles, output-schema guarantees, semantic equivalence, reference resolution or code execution. Unsupported keywords, composition, tuple items and schema-valued additionalProperties require manual review even when unchanged. Nonempty scalar enums only. Bounds: 100,000 code units per JSON text, 16 modeled levels, 2,000 nodes per side, 5,000 findings. Malformed or out-of-range modeled declarations are rejected; complex unsupported semantics still need a real dialect-aware validator and caller tests.

No uploads, APIs, telemetry, cookies, persistence, packages or external assets. All output uses text rendering. Exports omit input schemas but retain tool names and property paths: review metadata before sharing and never paste secrets. This tool is distinct from the historical unlaunched Structured Output Portability Checker proposal.

## Tests and deployment
`timeout 15s node --check app.js`

`timeout 15s node tests/test.cjs`

Twelve built-in synthetic assertions plus Node fixture/invalid-input checks. Publish `main:/` with `.nojekyll` and enforced HTTPS; no custom domain.

## Seven-node network
- [Hub](https://saipradikmallakuntla-tech.github.io/zion-ai-apps-hub/)
- [Stream Inspector](https://saipradikmallakuntla-tech.github.io/llm-stream-inspector/)
- [Retry Safety Lab](https://saipradikmallakuntla-tech.github.io/agent-retry-safety-lab/)
- [CORS Doctor](https://saipradikmallakuntla-tech.github.io/cors-cookie-doctor/)
- [Token Budget Lab](https://saipradikmallakuntla-tech.github.io/prompt-token-budget-lab/)
- [Webhook Replay Guard](https://saipradikmallakuntla-tech.github.io/webhook-replay-guard/)

[Discovery EN](https://saipradikmallakuntla-tech.github.io/zion-ai-apps-hub/batch-99-discovery.html) · [ES](https://saipradikmallakuntla-tech.github.io/zion-ai-apps-hub/es/batch-99-discovery.html) · [PT](https://saipradikmallakuntla-tech.github.io/zion-ai-apps-hub/pt/batch-99-discovery.html). [Network contract](NETWORK.md). Navigation carries no input.
