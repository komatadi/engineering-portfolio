# Technical Evidence Map

This page maps common technical interview questions to concrete examples from the case studies in this portfolio.

| Interview topic | Evidence |
|---|---|
| **How do you design an agentic system?** | Agentic Commerce: intent/routing layer, deterministic vs. agentic modes, explicit tools, state, iteration/time limits |
| **What does RAG actually do in your architecture?** | Customer-service flow: chunked source content → embeddings/vector retrieval → grounded context → model response |
| **Why not use an agent for everything?** | Catalog architecture deliberately uses deterministic execution for predictable, high-frequency discovery and reserves agent loops for complex reasoning |
| **How do you prevent hallucinations?** | Grounding in authoritative product/policy sources, structured contracts, confidence/fallback behavior, explicit tools for operational actions |
| **How do embeddings fit into the system?** | Semantic product discovery and policy retrieval use vector representations to find context before model generation |
| **How do tools/actions work?** | Calendar/API calls, product retrieval and support persistence remain explicit operations with typed inputs and failure handling |
| **How do you manage state?** | Agent session context, structured multi-step consultation state, run-scoped game state and durable person identity are intentionally separated |
| **What is your security model?** | Group Games: authentication ≠ identity ≠ authorization; server-side checks, RLS/RPCs, least-privilege credentials and explicit privileged services |
| **How do you think about platform architecture?** | Group Games: Platform / Shared Runtime / Game ownership model and second-consumer rule for reusable abstractions |
| **How do you evolve an architecture safely?** | Additive migrations, compatibility, architecture decisions and regression gates instead of broad rewrites |
| **How do you handle real data safely?** | Personal Finance: immutable source evidence, household RLS, private storage, deterministic parsing and repository sensitive-file protection |
| **How do you ensure an import is idempotent?** | Source hashes + semantic duplicate/conflict handling + canonical lineage |
| **Where should AI not be used?** | Financial monetary facts, dates, identities and event existence remain deterministic and authoritative |
| **How do you run CI around database changes?** | Disposable database reset, migration verification, RLS/integrity tests, generated-type equivalence and explicit hosted deployment |
| **How do you handle runtime/integration complexity?** | Store Operations: admin vs. storefront proxy boundaries, platform extensions, environment-specific workflows and predeploy validation |
| **Are you personally coding all of this?** | I use coding agents extensively. I personally own the architecture, contracts, prototypes, key technical choices, reviews, debugging, verification and acceptance. The goal is informed technical leadership, not claiming every line was manually authored by me. |

## My definition of hands-on

For a senior architect / technology leader, I consider “hands-on” to mean being able to:

1. decompose the problem into implementable components;
2. explain the runtime behavior of each important component;
3. prototype critical paths where learning is needed;
4. read and challenge implementation decisions;
5. debug across component boundaries;
6. understand security, data and operational consequences;
7. define acceptance and verification;
8. know when a framework or abstraction is adding unnecessary complexity; and
9. lead specialist engineers without becoming disconnected from the technology.

That is the technical standard these projects are intended to demonstrate.
