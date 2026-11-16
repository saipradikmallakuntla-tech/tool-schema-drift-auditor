> **Current seven-repository documentation map — 2026-11-16 UTC · CAT-v1**  
> **Primary category:** `LLM-SCHEMA` — AI/LLM → Input-Contract Drift.  
> [Canonical Category Index and Directory](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/CATEGORY_INDEX_AND_DIRECTORY.md) · [Seven-node registry](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/NETWORK.md) · [Portfolio status](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/PORTFOLIO_STATUS.md) · [Locale/review register](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/TRANSLATION_PARITY_REGISTER.md).  
> This owner-approved documentation map covers seven existing owned repositories: one hub and six utilities. Earlier scope statements/counts below are retained dated batch history. Current written coverage is **79 IDs / 237 locale entries total**, not approvals or apps; 48 pre-existing Markdown files plus the new index give 49 files. Category labels classify documentation, not website filters or software. Satellite interfaces remain English-only; human language/domain, receiver and channel decisions remain pending. No code, tests, byte-hash scripts, live checks, external distribution or automatic integration is introduced.

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

## Batch-99 documentation reconciliation — 2026-11-16 UTC

Batch: `zion-batch-99-portfolio-reconciliation-2026-11-16-en-es-pt`. This repository already existed; this cycle changes only README.md and NETWORK.md. The original body above is retained as dated documentary context, including commands that are not executed here. This is not a new app launch, software localization or deployment verification.

Catalog B99-C02 and routing B99-R01: [English](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/BATCH_99_CATALOG_ROUTING_GUIDE.md#en) · [Español neutro](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/BATCH_99_CATALOG_ROUTING_GUIDE.md#es) · [Português](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/BATCH_99_CATALOG_ROUTING_GUIDE.md#pt). Conservative version-to-version input-schema findings are not full validation, provider portability or compatibility certification. The interface remains documented as English-only.

Current reciprocal documentation is in the [dated local network appendix](NETWORK.md), with all six peer README destinations. Use the single [central portfolio/status and evidence register](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/PORTFOLIO_STATUS.md) and [locale-review register](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/TRANSLATION_PARITY_REGISTER.md); no competing local status file is added. Seven nodes/six utilities/42 possible directed relationships describe documentation, not verified live integration. Human language/domain, receiver and channel decisions remain pending. No sensitive inputs in links, automatic handoff, code/test/hash/browser/live-probe work, Pages/DNS change, Notion/further Mem0 call or external distribution.


## Saved handoff and free discovery — 2026-11-16 UTC

Batch: `zion-saved-handoff-discovery-2026-11-16-en-es-pt`. The complete earlier body is retained; this dated appendix is the newer editorial view, not a software change.

[Saved Handoff Playbooks and Discovery Promos — English](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/SAVED_HANDOFF_PLAYBOOKS_AND_DISCOVERY_PROMOS.md#en) · [Español neutro](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/SAVED_HANDOFF_PLAYBOOKS_AND_DISCOVERY_PROMOS.md#es) · [Português](https://github.com/saipradikmallakuntla-tech/zion-ai-apps-hub/blob/main/SAVED_HANDOFF_PLAYBOOKS_AND_DISCOVERY_PROMOS.md#pt). SH01–SH06 cover free self-serve discovery, seven-node routing, a manually saved private Markdown packet, actual receiver acknowledgment, optional human team/commercial scoping and reusable promotion drafts. The guide links back to this [README](README.md) and [NETWORK](NETWORK.md); existing six-peer pointers remain intact.

Schema findings remain conservative version-to-version input-contract observations, not full validation, compatibility certification or provider portability. Record only a synthetic or explicitly permitted minimum summary with source revision, uncertainty and next owner. Saved means manual documentation, not app persistence, synchronization, automatic email or replay permission. Team/commercial discussion requires verified people and separate scope/terms; no available service, price or SLA is promised.

The package's current written inventory is 51 Markdown files and 85 logical IDs/255 pending-review EN/ES/PT entries; older counts above remain dated history. These pointers repeat SH sources and add no translated IDs. All six utility interfaces remain English-only. Human language/domain, receiver and channel decisions remain pending; external distribution stays on hold. No private receipts or diagnostic inputs in public links. No code/HTML/test/runtime/Pages/DNS edits, test/hash/browser/live-probe scripts or further Mem0 calls.
