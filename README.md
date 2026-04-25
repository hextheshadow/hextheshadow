<!-- ───────────────────────────────────────────── -->
<!--  hextheshadow · GitHub README                 -->
<!-- ───────────────────────────────────────────── -->

<div align="center">

```
  _               _   _                 _               _  
 | |__   _____  _| |_| |__   ___  ___| |__   __ _  __| |___ _      __ 
 | '_ \ / _ \ \/ / __| '_ \ / _ \/ __| '_ \ / _` |/ _` / _ \ \ /\ / / 
 | | | |  __/>  <| |_| | | |  __/\__ \ | | | (_| | (_| \  __/\ V  V /  
 |_| |_|\___/_/\_\\__|_| |_|\___||___/_| |_|\__,_|\__,_|\___| \_/\_/   
```

**`vulnerability researcher`** &nbsp;·&nbsp; browser internals &nbsp;·&nbsp; sandbox security &nbsp;·&nbsp; ai-autonomous pipelines

<br/>

[![GitHub](https://img.shields.io/badge/github-hextheshadow-00ff6a?style=flat-square&logo=github&logoColor=00ff6a&labelColor=070a0d&color=182420)](https://github.com/hextheshadow)
[![HackerOne](https://img.shields.io/badge/hackerone-h3xb1tx-00ff6a?style=flat-square&logo=hackerone&logoColor=00ff6a&labelColor=070a0d&color=182420)](https://hackerone.com/h3xb1tx)
[![Bugcrowd](https://img.shields.io/badge/bugcrowd-HexShadow-00ff6a?style=flat-square&logo=bugcrowd&logoColor=00ff6a&labelColor=070a0d&color=182420)](https://bugcrowd.com/h/HexShadow)
[![Email](https://img.shields.io/badge/email-hextheshadow0x-00ff6a?style=flat-square&logo=gmail&logoColor=00ff6a&labelColor=070a0d&color=182420)](mailto:hextheshadow0x@gmail.com)

</div>

---

## `>_ whoami`

Independent vulnerability researcher at the intersection of **browser internals**,
**Linux kernel security**, and **AI-autonomous exploit pipelines**.

I operate research pipelines that autonomously map attack surfaces, reason about
logic flaws, generate PoCs, and triage findings — then validate everything manually
through dynamic instrumentation before responsible disclosure.

My work targets **Chromium**, **MetaMask**, **Doppler**, **Immutable Passport**,
and other high-impact open-source projects. I specialise in logic flaws and policy
bypass vulnerabilities that automated scanners miss.

---

## `>_ research`

| target | finding | status |
|--------|---------|--------|
| **Chromium** | Fenced Frame ACER Policy Bypass — missing check in `SetFencedFrameAutomaticBeaconReportEventData()` | `P3 · Privacy` |
| **MetaMask Snaps** | SES Compartment Sandbox Escape via thenable hijack in `BaseSnapExecutor.#registerSnapExports()` | `HackerOne` |
| **Doppler CLI** | Auth Token Exfiltration via `DOPPLER_API_HOST` injection in `PrepareSecrets()` | `In Triage` |
| **Immutable Passport** | Silent arbitrary transaction execution via attacker-controlled `apiUrl` | `Bugcrowd` |
| **Linux Kernel** | UAF in vsock Loopback Transport — race in `virtio_transport_consume_skb_sent()` yields KASAN-silent write primitive on `kmalloc-96` | `kernelCTF · 2026` |

---

## `>_ stack`

```
languages   →  C · C++ · Python
platforms   →  Linux (Arch, Ubuntu) · x86-64
tooling     →  GDB · ASAN · TSAN · KASAN · strace · ftrace · perf
domains     →  browser internals · sandbox escapes · IPC security · memory corruption
research    →  Chromium · Linux kernel · Hypervisors (KVM, gVisor)
```

---

## `>_ contact`

Open to **vulnerability research**, **browser security**, and **red team** roles.

<div align="center">

[![portfolio](https://img.shields.io/badge/portfolio-hextheshadow.github.io-00c8ff?style=for-the-badge&labelColor=070a0d&color=0c1117)](https://hextheshadow.github.io)
&nbsp;
[![email](https://img.shields.io/badge/email-hextheshadow0x%40gmail.com-00c8ff?style=for-the-badge&labelColor=070a0d&color=0c1117)](mailto:hextheshadow0x@gmail.com)

</div>

<br/>

<!-- hextheshadow · 2026 · finding what others miss -->
