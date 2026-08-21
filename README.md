<!-- hextheshadow · GitHub Profile README -->

<div align="center">


```
 _               _   _                 _               _
| |__   _____  _| |_| |__   ___  ___| |__   __ _  __| |___ _      __
| '_ \ / _ \ \/ / __| '_ \ / _ \/ __| '_ \ / _` |/ _` / _ \ \ /\ /
| | | |  __/>  <| |_| | | |  __/\__ \ | | | (_| | (_| \  __/\ V  V /
|_| |_|\___/_/\_\\__|_| |_|\___||___/_| |_|\__,_|\__,_|\___| \_/\_/
```


<br/>

**`vulnerability researcher`** &nbsp;·&nbsp; **`agentic systems`** &nbsp;·&nbsp; **`memory safety`**

<br/>

[![GitHub](https://img.shields.io/badge/hextheshadow-00ff6a?style=flat-square&logo=github&logoColor=00ff6a&labelColor=0d1117&color=0d1117)](https://github.com/hextheshadow)
[![Portfolio](https://img.shields.io/badge/portfolio-hex--the--shadow--vorthix.vercel.app-00ff6a?style=flat-square&labelColor=0d1117&color=0d1117)](https://hex-the-shadow-vorthix.vercel.app)
[![Email](https://img.shields.io/badge/haris@vorthix.com-00ff6a?style=flat-square&logo=gmail&logoColor=00ff6a&labelColor=0d1117&color=0d1117)](mailto:haris@vorthix.com)
[![Vorthix](https://img.shields.io/badge/vorthix.com-00ff6a?style=flat-square&labelColor=0d1117&color=0d1117)](https://vorthix.com)

</div>

---

## `>_ whoami`

Self-taught security researcher and AI systems engineer from Lahore, Pakistan.

I build **autonomous multi-agent systems** that do what an experienced vulnerability researcher does — read source code, form attack hypotheses, trace call graphs, confirm bugs with sanitizers, write working exploits, and produce full disclosure reports — without human involvement at any step.

My agents don't run scanners. They reason.

Founder of **[Vorthix](https://vorthix.com)** — an autonomous security research platform powered by **XOR-1**, a self-hosted multi-agent system running Qwen 3 27B that has operated continuously for **100+ hours** per session without getting stuck in a loop.

---

## `>_ research`

| target | finding | class | status |
|--------|---------|-------|--------|
| **libexpat** | Incomplete fix bypass for CVE-2026-50219 — `doCdataSection()` skips `beforeHandler()`/`afterHandler()`, leaving `m_handlerCallDepth` at zero during CDATA callbacks | `heap-UAF` · CWE-416 | ![](https://img.shields.io/badge/CVE--2026--56412-merged-00ff6a?style=flat-square&labelColor=0b1510) |
| **FreeRDP** | Unchecked palette read in `update_decompress_brush()` — stream check guarantees 8 bytes, palette dereference reaches stream\_pos+31 for bpp=32 | `heap-OOB-read` · CWE-125 | ![](https://img.shields.io/badge/CVE--2026--57158-confirmed-00c8ff?style=flat-square&labelColor=0b1510) |
| **LibRaw** | Dangling FORC loop variable reused as write offset in `rpi_load_raw8()` — crafted `padding_right` shifts every row write past the allocation end | `heap-overflow` · CWE-122 | ![](https://img.shields.io/badge/CVE--2026--72841-merged-00ff6a?style=flat-square&labelColor=0b1510) |
| **Monocypher** | Integer truncation in `crypto_argon2()` makes `lane_size` zero — init loop writes `blocks[1]` 1024 bytes past allocation end | `heap-overflow` · CWE-122 | ![](https://img.shields.io/badge/CVE--2026--53720-confirmed-00c8ff?style=flat-square&labelColor=0b1510) |
| **PJSIP / pjmedia** | H.263 `PLEN` field excluded from bounds check in `pjmedia_h263_unpacketize()` — single crafted RTP packet overflows decode buffer by up to 63 bytes | `heap-overflow` · network | ![](https://img.shields.io/badge/GHSA--8cxh--7rcw--x2m7-fixed · 2.18-00ff6a?style=flat-square&labelColor=0b1510) |
| **Chromium** | Fenced Frame ACER policy bypass — `SetFencedFrameAutomaticBeaconReportEventData()` accepts cross-origin beacon data without checking `allow_cross_origin_event_reporting_` | `privacy-boundary` | ![](https://img.shields.io/badge/P3%20·%20S3-in triage-f59e0b?style=flat-square&labelColor=0b1510) |
| **Linux Kernel** | UAF in vsock loopback transport — race in `virtio_transport_consume_skb_sent()` yields write + read primitive on `kmalloc-96` | `UAF` · KASAN | ![](https://img.shields.io/badge/kernelCTF%20·%202026-f59e0b?style=flat-square&labelColor=0b1510) |

---

## `>_ xor-1`

```
  input  →  github repo / source path / binary
  output →  confirmed vuln · sanitizer trace · minimized PoC · patch · disclosure report
  model  →  qwen 3 27b · self-hosted · openai-compatible api
  runtime → 100+ hours · no human intervention · no loop
```

**custom systems built from scratch:**

`call-graph` `find-callers` `memory-management` `token-management` `hypothesis-storage`  
`coverage-tracking` `deduplication` `self-correction` `loop-detection` `failure-handling`  
`agent-confidence` `context-management` `iteration-logging` `self-training-pipeline`

→ full architecture: **[hex-the-shadow-vorthix.vercel.app/#systems](https://hex-the-shadow-vorthix.vercel.app/#systems)**

---

## `>_ stack`

```
languages   →  C · C++ · Python
platforms   →  Linux (Arch, Ubuntu) · x86-64
sanitizers  →  ASan · KASan · UBSan · TSan
tooling     →  GDB · strace · ltrace · ptrace · DynamoRIO · ftrace · perf
ai/ml       →  LLM integration · self-hosted inference · agentic pipelines · training data
domains     →  memory corruption · browser security · kernel · IPC · agentic systems
```

---

## `>_ pocs`

Published PoCs for confirmed, patched vulnerabilities:  
**[github.com/hextheshadow/PoC-Exploit](https://github.com/hextheshadow/PoC-Exploit)**

---

## `>_ contact`

Open to **vulnerability research**, **AI security engineering**, **agentic systems**, and **red team** roles.

<div align="center">

[![portfolio](https://img.shields.io/badge/portfolio-hex--the--shadow--vorthix.vercel.app-00c8ff?style=for-the-badge&labelColor=0d1117&color=0d1117)](https://hex-the-shadow-vorthix.vercel.app)
&nbsp;
[![linkedin](https://img.shields.io/badge/linkedin-haris--hussain-00c8ff?style=for-the-badge&logo=linkedin&logoColor=00c8ff&labelColor=0d1117&color=0d1117)](https://linkedin.com/in/haris-hussain-42b93138a)
&nbsp;
[![email](https://img.shields.io/badge/email-haris@vorthix.com-00c8ff?style=for-the-badge&labelColor=0d1117&color=0d1117)](mailto:haris@vorthix.com)

</div>

<br/>

<div align="center">
<img src="https://komarev.com/ghpvc/?username=hextheshadow&style=flat-square&color=00ff6a&label=profile+views" />
</div>

<!-- hextheshadow · 2026 · autonomous research · finding what others miss -->
