# hextheshadow

Open Source Vulnerability researcher and browser security engineer.
I build AI-augmented pipelines that autonomously map attack surfaces,
reason about logic flaws, generate PoCs, and triage findings 
then validate everything manually.

## Research

**Chromium** — Fenced Frame ACER Policy Bypass  
Missing enforcement in `SetFencedFrameAutomaticBeaconReportEventData()`
allowing cross-origin iframes to fire automatic beacons across the
ACER boundary without operator opt-in. Confirmed on stable channel.

**MetaMask Snaps** — SES Compartment Sandbox Escape  
Zero-permission escape via thenable hijack in
`BaseSnapExecutor.#registerSnapExports()`. Snap-controlled `.then()`
fires as outer-realm microtask, bypassing SES entirely and exposing
real `globalThis` and Ethereum provider.

**Doppler CLI** — Auth Token Exfiltration via `DOPPLER_API_HOST` Injection  
`PrepareSecrets()` blocks `PATH`, `PS1`, `HOME` but leaves
`DOPPLER_API_HOST` injectable, allowing a malicious team member to
redirect `doppler run` to an attacker-controlled server with the
victim's real Bearer token.

**Immutable Passport SDK** — Unauthenticated Session Activity Endpoint  
Allows silent arbitrary transaction execution via attacker-controlled
`apiUrl` in custom chain configuration.

## Projects

**Ladybird Anti-Fingerprinting Engine** — C++ / Browser Internals  
Platform-coherent hardware identity generation system built into a
custom Ladybird fork. Generates internally consistent device profiles
enforced at the C++ component level — Windows profiles get ANGLE/D3D
GPUs, macOS gets Apple Silicon/Metal, iOS gets Apple SoC with no
discrete GPU. Covers audio, canvas, WebGL, navigator, geolocation,
timing, workers, UI events, and more. 10,000+ lines of custom C++.

## Skills
C · C++ · Python · GDB · ASAN/TSAN · Linux (Arch, Ubuntu) · x86-64
Browser internals · Sandbox escapes · IPC security · Memory corruption
