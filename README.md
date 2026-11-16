# Awesome System Verification [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of frameworks, methodologies, tools, talks and papers for **System Verification Engineering (SVE)**: proving that software, AI agents and autonomous systems do what they should, and nothing they should not.

Code is abundant; confidence is scarce. As AI agents write code, call tools and act in production, verification becomes the layer that lets teams move fast safely.

Maintained by [Carver Agents](https://carveragents.ai) and [Testfold](https://testfold.ai).

## Contents

- [Foundations and Manifestos](#foundations-and-manifestos)
- [Formal Methods and Specification](#formal-methods-and-specification)
- [Model Checking and Theorem Proving](#model-checking-and-theorem-proving)
- [Property-Based and Generative Testing](#property-based-and-generative-testing)
- [Fuzzing](#fuzzing)
- [Deterministic Simulation Testing](#deterministic-simulation-testing)
- [Distributed Systems Verification](#distributed-systems-verification)
- [Contract and API Verification](#contract-and-api-verification)
- [Mutation Testing](#mutation-testing)
- [Runtime Verification and Observability](#runtime-verification-and-observability)
- [AI Agent Evaluation and Verification](#ai-agent-evaluation-and-verification)
- [AI Agent Security and Guardrails](#ai-agent-security-and-guardrails)
- [Verifying AI-Generated Code](#verifying-ai-generated-code)
- [Regulatory and Compliance Verification](#regulatory-and-compliance-verification)
- [Safety-Critical Systems](#safety-critical-systems)
- [Talks and Presentations](#talks-and-presentations)
- [Books](#books)
- [Courses](#courses)
- [Contributing](#contributing)

## Foundations and Manifestos

- [The Lethal Trifecta for AI Agents](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/) - Simon Willison on private data + untrusted content + external communication.
- [Prompt Injection series](https://simonwillison.net/series/prompt-injection/) - Simon Willison's running catalog of agent attack patterns.
- [How Amazon Web Services Uses Formal Methods](https://cacm.acm.org/research/how-amazon-web-services-uses-formal-methods/) - CACM paper on TLA+ at AWS.
- [Use of Formal Methods at Amazon Web Services](https://lamport.azurewebsites.net/tla/formal-methods-amazon.pdf) - Original AWS formal methods report (PDF).
- [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) - Anthropic on agent architectures and where checks belong.
- [Hillel Wayne's blog](https://www.hillelwayne.com/) - Practical essays on formal methods and testing.

## Formal Methods and Specification

- [TLA+](https://lamport.azurewebsites.net/tla/tla.html) - Leslie Lamport's specification language for concurrent and distributed systems.
- [Learn TLA+](https://learntla.com/) - Hillel Wayne's practical TLA+ guide.
- [P Language](https://github.com/p-org/P) - Formal modeling language for distributed systems, used at AWS.
- [Alloy](https://alloytools.org/) - Lightweight formal modeling and analysis.
- [Dafny](https://dafny.org/) - Verification-aware programming language.
- [Quint](https://github.com/informalsystems/quint) - Modern, developer-friendly specification language built on TLA.
- [Z3](https://github.com/Z3Prover/z3) - Microsoft Research SMT solver behind many verification tools.
- [Kani](https://github.com/model-checking/kani) - Bit-precise model checker for Rust.
- [Verus](https://github.com/verus-lang/verus) - Verified Rust for systems code.
- [Prusti](https://github.com/viperproject/prusti-dev) - Static verifier for Rust.
- [Frama-C](https://frama-c.com/) - Analysis and verification platform for C.
- [SPARK](https://www.adacore.com/about-spark) - Formally verifiable subset of Ada.

## Model Checking and Theorem Proving

- [Lean](https://lean-lang.org/) - Theorem prover and programming language.
- [Coq / Rocq](https://rocq-prover.org/) - Interactive theorem prover.
- [Isabelle](https://isabelle.in.tum.de/) - Generic proof assistant.
- [CBMC](https://github.com/diffblue/cbmc) - Bounded model checker for C/C++.
- [SPIN](https://spinroot.com/) - Model checker for concurrent software.
- [seL4](https://sel4.systems/) - Formally verified microkernel.
- [CompCert](https://compcert.org/) - Formally verified C compiler.

## Property-Based and Generative Testing

- [Hypothesis](https://github.com/HypothesisWorks/hypothesis) - Property-based testing for Python.
- [QuickCheck](https://hackage.haskell.org/package/QuickCheck) - The original property-based testing library (Haskell).
- [fast-check](https://github.com/dubzzz/fast-check) - Property-based testing for JavaScript/TypeScript.
- [proptest](https://github.com/proptest-rs/proptest) - Property-based testing for Rust.
- [jqwik](https://jqwik.net/) - Property-based testing on the JVM.

## Fuzzing

- [AFL++](https://github.com/AFLplusplus/AFLplusplus) - Community-maintained fuzzer.
- [libFuzzer](https://llvm.org/docs/LibFuzzer.html) - In-process, coverage-guided fuzzing.
- [OSS-Fuzz](https://github.com/google/oss-fuzz) - Continuous fuzzing for open source.
- [The Fuzzing Book](https://www.fuzzingbook.org/) - Free interactive textbook.
- [RESTler](https://github.com/microsoft/restler-fuzzer) - Stateful REST API fuzzer.

## Deterministic Simulation Testing

- [Antithesis](https://antithesis.com/) - Autonomous deterministic simulation testing platform.
- [Testing Distributed Systems w/ Deterministic Simulation](https://www.youtube.com/watch?v=4fFDFbi3toc) - Will Wilson's classic FoundationDB talk (Strange Loop).
- [TigerBeetle VOPR](https://github.com/tigerbeetle/tigerbeetle) - Simulation-tested financial database.
- [madsim](https://github.com/madsim-rs/madsim) - Deterministic simulator for Rust distributed systems.

## Distributed Systems Verification

- [Jepsen](https://jepsen.io/) - Kyle Kingsbury's analyses of distributed databases.
- [Jepsen library](https://github.com/jepsen-io/jepsen) - Framework for distributed systems testing.
- [Elle](https://github.com/jepsen-io/elle) - Black-box transactional consistency checker.
- [Maelstrom](https://github.com/jepsen-io/maelstrom) - Workbench for learning distributed systems via verification.
- [Chaos Mesh](https://chaos-mesh.org/) - Chaos engineering for Kubernetes.
- [Principles of Chaos Engineering](https://principlesofchaos.org/) - The chaos engineering manifesto.

## Contract and API Verification

- [Pact](https://pact.io/) - Consumer-driven contract testing.
- [Schemathesis](https://github.com/schemathesis/schemathesis) - Property-based testing from OpenAPI/GraphQL schemas.
- [Dredd](https://github.com/apiaryio/dredd) - HTTP API testing against descriptions.
- [Pydantic](https://docs.pydantic.dev/) - Runtime data validation, widely used for agent tool I/O.

## Mutation Testing

- [Stryker Mutator](https://stryker-mutator.io/) - Mutation testing for JS, C#, Scala.
- [PIT](https://pitest.org/) - Mutation testing for Java.
- [mutmut](https://github.com/boxed/mutmut) - Mutation testing for Python.
- [cargo-mutants](https://github.com/sourcefrog/cargo-mutants) - Mutation testing for Rust.

## Runtime Verification and Observability

- [OpenTelemetry](https://opentelemetry.io/) - Vendor-neutral traces, metrics and logs.
- [OpenTelemetry GenAI semantic conventions](https://opentelemetry.io/docs/specs/semconv/gen-ai/) - Standard telemetry for LLM and agent calls.
- [Open Policy Agent](https://www.openpolicyagent.org/) - Policy-as-code engine for runtime authorization.
- [Cedar](https://www.cedarpolicy.com/) - Verifiable authorization policy language from AWS.
- [Langfuse](https://github.com/langfuse/langfuse) - Open source LLM tracing and evals.
- [Arize Phoenix](https://github.com/Arize-ai/phoenix) - LLM observability and evaluation.

## AI Agent Evaluation and Verification

- [Inspect](https://inspect.aisi.org.uk/) - UK AISI framework for LLM and agent evaluations.
- [OpenAI Evals](https://github.com/openai/evals) - Framework and registry of LLM evals.
- [promptfoo](https://github.com/promptfoo/promptfoo) - Test and red-team LLM apps.
- [DeepEval](https://github.com/confident-ai/deepeval) - Unit-test style LLM evaluation.
- [Ragas](https://github.com/explodinggradients/ragas) - Evaluation for RAG pipelines.
- [SWE-bench](https://www.swebench.com/) - Benchmark for coding agents on real GitHub issues.
- [tau-bench](https://github.com/sierra-research/tau-bench) - Tool-agent-user interaction benchmark.
- [Terminal-Bench](https://www.tbench.ai/) - Benchmark for agents in terminal environments.
- [Demystifying evals for AI agents](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents) - Anthropic engineering guide.

## AI Agent Security and Guardrails

- [OWASP Top 10 for LLM Applications](https://genai.owasp.org/llm-top-10/) - Canonical LLM risk list.
- [MITRE ATLAS](https://atlas.mitre.org/) - Adversarial threat landscape for AI systems.
- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) - Programmable guardrails for LLM apps.
- [Guardrails AI](https://github.com/guardrails-ai/guardrails) - Input/output validation for LLMs.
- [garak](https://github.com/NVIDIA/garak) - LLM vulnerability scanner.
- [PyRIT](https://github.com/Azure/PyRIT) - Microsoft's red-teaming toolkit for generative AI.
- [CaMeL: Defeating Prompt Injections by Design](https://arxiv.org/abs/2503.18813) - Google DeepMind capability-based agent security.
- [Model Context Protocol](https://modelcontextprotocol.io/) - Standard for agent-tool connections, including authorization.

## Verifying AI-Generated Code

- [SonarQube](https://www.sonarsource.com/products/sonarqube/) - Static analysis and code quality gates.
- [Semgrep](https://github.com/semgrep/semgrep) - Lightweight static analysis with custom rules.
- [CodeQL](https://codeql.github.com/) - Semantic code analysis engine.
- [Testfold](https://testfold.ai) - Verification-first testing for AI-built software.
- [Software Engineering at Google: Testing](https://abseil.io/resources/swe-book/html/ch11.html) - Free book chapters on testing at scale.

## Regulatory and Compliance Verification

- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) - US framework for AI risk.
- [EU AI Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) - Official text of Regulation (EU) 2024/1689.
- [ISO/IEC 42001](https://www.iso.org/standard/81230.html) - AI management system standard.
- [OSCAL](https://pages.nist.gov/OSCAL/) - NIST machine-readable control and assessment language.
- [Carver Agents](https://carveragents.ai) - Regulatory obligations as executable controls for agents.
- [Is My Agent Legal?](https://ismyagentlegal.com) - Free check of an agent description against obligations across jurisdictions.

## Safety-Critical Systems

- [DO-178C overview](https://en.wikipedia.org/wiki/DO-178C) - Avionics software assurance standard.
- [ISO 26262](https://www.iso.org/standard/68383.html) - Automotive functional safety.
- [UL 4600](https://ul.org/research-updates/ul-4600-standard-safety-evaluation-autonomous-products/) - Safety standard for autonomous products.
- [NASA Software Engineering Handbook](https://swehb.nasa.gov/) - NASA's verification and validation practices.
- [Engineering a Safer World (STAMP/STPA)](https://mitpress.mit.edu/9780262533690/engineering-a-safer-world/) - Nancy Leveson's systems safety approach.

## Talks and Presentations

- [AI Engineer YouTube channel](https://www.youtube.com/@aiDotEngineer) - Keynotes on agents, evals and software factories (Two Sigma, Sonar, Keycard, Ramp, Modal, Cognition, Capital One and more).
- [Strange Loop archive](https://www.youtube.com/@StrangeLoopConf) - Many classic testing and verification talks.
- [Jepsen talks](https://jepsen.io/talks) - Kyle Kingsbury's conference talks.
- [Leslie Lamport: Thinking Above the Code](https://www.youtube.com/watch?v=-4Yp3j_jk8Q) - Why specify before you code.
- [John Hughes: Testing the Hard Stuff and Staying Sane](https://www.youtube.com/watch?v=zi0rHwfiX1Q) - Property-based testing in industry.

## Books

- *Practical TLA+* - Hillel Wayne.
- *Specifying Systems* - [Leslie Lamport (free PDF)](https://lamport.azurewebsites.net/tla/book.html).
- *Software Foundations* - [Free online series](https://softwarefoundations.cis.upenn.edu/).
- *Property-Based Testing with PropEr, Erlang, and Elixir* - Fred Hebert.
- *Chaos Engineering* - Casey Rosenthal and Nora Jones.
- *Engineering a Safer World* - Nancy Leveson.

## Courses

- [Software Foundations](https://softwarefoundations.cis.upenn.edu/) - Logic, proofs and verified programs in Coq/Rocq.
- [Functional Programming in Lean](https://lean-lang.org/functional_programming_in_lean/) - Free Lean book.
- [The Fuzzing Book](https://www.fuzzingbook.org/) - Interactive fuzzing course.

## Contributing

Contributions welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) first.

## Maintainers

- [Carver Agents](https://carveragents.ai) - Regulatory intelligence and executable compliance for AI agents.
- [Testfold](https://testfold.ai) - Verification-first software development.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
