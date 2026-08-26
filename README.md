# Agent-Robber-Reserch


THE ROBBER AGENT: A NATIVE, ZERO-OVERHEAD, HYBRID-INTERFACE AUTONOMOUS SOFTWARE ENGINEERING & BROWSER AUTOMATION SYSTEM
Abstract
The Robber Agent is a next-generation, local-first autonomous software development and web automation framework engineered to bridge the gap between heavyweight enterprise AI agents and lightweight developer tooling. Operating on a Bring-Your-Own-Key (BYOK) zero-cost model, the system decouples high-level reasoning from local resource consumption. It unifies multi-model API consensus, a Single Source of Truth (SSOT) vector memory architecture, non-blocking asynchronous sub-agent execution, and computer-vision-driven humanlike web automation into a single lightweight platform.

Designed to execute seamlessly on constrained hardware environments (e.g., Intel Core i5-4590, 8GB DDR3 RAM) without compromising speed or control, The Robber Agent eliminates heavy Docker containerization while maintaining a unified visual design language across both a Web Graphical User Interface (GUI) and a Terminal User Interface (CLI TUI).

1. System Overview & Core Mission (What It Does)
The Robber Agent acts as an autonomous pair-programmer, terminal operator, and web navigation engine. Unlike traditional coding assistants that merely generate code snippets or execute isolated terminal commands, The Robber Agent autonomously plans, executes, validates, and self-heals multi-step software engineering tasks across entire repository trees.

Primary Operational Domains
Autonomous End-to-End Software Engineering: Writes code, executes build pipelines, diagnoses runtime exceptions (stderr), and applies surgicalAbstract Syntax Tree (AST) patches autonomously.


Humanlike Web & Third-Party App Automation: Controls websites and web applications without relying on public APIs by mimicking human interaction mechanics (Bézier mouse trajectories, natural typing cadences, vision-based DOM element mapping).


Cross-Model Orchestration: Simultaneously coordinates specialized cloud-native models (e.g., Gemini 2.0/Pro, DeepSeek R1, Groq Llama 3.3, OX Alpha on OpenCode) to achieve consensus on complex architectural decisions.


Context-Aware System Administration: Manages background terminal tasks, provisions environment dependencies (pip, npm, apt), and isolates experimental changes using Git worktree shields.


2. Architectural Paradigm & Operational Mechanics (How It Works)
The architecture of The Robber Agent relies on a decoupled, event-driven Python FastAPI daemon paired with a local vector engine and an asynchronous subprocess worker manager.

+-----------------------------------------------------------------------------------+
|                                THE ROBBER AGENT                                   |
+-----------------------------------------------------------------------------------+
|  HYBRID INTERFACE LAYER                                                           |
|  +----------------------------------+    +-------------------------------------+  |
|  | Web GUI (React / Tailwind Bento) |    | CLI TUI (Python Textual / Rich)     |  |
|  +----------------------------------+    +-------------------------------------+  |
+------------------------------------------+----------------------------------------+
                                           | Async WebSocket / REST
                                           v
+-----------------------------------------------------------------------------------+
|  BACKEND ORCHESTRATION DAEMON (FastAPI / Python)                                  |
|  +----------------------------------+    +-------------------------------------+  |
|  | SSOT Vector State (LanceDB)      |    | Dynamic Model Router (LiteLLM)      |  |
|  +----------------------------------+    +-------------------------------------+  |
|  | Tree-Sitter AST Patch Engine     |    | LSP Type-Checker & Validator        |  |
|  +----------------------------------+    +-------------------------------------+  |
+------------------------------------------+----------------------------------------+
                                           | Async Subprocesses
                                           v
+-----------------------------------------------------------------------------------+
|  AUTONOMOUS SUB-AGENTS                                                            |
|  +----------------------------------+    +-------------------------------------+  |
|  | Non-Blocking Terminal Sub-Agent  |    | Vision & Playwright Web Automator   |  |
|  | (Self-Healing Error Loop)        |    | (Bézier Trajectories & Anti-Bot)    |  |
|  +----------------------------------+    +-------------------------------------+  |
+-----------------------------------------------------------------------------------+


Key Subsystems
1. Single Source of Truth (SSOT) Live Memory Engine
The system uses an embedded, local-first vector database (LanceDB) to index project files, workspace state, environment logs, and developer preferences. Every connected AI model queries and writes to this unified state, eliminating context fragmentation across multi-model tasks.

2. Virtual Super-Model Consensus Engine
Instead of relying on a single LLM, the orchestrator splits complex tasks among multiple specialized models in parallel. For instance, DeepSeek R1 generates mathematical/logic trees, Gemini evaluates overall architecture, and Groq streams rapid syntax checks. The consensus engine deduplicates logic and synthesizes a single, optimal execution path.

3. Autonomous Non-Blocking AI Terminal Sub-Agent & Self-Healing Loop
Terminal command execution is offloaded to an asynchronous background worker. If a build or script fails:

The sub-agent captures the exact stderr stack trace.


It routes the error and surrounding AST context to a high-speed inference endpoint (e.g., Groq/Gemini).


It generates a corrective patch, applies it to disk, and re-executes the command automatically without blocking the main user interface.


4. Surgical AST Patching via Tree-Sitter
Rather than regenerating entire files—which wastes tokens and introduces regression bugs—The Robber Agent uses Tree-Sitter parsing to generate and apply unified line-by-line diff patches directly to specific code nodes.

5. Computer Vision & Humanlike Automation Mechanics
For third-party web interaction, the agent merges Playwright DOM trees with lightweight visual object-detection models. Actions are executed via human-simulated interaction curves (Bézier mouse movement, variable delay typing cadences, and session cookie persistence), bypassing anti-bot locks and API constraints.

3. Comparative Advantage & Superiority (How It Differs)
Existing autonomous agents suffer from critical architectural bottlenecks: they either demand expensive recurring subscriptions (Devin), require heavy, resource-draining Docker virtualization (OpenHands), or lock developers into monolithic Electron applications (Cursor).

The Robber Agent establishes a new standard by optimizing for extreme efficiency, hardware accessibility, and developer sovereignty.

Feature / Metric
The Robber Agent
Devin
OpenHands (OpenDevin)
Cursor / Windsurf
Aider CLI
Execution Architecture
Local Daemon + Hybrid GUI/TUI
Cloud Closed-SaaS
Heavy Docker Containers
Electron IDE Fork
CLI Terminal Only
Disk Footprint
~2.5 GB
N/A (Cloud)
~15.0 GB – 20.0 GB
~2.0 GB
~300 MB
Runtime RAM Usage
~1.1 GB – 1.3 GB
N/A (Cloud)
~4.0 GB – 8.0 GB
~1.8 GB – 2.5 GB
~200 MB
Cost Model
100% Free (BYOK)
~$500+/mo
API Usage + Cloud VPS
$20/mo Subscription
API Usage
Humanlike Web Automation
Native Vision + Playwright
Basic Web Browser
Experimental / Limited
None
None
Interface Flex
Dual Parity (GUI + TUI)
Web Dashboard
Web Dashboard
IDE GUI
CLI Terminal
AST Surgical Patching
Yes (Tree-Sitter)
Unknown
No (Whole File/Diff)
Yes
Yes (Diff)

4. Comprehensive Feature Specification Matrix
Core Architecture & Memory Systems
SSOT Live Memory Indexing: Local vector embeddings linking file systems, chat history, and runtime logs.


Virtual Super-Model Consensus Engine: Multi-model concurrent processing and logic deduplication.


Dynamic Power Throttling:



Eco Mode: Runs entirely offline via local Ollama instances.


Balanced Mode: Routes traffic through a single high-speed cloud API key.


Max Beast Mode: Executes parallel multi-model cloud consensus.


BYOK Zero-Cost Infrastructure: Native localhost connections eliminating proxy server latency and API markups.


Project Directive Enforcement: Strict adherence to workspace .rules, architectural patterns, and security constraints.


Process Safety & Execution Control
One-Click Process Purge (PID Killer): Immediate visual/terminal button to kill runaway processes, deadlocked build scripts, or infinite loops.


Hyperparameter Sliders: On-the-fly adjustment of Temperature, Top-P, Top-K, and Repetition Penalty per model node.


Token & Rate Limit Radar: Real-time visual tracking of Tokens Per Second (TPS), latency (ms), and free-tier API quotas.


