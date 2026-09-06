# Anastasia Shebalkina

**Product Security Architect · Security Researcher · Purple R&D**

> Everything you build — sucks. Lucky for you, I know how to suckless.

Independent Security Architect with dual degrees in Computer Engineering and Information Security. Former Lead Fullstack Engineer, DevSecOps, and Technical Project Manager (including Critical Information Infrastructure).

My work follows the **Security by Subtraction** principle: eliminating systemic complexity instead of adding abstraction layers. Operating across the full stack — from bare-metal, OS internals, and core C libraries up to application logic, CI/CD pipelines, and business processes — I evaluate and design architectures with an adversarial mindset.

**Core focus:**

- **Product Security Architecture** — I simplify complex systems by eliminating architectural waste instead of stacking third-party defensive layers. By removing non-operational bloat, I reduce vulnerability noise, streamline SBOM/VEX compliance, and drastically lower operational expenditure (OpEx) while achieving mathematical determinism.
- **Low-Level & Runtime Hardening** — Enforcing strict execution boundaries and OS-level isolation (seccomp-bpf, Landlock, dm-verity, W^X, read-only squashfs). Expertise in low-level runtime edge cases (glibc vs musl, dynamic vs static linking illusions), toolchain-level attack surface reduction (DCE, LTO, CFI, -fno-exceptions), and kernel/binary-level stripping.
- **Adversarial Research & Audits** — Identification of structural design flaws, broken isolation, and complex logic vulnerabilities in web, mobile, and Web3 environments.

## Selected work

**The Static Linking Illusion** — OFFZONE 2026  
Showed how default glibc NSS dispatcher silently breaks self-contained isolation in OT/ICS and distroless builds by dynamic loading of host `.so` libraries inside "static" binaries. Includes a working PoC for ACE in static binaries. Acknowledged by Red Hat Product Security.  
→ [Research](https://blog.jarpex.com/research/offzone2026/) · [PoC](https://github.com/jarpex/glibc-static-nss-poc)

**CVE-2023-4911 (Looney Tunables)**  
Rewrote the LPE exploit in pure C with multi-process brute-forcing, dynamic calibration, and integrated ELF parser. Ported to AArch64 with adaptive ASLR bypass.  
→ [x86_64](https://blog.jarpex.com/articles/CVE-2023-4911/) · [ARM64](https://blog.jarpex.com/articles/CVE-2023-4911-arm64/) · [Exploit](https://github.com/jarpex/cve-2023-4911-exploit-optimized)

**spotlight-js**  
Zero-dependency image gallery under 9 kB brotli. Native trackpad gestures, touch, keyboard navigation.  
→ [Repository](https://github.com/jarpex/spotlight-js)

**Tools and contributions**  
Minimal systems tools: [siligpu](https://github.com/jarpex/siligpu) (Apple Silicon GPU telemetry in Rust), [uc](https://github.com/jarpex/uc) (unicode cleaner in C). Fullstack Shift-Left SSDLC reference implementation ([ssdlc-fastapi-backend](https://github.com/jarpex/ssdlc-fastapi-backend) & [ssdlc-svelte-frontend](https://github.com/jarpex/ssdlc-svelte-frontend)) featuring K3s self-hosted runners, Vault dynamic secret injection, Kaniko daemonless builds, automated SAST/DAST (CodeQL, Semgrep, ZAP), and SARIF dashboard integration. Upstream contributions to [bt](https://github.com/LeperGnome/bt) and [Runtime Radar](https://github.com/Runtime-Radar/runtime-radar).

---

If you also believe that complexity is the ultimate vulnerability — let's connect.

[jarpex.com](https://jarpex.com) · [blog.jarpex.com](https://blog.jarpex.com) · [Telegram Blog](https://t.me/defaultjarpex) · [LinkedIn](https://www.linkedin.com/in/jarpex/)