Resource Throttler: Enforces strict memory and CPU boundaries to keep system usage below 1.5 GB RAM on host machines.


Interactive Slash Command Suite (/)
/fix: Pulls the latest terminal error stack trace, performs AST analysis, and applies an instant patch.


/clean: Flushes temporary build caches (node_modules, __pycache__) and optimizes the LanceDB index.


/compact: Summarizes active chat logs into dense vector embeddings without state loss.


/rollback: Reverts workspace files to their state prior to the last AI-generated patch using local Git AST history.


/mode [eco | balanced | beast]: Switches hardware and model execution strategies instantly.


/explain: Generates architectural breakdowns for targeted code blocks.


/test: Auto-generates and runs unit tests inside the background terminal sub-agent.


Vision & Web/App Automation Engine
Vision DOM Element Mapping: Uses object detection to locate UI elements, inputs, and buttons on web platforms.


Bézier Motion Trajectories: Simulates human mouse movements with organic acceleration and deceleration curves.


Typing Cadence Randomization: Introduces micro-delays between keystrokes to mimic human input.


Anti-Bot & Captcha Navigation: Detects interactive challenges, dynamic pop-ups, and rate limits without freezing the agent.


Session Vault: Securely stores local cookies, session tokens, and local storage states for authenticated cross-session workflows.


MCP Protocol Bridge: Native support for Model Context Protocol servers alongside direct browser automation.


Dual-Interface Parity (GUI & CLI TUI)
Visual Aesthetic: Dark Onyx (#0D0D10) theme with Warm Amber (#FF8C00) accents, Bento-grid layouts, and rounded card geometry.


Web Dashboard (React + Tailwind): Dense multi-panel workspace featuring live token radars, dual-pane prompt/thinking views, and interactive Playwright streams.


Terminal Interface (Python Textual/Rich): 1:1 visual parity CLI featuring identical Bento card borders, live streaming sub-agent outputs, and keyboard-first slash-command controls.

1. Multi-Model Orchestration & Core Intelligence
Virtual Super-Model Consensus Engine: Concurrently dispatches complex prompts to multiple specialized models (e.g., Gemini 2.0 Pro, DeepSeek R1, Groq Llama 3.3, OX Alpha on OpenCode). Synthesizes responses, removes duplicated logic, and outputs a single optimized execution plan.


Direct BYOK Zero-Cost Routing: Operates via a local native connection using personal API keys (Google AI Studio, Groq, OpenCode). Bypasses third-party proxy servers, markup costs, and artificial speed limits.


Dynamic Power Throttling Engine:



Eco Mode: Runs local processing via Ollama for offline work or hardware preservation.


Balanced Mode: Directs traffic through a single high-speed cloud API key for daily development tasks.


Max Beast Mode: Activates full parallel multi-model consensus across all configured cloud providers simultaneously.


Enforced Custom .rules Directives: Strictly enforces project-specific coding conventions, folder structures, design tokens, and architectural constraints across every generated patch.


2. Memory Architecture & Code Analysis
Single Source of Truth (SSOT) Live Memory Engine: Uses an embedded local vector database (LanceDB) to index file contents, AST nodes, chat history, and terminal outputs. Provides a unified context layer accessible by all active AI processes.


Tree-Sitter Surgical AST Patching: Parses codebases into Abstract Syntax Trees to generate line-by-line unified diff patches. Modifies exact target nodes rather than regenerating full files, saving tokens and preventing code regressions.


Language Server Protocol (LSP) Pre-Check: Connects to local LSP servers to validate TypeScript, Python, or Rust types in memory prior to applying changes to disk.


Dynamic Context Pruning: Automatically detects and strips redundant stack traces, duplicate log lines, and outdated context blocks from active model memory windows.


Predictive File Pre-Fetching: Analyzes prompt intent in real time to pre-load relevant project files into system RAM while the prompt is being typed.


3. Autonomous Execution & Sub-Agent Mechanics
Non-Blocking Terminal Sub-Agent: Executes long-running shell processes (npm build, pip install, docker-compose) in a decoupled background worker thread, keeping the UI interactive.




Self-Healing Terminal Error Loop: Intercepts stderr outputs from failed commands, routes the stack trace to high-speed endpoints (Groq/Gemini Flash), generates a corrective patch, and retries the command automatically.


Automatic Dependency Provisioning: Proactively identifies uninstalled libraries or system packages (npm, pip, apt, brew) mentioned in code patches and installs them silently in the background.


Sub-Agent Recall Hook Indicator: Dispatches asynchronous callback signals to update the UI and notify the orchestrator when background builds or tests complete.


Multi-Branch Workspace Isolation: Executes experimental code changes inside temporary Git worktrees, shielding the main workspace branch from broken builds or failing tests.


4. Vision & Humanlike Web Automation Engine
Computer Vision UI Mapping: Combines Playwright DOM inspection with object detection models to locate buttons, inputs, dropdowns, and canvas components on third-party websites without public APIs.


Bézier Curve Motion Trajectories: Generates organic mouse movement paths with realistic acceleration, deceleration, and micro-overshoots to replicate human hand movement.


Randomized Typing Cadence: Introduces micro-delays between keystrokes to mimic human typing speeds and avoid bot detection mechanisms.


Anti-Bot & Captcha Navigation: Detects interactive rate-limit screens, modal pop-ups, and dynamic challenges, adjusting navigation strategies without throwing fatal execution errors.


Session & Cookie Vault: Persists encrypted local storage states, user-agent profiles, and session cookies to maintain login states across multiple automated sessions.


MCP Protocol Bridge: Integrates native Model Context Protocol (MCP) server support alongside raw browser automation for hybrid web-API workflows.


5. Interactive Slash Command Suite (/)
/fix: Pulls the latest terminal exception, analyzes the relevant AST context, and applies an automated patch.


/clean: Clears build caches (node_modules, __pycache__), purges temporary logs, and defragments the local LanceDB index.


/compact: Compresses active chat history into dense vector embeddings while preserving critical workspace context.


/rollback: Reverts the workspace to its exact state prior to the last AI-generated patch using local Git AST history.


/mode [eco | balanced | beast]: Switches model execution strategy and hardware resource allocation dynamically.


/explain: Produces architectural breakdowns for selected functions or modules without mutating any files.


/test: Automatically constructs unit tests for active files and executes them via the background terminal sub-agent.


6. Safety, Process Control & Telemetry
One-Click Process Purge (PID Killer): A physical UI button and TUI shortcut to terminate deadlocked build scripts, runaway sub-agents, or infinite loops instantly.


Hyperparameter Control Sliders: Real-time controls to adjust Temperature, Top-P, Top-K, and Repetition Penalty per model node during active sessions.


Token & Rate Limit Telemetry Radar: Displays live metrics for Tokens Per Second (TPS), active latency (ms), and remaining free-tier API quotas.


Resource Throttler: Caps memory allocation (~1.2 GB RAM ceiling) and CPU thread priority, keeping system usage light on constrained development hardware.


AI Code Smell & Security Detector: Scans proposed code patches for security risks, exposed keys, and performance bottlenecks before committing files to disk.


7. Hybrid Dual-Interface System (GUI & TUI)
Unified Visual System: Built around a Deep Onyx (#0D0D10) dark theme, Warm Amber (#FF8C00) accents, rounded Bento-box cards, and crisp typography.


Web Dashboard (React + Tailwind): Features a multi-column cockpit layout with a dual-pane prompt/reasoning viewer, live AST diffs, a streaming Playwright canvas, and real-time token radars.


Terminal Interface (Python Textual/Rich): Provides 1:1 visual parity inside the terminal, complete with Unicode rounded card borders, live streaming console output boxes, and keyboard-first slash navigation.

Core System & Execution Control
/mode [eco | balanced | beast]



Description: Dynamically toggles execution hardware and model routing strategy.


Underlying Engine: Eco routes prompts through local Ollama instances; Balanced uses a single cloud key (e.g., Gemini Flash); Beast engages parallel multi-model consensus across all connected providers.


/purge [pid]



Description: Triggers the emergency PID Killer to forcefully terminate deadlocked sub-agents, runaway build scripts, or stuck background threads without crashing the main daemon.


Underlying Engine: Asynchronous process tree signal sender (SIGTERM / SIGKILL).


/rules [view | reload | edit]



Description: Manages workspace .rules architectural directives and coding standard constraints.


Underlying Engine: Injects active rule definitions directly into the system prompt prefix and AST validation pipeline.


/benchmark



Description: Executes speed and latency tests across all configured cloud and local model providers.


Underlying Engine: Sends standardized ping payloads to measure Tokens Per Second (TPS), Time To First Token (TTFT), and latency in milliseconds.


/keys [status | rotate]



Description: Displays current BYOK key utilization, rate-limit windows, and quota health across Google AI Studio, Groq, OpenCode, and Ollama.


Underlying Engine: Real-time API telemetry parser and dynamic fallback key manager.


Code Engineering & AST Surgery
/fix [terminal | line_range]



Description: Captures the latest error stack trace or targeted code block, constructs a surgical AST patch, and applies the fix.


Underlying Engine: Tree-Sitter AST parser + Groq/Gemini high-speed inference engine.


/diff



Description: Launches an interactive "Before & After" diff viewer showing pending AI modifications before committing changes to disk.


Underlying Engine: Git unified diff parser and local AST line-change inspector.


/refactor [function_name | module]



Description: Performs targeted structural code refactoring on specific syntax nodes without altering surrounding file context or introducing regressions.


Underlying Engine: Tree-Sitter AST node replacement engine coupled with LSP type-checking validation.


/explain [selection]



Description: Generates a detailed architectural breakdown of targeted functions, classes, or logic flows.


Underlying Engine: Read-only prompt routing without writing to disk or altering vector state.


/test [file_path]



Description: Auto-generates unit/integration tests for target files and executes them in the non-blocking background terminal sub-agent.


Underlying Engine: Subprocess test runner (pytest, vitest, jest) + assertion generator.


/doc [export_format]



Description: Scans modified code modules and auto-writes JSDoc, PyDoc, or OpenAPI specifications.


Underlying Engine: AST comment block generation and structural documentation parsing.


/security



Description: Audits active workspace files for hardcoded API secrets, vulnerable dependencies, and unsafe execution paths.


Underlying Engine: Static AST pattern scanning combined with automated CVE vulnerability matching.


SSOT Memory & Vector Management
/clean [cache | db | all]



Description: Clears temporary build artifacts (node_modules, __pycache__) and defragments the local LanceDB vector index.


Underlying Engine: OS file system cleanup utilities + LanceDB index optimization triggers.


/compact



Description: Summarizes active conversational state into dense vector embeddings to free up prompt context windows while preserving memory continuity.


Underlying Engine: Recursive text summarizer and LanceDB embedding update workflow.


/inspect [query]



Description: Opens the visual vector database inspector to view indexed code chunks, semantic score distances, and context relevance weights.


Underlying Engine: LanceDB vector similarity query visualizer.


/rollback [step_count]



Description: Reverts workspace files to their exact state prior to recent AI patches using local Git AST history.


Underlying Engine: Internal Git worktree commit parser and automated checkout manager.


Vision & Humanlike Web Automation
/browse [url]



Description: Spawns a Playwright headless/headful browser instance targeting a specific URL for automated interaction or data scraping.


Underlying Engine: Playwright core driver + real-time canvas stream renderer.


/stealth [low | medium | high]



Description: Adjusts Bézier curve curvature intensity, typing micro-delays, and user-agent spoofing parameters to evade anti-bot triggers.


Underlying Engine: Synthetic human-input motion algorithm and random header generation library.


/session [save | load | clear] [domain]



Description: Manages encrypted browser cookies, local storage payloads, and authentication tokens for target websites.


Underlying Engine: AES-256 encrypted local state vault linked to Playwright context profiles.


/mcp [list | connect | logs] [server_name]



Description: Connects, inspects, or debugs active Model Context Protocol (MCP) server integration bridges.


Underlying Engine: Standard MCP client protocol wrapper and JSON-RPC payload inspector.


Workspace Sandboxing & Consensus
/worktree [create | merge | discard] [branch_name]



Description: Creates an isolated Git worktree sandbox to execute high-risk code refactoring without touching the primary development branch.


Underlying Engine: Native git worktree isolation engine.


/consensus [prompt]



Description: Forces simultaneous multi-model execution across DeepSeek R1, Gemini 2.0 Pro, and Groq to compare and synthesize distinct reasoning paths.


Underlying Engine: Asynchronous parallel API orchestration layer and response deduplication algorithm.


! Direct System & Hardware Signal Commands (Force Execution Layer)

Commands prefixed with ! bypass the AI reasoning layer and issue direct instructions to the OS, local hardware, or system daemon.

!sh [command]



Description: Executes a raw shell command directly in the host system terminal without AI interception or safety pre-checks.


Underlying Engine: Async Python subprocess.Exec stream piped directly to stdout/stderr.


!kill [pid | all]



Description: Issues a direct OS signal to terminate target background processes, runaway sub-agents, or stuck node processes.


Underlying Engine: Low-level OS process tree signal sender (os.kill with SIGKILL / SIGTERM).


!hw



Description: Displays live host machine hardware telemetry (CPU core load, RAM allocation, GPU utilization, and swap space).


Underlying Engine: psutil system metrics fetcher with real-time hardware polling.


!override



Description: Temporarily disables system .rules files, security linters, and AST safety barriers for a single execution cycle.


Underlying Engine: Context flag toggle bypassing input validation hooks in the FastAPI daemon.


!install [package_name]



Description: Directs the daemon to instantly install a missing package (pip, npm, apt) into the active environment without confirmation prompts.


Underlying Engine: Package manager CLI binding execution worker.


!git [native_command]



Description: Passes a raw command directly to the local Git binary (!git push, !git commit -m "...", !git checkout).


Underlying Engine: Direct native Git CLI wrapper execution.


!hard-reset



Description: Forces a complete daemon state flush, killing all background workers, clearing RAM caches, and restarting the local server.


Underlying Engine: FastAPI self-restart pipeline paired with memory release garbage collection.


@ Context Targeting & Entity Reference Commands (Context Scoping Layer)

Commands prefixed with @ allow explicit injection of workspace resources, hardware nodes, visual streams, or external data into the active AI prompt context window.

@file [relative_path]



Description: Attaches a specific workspace file directly into the model's active context window with syntax-aware framing.


Underlying Engine: Tree-Sitter AST parser file reader with token-count tracking.


@folder [directory_path]



Description: Injects an entire directory structure and file index tree into the context window for broad architectural tasks.


Underlying Engine: Recursive file-tree walker combined with structural AST directory serialization.


@terminal [line_count]



Description: Pulls the last N lines of stdout/stderr logs from the background terminal sub-agent directly into the prompt context.


Underlying Engine: Circular ring-buffer memory log reader from the async subprocess runner.


@diff



Description: Scopes the model's focus exclusively to uncommitted local Git code changes across the current workspace.


Underlying Engine: git diff output parser formatted into unified unified-diff blocks.


@model [gemini | deepseek | groq | opencode]



Description: Forces a specific query or task to be routed to a target AI provider, overriding default auto-routing settings.


Underlying Engine: LiteLLM model routing flag modifier.


@browser



Description: Takes a visual snapshot and extracts the live DOM node tree from the Playwright canvas to use as context for web actions.


Underlying Engine: Playwright DOM accessibility tree snapshot + visual base64 screenshot decoder.


@docs [library_name | url]



Description: Fetches, parses, and injects external framework documentation or web API specs into the immediate reasoning context.


Underlying Engine: Async Web Scraper / Readability parser integrated into the LanceDB context staging buffer.


@mcp [server_node]


Description: References contextual data, schema structures, or tools exported by an active Model Context Protocol server.


Underlying Engine: MCP JSON-RPC protocol endpoint query runner.


@ssot [query_string]



Description: Performs a manual vector similarity search against the local vector database and injects top matching code chunks.


Underlying Engine: LanceDB vector distance query engine using local text embeddings.
  

Header & Global System Telemetry

Brand Pulse Badge: Displays "THE ROBBER AGENT v1.0" branding alongside a pulsing neon LED indicator that shifts color based on state (Green: Idle, Amber: Reasoning, Cyan: Web Automating, Red: Error/Terminated).


Model Engine Selector: An interactive dropdown pill allowing instant routing switches between active LLMs (Gemini 2.0 Pro, DeepSeek R1, Groq Llama 3.3, and OX Alpha on OpenCode).


Power Mode Switcher: A three-way segmented toggle switch (Eco | Balanced | Beast) that dynamically shifts execution between local Ollama models, single-key cloud APIs, or parallel multi-model consensus.


Token & Latency Radar: A real-time telemetry counter displaying active Tokens Per Second (TPS), round-trip API latency in milliseconds, and remaining free-tier daily quotas.


Emergency PID Killer Button: A high-visibility, elevated red action button that issues an immediate OS-level SIGKILL signal to terminate stuck background processes, deadlocked sub-agents, or infinite loops.


Left Sidebar: SSOT Memory & Project Tree

Tree-Sitter Project Explorer: A file tree view powered by Tree-Sitter parsing, featuring custom file icons, syntax-aware node nesting, and real-time AST change badges (Added, Modified, Staged).


SSOT Vector State Gauge: A visual progress meter displaying indexed file counts, total vector embeddings, and LanceDB database health in memory.


Interactive Command Palette (/, !, @): A searchable drawer listing available slash commands (/fix, /rollback), force signals (!sh, !kill), and context targeting triggers (@file, @browser).


Git Worktree Shield Bar: An indicator card showing active Git branches and temporary isolated worktrees used for sandbox testing.


System Hardware Telemetry Widget: A compact bottom card monitoring real-time host RAM allocation (capped under 1.5 GB), CPU core usage percentage, and active process threads.


Center Workspace: Execution Arena & Code Editor

Dual-Pane Prompt & Reasoning Canvas: A split-view interface separating raw user prompts from the agent's internal "Chain-of-Thought" reasoning and planning steps.


Floating Macro Input Bar: A sleek, rounded input container centered on the workspace, equipped with model selector dropdowns, file attachment triggers (@), and a rounded submission button (↑).


Tabbed File Workspace Bar: A horizontal browser-style tab bar for managing active code files, complete with unsaved modification dots and file-type badges.


Surgical AST Diff Viewer: An inline code editor view displaying line-by-line syntax changes using green (additions) and red (deletions) highlighting, bypassing full-file rewrites.


Hyperparameter Adjustment Sliders: Real-time range sliders for modifying LLM execution mechanics on the fly, including Temperature (0.0–1.0), Top-P, and Repetition Penalty.


Right Panel: Sub-Agent Terminal & Browser Automation

Non-Blocking Terminal Console: An asynchronous streaming console log box rendering background npm, pip, and shell script outputs without freezing the UI thread.


Self-Healing Loop Monitor: A dedicated execution feedback card that intercepts stderr exception traces, displays auto-generated bug fixes, and logs retry attempts.


Playwright Vision Stream Canvas: A live visual preview pane rendering the active headless browser session, complete with visual overlays over detected DOM elements.


Bézier Motion & Cadence Sliders: Controls to adjust humanlike automation parameters, including mouse cursor trajectory curvature, acceleration curves, and typing delay randomization ranges.


MCP Server Hub & JSON Inspector: An accordion list of connected Model Context Protocol servers with an expandable JSON viewer for inspecting live request/response payloads.


Encrypted Session Vault: A security card for managing stored cookies, authentication headers, user-agent profiles, and local storage states for target automated domains.
  

The CLI Terminal User Interface (TUI) is built using Python's Textual and Rich frameworks. It replicates the Web Dashboard's 3-column Bento grid layout within a standard terminal window, using Unicode rounded box-drawing characters (╭───╮, │, ╰───╯), ANSI color codes, and keyboard-first controls.

Top Header Dock (Sticky Status Bar)

TUI Brand Header: A prominent Unicode badge displaying [THE ROBBER AGENT v1.0] with a dynamic Rich color tag ([bold green]IDLE[/], [bold yellow]THINKING[/], [bold cyan]AUTOMATING[/]).


Model Engine Badge: Displays the active model provider tag (e.g., [Gemini 2.0 Pro], [DeepSeek R1]).


Power Mode Segment: A visual text toggle highlighting the active hardware profile: [ECO | BALANCED | BEAST].


Telemetry Micro-Bar: Compact ANSI text counters rendering live Tokens Per Second (48 TPS), API Latency (120ms), and daily quota usage percentages.


Left Column: Workspace Tree & Memory (Textual Panel / 20% Width)

Textual File Tree Widget: An interactive ASCII directory tree using Unicode branch markers (├──, └──) with color-coded file status tags ([+] Staged, [*] Modified).


SSOT Vector Gauge (Rich.Progress): A text-based progress bar showing LanceDB vector embedding indexing status and total indexed file chunks.


Keybinding Footer Drawer: A sticky list of terminal shortcuts ([F1] Help, [F2] /fix, [F3] !kill, [F5] Mode).


Hardware Monitor Box: A compact ASCII box rendering real-time CPU thread usage bars and system RAM allocation capped under 1.5 GB.


Center Column: Execution Arena & Prompt (Textual Panel / 55% Width)

Dual-Pane Reasoning Window: A split Rich.Panel container separating the agent's internal Chain-of-Thought logs from the primary conversation stream.


Surgical AST Diff Panel: A syntax-highlighted code block displaying unified line diffs with green + additions and red - deletions.


Central TUI Input Bar (Textual.Input): A command box supporting inline autocomplete overlays when typing / slash commands, ! system signals, or @ context targets.


Hyperparameter Status Row: A single-line ASCII readout displaying active execution parameters (Temp: 0.2 | Top-P: 0.95 | Rep: 1.1).


Right Column: Sub-Agent & Automation Stream (Textual Panel / 25% Width)

Streaming Sub-Agent Terminal (Rich.Log): A non-blocking, scrollable log viewport streaming background npm, pip, and shell script execution outputs.


Self-Healing Exception Box: An alert panel with an amber border that isolates caught stderr stack traces and displays auto-remediation steps.


ASCII Playwright Snapshot Box: A text-based DOM tree preview box rendering live element coordinates, click targets, and selector states during web automation tasks.


MCP Server Collapsible Accordion: Expandable Textual tree blocks displaying connected Model Context Protocol servers and live JSON-RPC payload logs.
  

Programming Languages

Primary Backend & Automation Engine: Python 3.11+ (Selected for native asynchronous asyncio handling, Playwright bindings, AST manipulation, and vector database compatibility).


Web GUI Dashboard: TypeScript / JavaScript (Node.js 20+ build environment, React 18/19 framework, Tailwind CSS).


Terminal CLI (TUI): Python 3.11+ (Leveraging Textual and Rich frameworks to achieve 1:1 visual UI parity with the Web GUI).


Backend Requirements & System Libraries

Core Daemon Framework: FastAPI powered by Uvicorn ASGI server for high-speed REST endpoints and WebSockets for real-time streaming data.


LLM Routing & Multi-Model Orchestration: LiteLLM for universal API abstraction across Google AI Studio (Gemini), Groq, OpenCode, DeepSeek, and local Ollama nodes.


AST Parsing & Surgery Engine: tree-sitter and tree-sitter-languages for parsing TypeScript, Python, C++, and JavaScript into Abstract Syntax Trees for surgical line diffs.


Browser Automation & Vision Infrastructure: playwright (async Python API) combined with opencv-python-headless and pillow for DOM canvas analysis and visual element detection.


Asynchronous Sub-Agent Runner: Native asyncio subprocess streams (asyncio.create_subprocess_exec) for non-blocking terminal execution and stdout/stderr capturing.


Host System Telemetry: psutil for monitoring host hardware metrics (CPU core loads, memory allocation, PID process trees).


Security & Key Encryption: cryptography (AES-256 symmetric encryption) for storing BYOK keys, session cookies, and local domain tokens.


Frontend Requirements (Web Dashboard)

UI Framework & Build Tools: React.js built with Vite for rapid development and lightweight asset bundling.


Styling & UI System: Tailwind CSS (configured with dark Onyx #0D0D10 background and Amber #FF8C00 accents) paired with Lucide React icons.


State & WebSocket Management: Zustand for global state management; ReconnectingWebSocket for resilient, zero-lag streaming of terminal logs, token telemetry, and Playwright canvas snapshots.


Code & Diff Viewer Component: @monaco-editor/react or CodeMirror 6 customized with inline diff highlighting extensions for surgical code modifications.


Database & Storage Architecture

Vector Database (SSOT Memory Engine): LanceDB (An embedded, serverless, ultra-fast vector database running directly on the local file system without Docker containers or background services).


Local Text Embeddings: fastembed / sentence-transformers for zero-cost, local vector generation directly on the host CPU.


Session & Vault Storage: Local encrypted SQLite file or .vault JSON storage for persisting domain cookies, local storage states, and custom .rules directives.


System & Hardware Execution Baseline

Target Hardware Specification: Optimized to run efficiently on an Intel Core i5-4590 (4 Cores / 4 Threads) with 8 GB DDR3 RAM and 10 GB free disk space.


Memory Ceiling Enforcer: Strict RAM overhead ceiling capped between 1.1 GB and 1.3 GB total footprint across the Python daemon, LanceDB index, and browser canvas worker.


OS & Environment Compatibility: Cross-platform support across Windows 10/11 (PowerShell/CMD), Linux (Ubuntu/Debian), and macOS via local loopback (127.0.0.1:8000).
   


The Unified Context Engine and the BYOK Router form the core architectural foundation of The Robber Agent, decoupling persistent memory and AI model orchestration from proprietary SaaS backends.

---

**1. UNIFIED CONTEXT ENGINE (SSOT MEMORY)**

The Unified Context Engine serves as a local-first Single Source of Truth (SSOT). Instead of feeding whole files or fragmented conversation histories into an LLM—which burns tokens and causes context degradation—this engine maintains a live, vectorized representation of the entire workspace, AST nodes, terminal logs, and agent decisions.

```
+-----------------------------------------------------------------------------------+
|                           UNIFIED CONTEXT ENGINE (SSOT)                           |
+-----------------------------------------------------------------------------------+
|  1. FILE SYSTEM WATCHER (`watchfiles`)                                           |
|     Tracks real-time file creation, mutation, and deletion events (`IN_MODIFY`).  |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  2. AST SURGICAL CHUNKER (`tree-sitter`)                                         |
|     Parses raw code into functional syntax nodes (Functions, Classes, Imports).  |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  3. LOCAL VECTOR PIPELINE (`fastembed` / ONNX Runtime)                            |
|     Generates 384/768-dim dense vectors locally on host CPU (~0ms API cost).      |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  4. EMBEDDED VECTOR STORE (`LanceDB` on Disk)                                     |
|     Performs Hybrid Search (BM25 Keyword + Vector Cosine Similarity).            |
+-----------------------------------------------------------------------------------+

```

**Step-by-Step Internal Mechanics**

1. **AST-Aware Code Chunking:** When a workspace is loaded, raw code files are not split by arbitrary character limits. Instead, `tree-sitter` parses the codebase into an Abstract Syntax Tree (AST), isolating distinct semantic structures (classes, functions, interface definitions).
2. **Zero-Cost CPU Vectorization:** Extracted AST chunks are passed to `fastembed`, an ONNX Runtime-backed local embedding library. It converts code snippets into dense vector embeddings locally without sending data over the internet or incurring API costs.
3. **Hybrid Search Indexing:** Embeddings and metadata are written directly into an embedded `LanceDB` table stored on the host disk. Queries execute a hybrid retrieval pipeline, combining full-text keyword search (BM25) with vector cosine similarity search.
4. **Real-Time Differential Synchronization:** A background file-system daemon (`watchfiles`) intercepts file save events. When a file changes, the engine calculates an AST diff, purges only the modified vector IDs from LanceDB, and re-indexes the new AST nodes in milliseconds.
5. **Context Window Staging:** Before any prompt is dispatched to an AI model, the engine queries LanceDB for top-scoring context chunks, formats them into a unified system context buffer, and prunes redundant stack traces or duplicate imports.

**Development Frameworks & Module Stack**

* **Vector Database:** `lancedb` (Native Python embedded vector store; requires no server process or Docker container).
* **Local Embedding Engine:** `fastembed` (C++ ONNX Runtime bindings for fast CPU inference).
* **AST Code Parser:** `tree-sitter` with `tree-sitter-languages` (Multi-language grammar parser).
* **File System Monitor:** `watchfiles` (Rust-backed asynchronous file watcher for Python).
* **Data Schemas:** `pydantic` v2 (Strict validation for vector metadata payloads).

---

**2. BYOK (BRING-YOUR-OWN-KEY) & MULTI-MODEL ROUTER**

The BYOK Engine enables zero-cost operation by establishing direct, unmediated client-to-API communication from localhost (`127.0.0.1`) to official LLM endpoints. It bypasses SaaS subscription markups, proxy servers, and artificial speed throttles by allowing developers to plug in their personal developer API keys.

```
+-----------------------------------------------------------------------------------+
|                        BYOK MULTI-MODEL ROUTING ENGINE                            |
+-----------------------------------------------------------------------------------+
|  1. AES-256 ENCRYPTED KEY VAULT (`cryptography.fernet`)                          |
|     Decrypts personal keys in-memory using machine-specific hardware signatures.  |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  2. UNIVERSAL SCHEMA TRANSLATOR (`LiteLLM` + `httpx`)                             |
|     Normalizes API requests for Gemini, Groq, DeepSeek, OpenCode, and Ollama.     |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  3. TELEMETRY & AUTO-ROTATION RADAR                                               |
|     Monitors TPS/TTFT, catches HTTP 429 errors, and auto-switches backup keys.   |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  4. ASYNCHRONOUS CONSENSUS SYNTHESIZER (`asyncio.gather`)                         |
|     Dispatches prompts in parallel across models; merges logic trees into AST diffs. |
+-----------------------------------------------------------------------------------+

```

**Step-by-Step Internal Mechanics**

1. **Hardware-Locked Encryption Vault:** Personal API keys (Google AI Studio, Groq, OpenCode, DeepSeek) are encrypted at rest using AES-256 (Fernet). The encryption key is derived from local host machine identification markers (CPU UUID + MAC address), ensuring keys cannot be transferred or read outside the host machine.
2. **Unified Endpoint Abstraction:** The router leverages `LiteLLM` to normalize incoming prompts into standard JSON schemas. Whether targeting Gemini 2.0 Pro, DeepSeek R1, or a local Ollama instance, the application logic communicates with a single interface.
3. **Telemetry & Rate-Limit Tracking:** Every outbound request passes through an async network interceptor built on `httpx`. It monitors Time-To-First-Token (TTFT), Tokens-Per-Second (TPS), active latency, and HTTP status codes in real time.
4. **Dynamic Key & Model Fallback:** If a cloud provider returns an HTTP 429 (Rate Limit Exceeded) or HTTP 503 error, the router intercepts the failure within 10 milliseconds, rotates to a secondary API key from the local key pool, or reroutes the request payload to an alternate provider (e.g., fallback from Groq to Gemini Flash).
5. **Parallel Model Consensus (Beast Mode):** When operating in parallel mode, the engine uses Python's `asyncio.gather()` to stream prompt payloads to multiple models simultaneously. The incoming responses are evaluated by a consensus algorithm that eliminates logic duplicates and outputs a single synthesized execution plan.

**Development Frameworks & Module Stack**

* **Unified API Wrapper:** `litellm` (Normalizes API parameters and streaming responses across 100+ LLMs).
* **Async HTTP Engine:** `httpx` (High-performance HTTP client supporting HTTP/2 and WebSockets).
* **Encryption Vault:** `cryptography.fernet` (AES-256 symmetric encryption library).
* **Concurrency Core:** Python native `asyncio` event loop.
* **Telemetry & System Metrics:** `psutil` (Tracks host memory, CPU threads, and network socket activity).
   

12-Model Parallel Consensus Architecture on a Single Task
Executing 12 distinct AI models concurrently on a single task requires a Map-Reduce Orchestration Pattern tied to the read-only snapshot of the Single Source of Truth (SSOT) Unified Context Engine. Rather than feeding raw prompt text to 12 models sequentially, the system decouples task breakdown, execution, and synthesis into three distinct phases.

                                 +---------------------------------------+
                                  |         USER TASK PROMPT              |
                                  +---------------------------------------+
                                                      |
                                                      v
                                  +---------------------------------------+
                                  |     UNIFIED CONTEXT ENGINE (SSOT)     |
                                  |  (LanceDB + Pre-Indexed Dependency    |
                                  |   Tree + Active AST State + Logs)     |
                                  +---------------------------------------+
                                                      |
                       +------------------------------+------------------------------+
                       | (Concurrent Read-Only Shared Context Lock via asyncio.gather) |
                       v                                                             v
        +-----------------------------+               ...             +-----------------------------+
        |  Model 1: DeepSeek R1       |                               |  Model 12: Groq Llama 3.3   |
        |  (Mathematical / Logic Tree)|                               |  (Syntax & Lint Validation) |
        +-----------------------------+                               +-----------------------------+
                       |                                                             |
                       +------------------------------+------------------------------+
                                                      |
                                                      v
                                  +---------------------------------------+
                                  |    SYNTHESIS & CONSENSUS ENGINE       |
                                  | (Weighted Scoring + Tree-Sitter AST)  |
                                  +---------------------------------------+
                                                      |
                                                      v
                                  +---------------------------------------+
                                  |       SURGICAL AST CODE PATCH         |
                                  +---------------------------------------+


Step-by-Step Execution Mechanics
Context Snapshot & Lock: When a prompt is submitted, the orchestrator freezes an immutable point-in-time snapshot of the Unified Context Engine. All 12 models read from this identical context snapshot simultaneously via zero-copy in-memory pointers, avoiding data races or vector state corruption.


Specialized Task Partitioning (The Map Phase): The orchestrator splits the primary prompt into 12 specialized sub-perspectives based on each model’s architectural strengths:



Model 1 (DeepSeek R1): Generates algorithmic logic and edge-case execution paths.


Model 2 (Gemini 2.0 Pro): Evaluates overall project architecture and structural dependencies.


Model 3 (Claude 3.5 Sonnet): Writes clean, maintainable modular code blocks.


Model 4 (Groq Llama 3.3 70B): Performs ultra-high-speed syntax checks and AST diff framing.


Model 5 (Codestral / Qwen Code): Analyzes type-safety, interface signatures, and bindings.


Model 6 (Mistral Large): Generates unit assertions and test scenarios.


Model 7 (OpenCode OX Alpha): Evaluates framework optimization and memory efficiency.


Model 8 (GPT-4o / O3-Mini): Audits security vulnerabilities and anti-patterns.


Model 9–12 (Auxiliary / Local Ollama Models): Run sanity checks, docstring generation, terminal command verification, and UI visual contract matching.


Asynchronous Parallel Dispatch: asyncio.gather() dispatches all 12 model payloads concurrently using non-blocking HTTP/2 connections managed by httpx and LiteLLM.


Consensus Aggregation & Voting (The Reduce Phase): The incoming responses are fed into a Consensus Synthesizer:



AST Node Alignment: Candidate code blocks are parsed into syntax trees using tree-sitter.


Weighted Voting: Logic structures agreed upon by a majority of high-tier models (e.g., DeepSeek + Gemini + Claude) receive high confidence scores.


Conflict Resolution: If Model 1 proposes a refactor that breaks Model 5's type-safety check, the synthesizer drops the conflicting patch and selects the highest-scoring compliant candidate.


Single AST Patch Output: The 12 streams collapse into a single, clean AST diff applied to the workspace.


Enhanced Unified Context Engine (Feature Specifications)
The Unified Context Engine incorporates real-time system monitoring, persistent environment states, and precise manual context manipulation controls.

+---------------------------------------------------------------------------------------------------+
|                               ENHANCED UNIFIED CONTEXT ENGINE (SSOT)                              |
+---------------------------------------------------------------------------------------------------+
|  [Dynamic Window Scaler]  |  [Context Pointer (@point)]  |  [Dependency Indexer (Installed PKGs)] |
|  Capped per-model bounds  |  Anchor AST nodes & files    |  Pre-scanned pip/npm/system maps       |
+---------------------------------------------------------------------------------------------------+
|  [Terminal Log Streamer]  |  [Import / Export Subsystem] |  [Pre-Quit Auto-Save Vault Hook]       |
|  Ring-buffered stdout/err |  `.robberctx` state dump     |  Zero data loss on exit signals        |
+---------------------------------------------------------------------------------------------------+


1. Dynamic & Adjustable Context Window Scaling
Mechanism: A slider in the Web GUI (and an inline slash command /context --limit [tokens] in the CLI TUI) dynamically caps or expands the token budget fed to each model.


Granular Allocation: Allows assigning a massive 100k+ token context window to long-context models (like Gemini) while restricting fast-check models (like Groq) to a tight 8k window, conserving rate limits and reducing latency.


2. Context Import & Export Subsystem (.robberctx)
Mechanism: Executes /context export [filename] to serialize the current LanceDB vector database, conversation state, AST index, active terminal logs, and system rules into a single compressed binary package (.robberctx).


Importing State: Running /context import [filename] instantly restores an entire workspace context on another machine or session without requiring re-indexing or initial code-analysis passes.


3. Context Section Pointing (@point Anchors)
Mechanism: Allows developers to pin specific functions, classes, or code regions into high-priority memory using syntax tags (e.g., @point:auth_service.py#validate_token or @point:line:45-80).


Priority Weighting: Pointed nodes receive a 2.0 relevance multiplier in the LanceDB hybrid search retriever, preventing critical functions from being pruned during automatic context summarization.


4. Real-Time Terminal Log Recorder & Ring Buffer
Mechanism: Intercepts every line of stdout and stderr emitted by background terminal processes (npm run dev, python main.py) and writes it to a circular, 5,000-line memory ring-buffer.


Vector Log Streaming: Error traces are indexed directly into the active vector database in real time. If a build fails, the agent immediately accesses the exact execution log without requiring manual copy-pasting.


5. Pre-Indexed Environment Dependency Tracker
Mechanism: On startup, a background worker scans host environment managers (pip list, npm list -g, cargo, system binaries) and saves an in-memory Dependency Map.


Zero-Exploration Execution: The agent knows instantly whether playwright, torch, tailwinds, or ffmpeg are installed. It will never run exploratory diagnostic commands like which node or pip show, eliminating unnecessary execution loops.


6. Auto-Save State Pre-Quit Hooks (Zero Data Loss)
Mechanism: Registers OS signal traps (SIGINT, SIGTERM, SIGHUP) and UI close events.


State Preservation: When quitting, the daemon intercepts the shutdown signal, commits all unwritten vector embeddings to disk, flushes active terminal logs, saves pending AST diffs, and writes out a .robber_session.lock file. Upon restart, session continuity is fully restored.


7. Additional System Extensions
Memory Pinning & Rule Locking: Designates project conventions (.rules) and core configuration files as immutable context elements that bypass garbage collection.


Context Snapshot Diffing (/context diff): Visually compares context states between two points in time to inspect how vector index weights changed during an editing session.


Automatic Garbage Collection & Defragmentation: Periodically scans the vector database to prune duplicate error logs, obsolete stack traces, and dead code references, keeping LanceDB search performance below 5ms.
Technical Module & Framework Mapping
Feature Component
Technology / Framework Stack
Primary Role
Consensus Engine
Python asyncio.gather + LiteLLM
Manages parallel model dispatch and multi-model API streaming.
AST AST Parser
tree-sitter / tree-sitter-languages
Parses multi-language code for surgical diffing and syntax consensus.
Vector Storage
LanceDB (Embedded Native C++/Python)
Stores local hybrid search index (BM25 + Cosine Distance).
Dependency Indexer
importlib.metadata + pkg_resources
Scans host package managers to map installed environment tools.
Terminal Ring-Buffer
asyncio.subprocess + collections.deque
Captures non-blocking terminal streams into an in-memory buffer.
Context Encryption
cryptography.fernet (AES-256)
Encrypts exported .robberctx packages and local BYOK keys.
TUI Interface
Python Textual + Rich
Renders TUI panels, ASCII gauges, and terminal diff views.
Web GUI Dashboard
React 19 + Tailwind CSS + Lucide React
Provides visual cockpit layout, AST diff viewer, and model monitors.

   

To bring The Robber Agent architecture from a conceptual framework to a fully realized, production-grade application, the remaining components needed span execution security, multi-agent coordination, and deployment tooling.

1. Inter-Agent Communication Bus (The Dispatcher)

Purpose: Manages secure, asynchronous messaging between sub-agents (e.g., when the planning agent passes a structured task payload to the browser automation agent or code-writing worker).


Underlying Engine: Redis Streams or an in-memory Pub/Sub broker using asyncio queues to prevent message drops and handle backpressure during 12-model parallel execution cycles.


2. Automated Sandbox & Execution Jail (Docker/Firejail Wrapper)

Purpose: Safely executes code generated by the parallel consensus models or raw shell commands (!sh) without risking host system integrity.


Underlying Engine: Ephemeral container isolation or system-level process sandboxing that restricts file-system write access strictly to the designated workspace root.


3. Visual AST Refactoring & Conflict Resolution UI

Purpose: Provides a human-in-the-loop merge interface when multiple parallel models propose conflicting surgical code patches for the same function.


Underlying Engine: A three-way merge conflict resolution screen integrated into both the React Web GUI and Textual TUI, highlighting semantic divergence using tree-sitter node comparisons.


4. Continuous Self-Correction & Feedback Loop Monitor

Purpose: Automatically catches test failures (pytest errors) or runtime exceptions (stderr), feeds the stack trace back into the context engine, and triggers an autonomous /fix loop until tests pass.


Underlying Engine: Event-driven listener tied to the terminal ring-buffer that automatically dispatches error payloads to a fast model (e.g., Groq) for rapid patch generation.


5. Plugin & MCP Extension Marketplace

Purpose: Allows quick installation of community-built Model Context Protocol (MCP) servers, custom automation tools, and specialized prompt templates.


Underlying Engine: A local package registry scanner that downloads, verifies checksums, and mounts external JSON-RPC tools into the daemon configuration.


What specific layer of the stack would you like to build or detail next?


**1. Inter-Agent Communication Bus (The Dispatcher)**

The Dispatcher acts as the nervous system of The Robber Agent, routing asynchronous events between internal sub-agents—including the Planner, AST Code Synthesizer, Terminal Executor, Playwright Vision Engine, and Consensus Orchestrator. It enforces strict backpressure control and priority queue management to prevent memory saturation during concurrent 12-model execution passes on local hardware.

**Core Architecture & Message Routing**

* **Async In-Memory Event Broker:** Built on Python's native `asyncio.PriorityQueue` and event-driven observers to pass messages zero-copy in RAM, maintaining a minimal memory footprint (~15 MB) without requiring external Redis processes.
* **Topic-Based Channel Segmentation:** Segregates system traffic across isolated channels:
* `agent.planning`: Task decomposition payloads and model consensus plans.
* `agent.execution`: Shell execution commands and Playwright action steps.
* `agent.ast_surgery`: Code diff proposals and Tree-Sitter syntax patches.
* `agent.telemetry`: Token rates, latency metrics, and hardware alerts.


* **Priority-Weighted Queueing:** Messages carry strict priority ratings (`CRITICAL` > `HIGH` > `NORMAL`). Emergency PID termination signals (`!kill`) and compiler syntax exceptions bypass standard task queues for instant processing.

**Standardized Message Payload Schema (Pydantic v2)**

* **`message_id`**: Unique UUIDv4 transaction identifier.
* **`correlation_id`**: Traces child sub-agent tasks directly back to the parent prompt session.
* **`sender_id` / `target_id**`: Routing nodes (e.g., `sender: vision_agent_01` → `target: terminal_subagent`).
* **`priority_level`**: Numeric rank (`0: SYSTEM_OVERRIDE`, `1: TASK_EXECUTION`, `2: BACKGROUND_LOG`).
* **`context_ref`**: Direct memory pointers referencing LanceDB vector IDs or Tree-Sitter AST node offsets.
* **`payload`**: Structured JSON containing execution commands, AST diffs, or diagnostic errors.

**Backpressure Control & Fail-Safe Mechanics**

* **Queue Depth Throttling:** Enforces a hard limit of 1,000 pending message events. If queue capacity approaches threshold limits during multi-model bursts, low-priority background logging pauses automatically to conserve host RAM.
* **Dead Letter Queue (DLQ):** Messages that fail sub-agent execution 3 times are routed to an isolated DLQ. This triggers an automated self-healing inspection pass instead of crashing the primary daemon thread.

Would you like to move directly to Component 2 (Automated Sandbox & Execution Jail), or do you want to tweak the Dispatcher's priority schema first?




2. Automated Sandbox & Execution Jail (Security & Isolation Layer)

The Automated Sandbox & Execution Jail provides an isolated, secure execution environment for AI-generated code, build scripts, test suites, and raw system commands (!sh). It prevents directory traversal, unauthorized network access, host file corruption, and malicious process spawns without adding heavy performance overhead to host hardware.

Dual-Tier Isolation Engine

Tier 1: Native Micro-Jail (Low Overhead - Default): Leverages Linux bubblewrap / firejail (or Windows Job Objects on Windows) to create an instant sandboxed process. It bind-mounts the active project root as the only writable directory while mounting system binaries (/bin, /usr) as read-only. Home directories (~), system secrets, and root paths remain invisible to the execution context. Startup latency is near-zero (~2ms).


Tier 2: Ephemeral Container Jail (High-Risk Tasks): For executing untrusted third-party code or running full dependency builds, the engine provisions lightweight, ephemeral Docker or Podman containers. The container runs on an unprivileged user namespace, mounts the workspace in isolation, executes the command, and self-destructs immediately upon completion.


Resource Capping & Syscall Filtering

cgroups v2 Enforcement: Enforces strict hardware boundaries per sandbox process tree:



RAM Ceiling: Max 512 MB per sandbox instance.


CPU Ceiling: Capped at 200% thread allocation (2 cores max).


Disk I/O: Throttled to prevent disk-filling loop attacks.


Seccomp System Call Profile: Injects a custom seccomp filter blocking dangerous kernel calls (ptrace, kexec_load, reboot, syslog, init_module). Sub-agent processes cannot inspect host memory spaces or escalate permissions.


Secret Masking & Environment Sanitization

Secret Stripping Pipeline: Before executing any shell command or script, the process launcher purges sensitive host environment variables (AWS_SECRET_ACCESS_KEY, SUDO_PASSWORD, BYOK LLM keys).


Path Jailing: Normalizes all file paths and blocks relative path navigation containing ../. Attempts to access paths outside the target workspace throw an instant security trap.


Subprocess Timeout Watchdog

Hard Execution Ceiling: Every sandboxed execution thread is assigned an enforced timeout counter (e.g., 30s default for tests, 120s for package installs).


SIGKILL Execution: If a subprocess hangs or enters an infinite loop, an asynchronous Python watchdog process sends an immediate SIGKILL to the sandbox process group, flushing stale threads from host memory.




3. Visual AST Refactoring & Conflict Resolution UI (Semantic Merge Engine)

When operating under 12-model parallel consensus or resolving conflicts between human edits and AI patches, standard text-line diffs (git diff) frequently break syntax by splitting functions or misaligning brackets. The Visual AST Refactoring & Conflict Resolution UI resolves conflicts at the structural syntax level using Abstract Syntax Tree (AST) node parsing, providing a visual merge interface across both the Web GUI and CLI TUI.

3-Way Semantic AST Diff Engine
Instead of treating code as flat text lines, the diff engine uses tree-sitter to parse code into a 3-way AST node tree:

Base Node (Ancestor): The original unmodified syntax tree before AI reasoning.


Consensus Proposal (Model AST): The unified AST structure generated by the multi-model consensus pass.


Local State (Developer AST): Uncommitted local developer modifications or active branch state.


The engine isolates exact node divergences (e.g., modified function signatures, appended class methods, reordered import statements) while ignoring non-functional whitespace or line-number shifts.

Dual-Interface Visual Layout
A. Web GUI Conflict Studio (React + Monaco Diff / CodeMirror 6)
Split Node Viewport: Renders the active file with visual color-coded node overlays (Green: Clean Additions, Amber: Semantic Conflicts, Red: Node Removals).


Interactive AST Breadcrumb Bar: Displays the exact structural path of the active conflict (e.g., src/auth.ts → Class: AuthManager → Method: validateToken()).


Floating Conflict Action Pill: A context-sensitive widget floating above the contested AST node providing 3 one-click actions:



[Accept AI Consensus]: Overwrites target node with multi-model patch.


[Keep Original Node]: Preserves developer's original AST node.


[Synthesize Hybrid AST]: Triggers a fast model pass (e.g., Groq) to merge both logic nodes safely.


B. CLI TUI Conflict Panel (Python Textual + Rich)
Side-by-Side Dual-Pane Terminal View: Uses Textual grid layout to render two parallel code panes with synchronized vertical scrolling.


Unicode Syntax Node Highlighting: Encloses conflicting AST nodes in rounded Unicode boxes (╭── Conflict: Function Signature ──╮).


Single-Key Hotkey Resolution:



[A]: Accept AI consensus node.


[K]: Keep local developer node.


[M]: Trigger interactive hybrid AST merge.


[Tab]: Jump to next contested AST node.


Pre-Flight LSP Validation & Syntax Shield
Before any resolved AST is committed to disk, it passes through an automated validation gate:

In-Memory AST Re-parse: Verifies that the merged node structure forms a valid syntax tree without dangling tokens or unclosed scopes.


LSP Pre-Check: Invokes local Language Server Protocol (LSP) diagnostics (tsserver, pyright, rust-analyzer) to ensure types, imports, and interface contracts remain valid.


Visual Syntax Alert: If a manual merge introduces a type error, the UI flashes an amber warning banner detailing the exact type mismatch line before allowing file save.


   

4. Continuous Self-Correction & Feedback Loop Monitor (Autonomous Healing Engine)

The Continuous Self-Correction & Feedback Loop Monitor transforms error handling from a reactive human bottleneck into an autonomous, closed-loop repair cycle. When a test suite fails, a build breaks, or a browser automation step misses a DOM element, the monitor intercepts the exception, diagnoses the root cause against the AST, generates a targeted patch, and re-executes the task until the build turns green.

Event-Driven Exception Interceptor
Multi-Source Log Trapper: Listens directly to the in-memory terminal ring-buffer and background workers, capturing raw stderr outputs from compilers (tsc, rustc), test runners (pytest, vitest, jest), and linter diagnostics (eslint, ruff).


Playwright Failure Detector: Captures browser automation exceptions, missing DOM element timeouts, and dynamic network failures from the Playwright engine alongside a base64 visual snapshot of the failed state.


Structured Exception Serialization: Formats raw stack traces into standardized error payloads containing:



Failed target file and exact line offset.


Exception class (TypeError, AssertionError, ElementHandleNotFound).


Surrounding Tree-Sitter AST code node context.











Autonomous Self-Healing Workflow
                        AUTONOMOUS SELF-HEALING LOOP                               |
+-----------------------------------------------------------------------------------+
|  1. INTERCEPT EXCEPTION                                                           |
|     Traps `stderr` stack trace / test assertion failure from ring-buffer.         |
+-----------------------------------------------------------------------------------+
                                         |+-----------------------------------------------------------------------------------+
|
                                         v
|  2. AST ROOT-CAUSE DIAGNOSIS                                                      |
|     Maps stack frame lines directly to exact Tree-Sitter code syntax nodes.       |
+-----------------------------------------------------------------------------------+
                                         |                                         v

|  3. HIGH-SPEED PATCH GENERATION                                                   |
|     Routes stack trace + AST context to fast inference endpoints (Groq / Gemini). |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  4. ISOLATED AST REPAIR APPLY                                                     |
|     Applies line diff patch in Git worktree sandbox & re-runs test/build command. |
+-----------------------------------------------------------------------------------+


AST Node Isolation: Maps stack trace line numbers directly to their parent AST nodes in memory using tree-sitter.


Context Enrichment: Queries LanceDB vector memory for related utility functions, type definitions, or recent code edits that caused the regression.


High-Speed Patch Generation: Routes the localized error context and AST snippet to a high-throughput endpoint (Groq Llama 3.3 / Gemini Flash) to formulate a minimal, targeted code patch.


Sandboxed Re-Execution: Applies the generated patch to a Git worktree sandbox and re-executes the failing test or build command automatically.


Execution Guardrails & Escalation Protocol
Iteration Ceiling (Max Retry Budget): Enforces a strict limit of 3 to 5 retry attempts per error loop to prevent infinite token consumption or runaway loops.


Loop Circuit Breaker: If the agent generates identical patches or fails to resolve the exception within the allocated retry budget, it halts execution, trips the circuit breaker, and escalates the issue.


User Escalation View: Flashes an amber alert banner in the UI (Web GUI and CLI TUI), presenting the developer with the persistent stack trace, attempted AI patches, and one-click manual overrides.



5. Plugin & MCP Extension Marketplace (Extensible Tooling Infrastructure)

The Plugin & MCP Extension Marketplace provides an extensible tool runtime allowing developers to dynamically extend The Robber Agent with custom Model Context Protocol (MCP) servers, community plugins, domain-specific rule sets, and system integrations—without modifying core daemon code.

Core Architectural Layers
+-----------------------------------------------------------------------------------+
|                   PLUGIN & MCP EXTENSION MARKETPLACE ENGINE                      |
+-----------------------------------------------------------------------------------+
|  1. LOCAL REGISTRY & MANIFEST SCANNER (`robber-plugin.json`)                     |
|     Loads plugin metadata, system permission requirements, and tool schemas.     |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  2. MCP CLIENT PROTOCOL LAYER (JSON-RPC 2.0 over stdio/SSE)                       |
|     Discovers resources, prompts, and tools from external Model Context Servers.  |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  3. DYNAMIC TOOL REGISTRATION & SCHEME INJECTOR                                   |
|     Injects tools into LiteLLM definitions, `@` context references, & `/` commands. |
+-----------------------------------------------------------------------------------+
                                         |
                                         v
|  4. ISOLATED RUNTIME SANDBOX & SECURITY GATEKEEPER                                |
|     Verifies SHA-256 checksums and enforces privilege scopes (FS, Network, Exec). |
+-----------------------------------------------------------------------------------+


Key Subsystems & Execution Mechanics
1. Native Model Context Protocol (MCP) Client
JSON-RPC 2.0 Engine: Implements full client support for the open MCP standard over stdio and Server-Sent Events (SSE).


Dynamic Capability Discovery: Automatically polls connected MCP servers on startup to extract:



Tools: Standardized executable functions (e.g., PostgreSQL query runners, Figma layout extractors, GitHub API adapters).


Resources: File-like data streams and URI schemas injectable into context via @ commands.


Prompts: Pre-engineered system template flows.


2. Manifest Schema (robber-plugin.json)
Every plugin or extension is declared using a standardized JSON manifest defining its scope and capabilities:

JSON
{
  "name": "db-schema-inspector",
  "version": "1.0.0",
  "description": "Inspects local SQLite & Postgres schemas and updates SSOT context",
  "permissions": ["network:localhost", "filesystem:read"],
  "entrypoint": "node dist/index.js",
  "transport": "stdio",
  "commands": [
    { "trigger": "/db-sync", "description": "Rescan local database schema into LanceDB" }
  ],
  "context_targets": [
    { "prefix": "@db", "description": "Inject table schemas into active context" }
  ]
}


3. Security Verification & Permission Scoping
SHA-256 Checksum Validation: Ensures remote plugin downloads match signed hashes before mounting to local runtime environments.


Explicit Permission Prompts: Enforces explicit user confirmation in the UI when a plugin requests elevated privileges (e.g., unrestricted network access, raw shell execution, system path access).


Process Isolation: Runs each MCP server in an unprivileged background subprocess bounded by system hardware limits (max 128 MB RAM per plugin).


4. UI & TUI Inspection Hub
Web GUI MCP Console: An accordion view rendering active connected servers, live request/response JSON payloads, and dynamic tool call execution statuses.


CLI TUI Tool Inspector: Accessible via /mcp command, rendering a clean Textual table of mounted tools, active RPC socket states, and performance metrics.


Command Integration
@mcp:[server_name]: Directs the context engine to pull live resources or schema objects from a targeted MCP server into prompt context.


!plugin install <repo_or_pkg>: Fetches, builds, and mounts a new plugin directly into .robber/plugins/.


/mcp reload: Dynamically restarts background JSON-RPC processes without restarting the main daemon thread.


Complete Architecture Overview Summary
With all 5 major modules defined—Inter-Agent Communication Bus, Automated Sandbox & Execution Jail, Visual AST Refactoring UI, Continuous Self-Correction Loop, and Plugin & MCP Marketplace—The Robber Agent forms a complete, self-contained, high-performance system capable of running local vector memory, parallel model consensus, and surgical code automation entirely under local hardware control.
