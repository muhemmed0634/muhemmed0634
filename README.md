<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:0f3d2e&height=170&section=header&text=Muhemmed&fontSize=62&fontColor=3fb950&fontAlignY=38&desc=Reverse%20engineering%20%C2%B7%20low-level%20C%20%C2%B7%20security%20Linux&descAlignY=60&descSize=17&animation=fadeIn" alt="Muhemmed">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=2800&pause=900&color=3FB950&center=true&vCenter=true&width=820&height=52&lines=Reverse+engineering+binaries.;C+first,+then+Assembly.;Building+OmidenOS,+a+security+live+system.;Linux+only." alt="Reverse engineering, C, Assembly, OmidenOS">

<p>
  <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" alt="C">
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Shell-4EAA25?style=flat-square&logo=gnubash&logoColor=white" alt="Shell">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Ghidra%20%C2%B7%20IDA%20Pro%20%C2%B7%20gdb-1f2328?style=flat-square" alt="Ghidra, IDA Pro, gdb">
  <img src="https://komarev.com/ghpvc/?username=muhemmed0634&label=PROFILE+VIEWS&color=0f3d2e&style=flat-square" alt="Profile views">
</p>

<img src="https://skillicons.dev/icons?i=c,cpp,py,js,linux,bash,git,cmake,html,css" alt="Toolchain">

<br>

<a href="https://portfolio-site-mocha-seven-44.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-site-3fb950?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"></a>
<a href="mailto:muhemmed0634@gmail.com"><img src="https://img.shields.io/badge/Email-muhemmed0634@gmail.com-1f2328?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

---

## Whoami

I take software apart. It started with crackmes — a binary with one hidden branch,
and no source to read — and grew into the systems those binaries run on: boot
loaders, initramfs, read-only root images, the parts that are invisible until they
break.

Most of what I write is C: small programs where I can explain every line and every
syscall, with no library I would not know how to debug. Python and JavaScript cover
the parts that need a server, a database or a UI in front of them.

## Selected work

| Project | What it is | Stack |
| --- | --- | --- |
| [**OmidenOS**](https://github.com/muhemmed0634/OmidenOs) | Live security system built with `mkarchiso`: UEFI-only boot, squashfs root with a RAM overlay, its own style linter and brand scanner, REUSE-licensed tree. Phase 2 of 8 is closed — it builds, boots on QEMU and VirtualBox, and drops to a shell. No installer yet. | `Python` `Shell` `Make` |
| [**Virbot v6**](https://github.com/muhemmed0634/Virbot) | Turkish and Azerbaijani Discord bot that replaces the usual stack of five bots with one process: moderation, jail, auto-role, levels, economy, giveaways, a Gemini-backed AI channel and a web dashboard. | `JavaScript` `discord.js` `MongoDB` |
| [**nmap-cli**](https://github.com/muhemmed0634/nmap-cli) | Menu-driven front end for nmap, in plain C with a CMake build and a release binary for people who do not want to remember flags. | `C` `CMake` |
| [**Crackme-with-muhemmed**](https://github.com/muhemmed0634/Crackme-with-muhemmed) | A crackme written to be broken: one small C binary, one hidden check, nothing else in the way. The exercise I hand to anyone who asks where to start with reversing. | `C` |
| [**ai-agent**](https://github.com/muhemmed0634/ai-agent) | Terminal chat agent over Gemini, with streamed, formatted output instead of a wall of raw text. | `Python` `google-genai` `rich` |
| [**Lənkəran Çay Dükanı**](https://github.com/muhemmed0634/tea-shopping) | Storefront for a real tea shop: catalog, cart, serverless order endpoint on Vercel and an admin page for the order list. | `HTML` `CSS` `JavaScript` |
| [**muhemmed0634-portfolio**](https://github.com/muhemmed0634/muhemmed0634-portfolio) | Personal site, dark by default, written by hand without a framework. | `HTML` `CSS` `JavaScript` |

## Currently

| Track | Where it stands |
| --- | --- |
| **OmidenOS** | Phase 2 verified. Next gate is a working disk install, then a signed and reproducible build. |
| **Nyx** | Terminal IDE for C and C++ in pure C, no dependencies. Design and keymap are settled; source is not published yet. |
| **Assembly** | Reading what the compiler emits instead of guessing from the debugger. Enough to follow a function frame, not enough to write it — yet. |

## How I build

- **Read it before rewriting it.** A stripped binary, a boot log or a stack trace
  tells you where the design actually breaks. Rewriting first just relocates the
  bug.
- **A claim needs a check behind it.** In OmidenOS a phase only closes when the
  build transcript and the boot test are recorded, and a negative test — BIOS must
  fail, not fall back — counts as evidence too. The same rule applies to these
  READMEs.
- **No dependency I cannot debug.** nmap-cli is C and CMake, nothing else; the
  live image carries only `[core]` and `[extra]`. Fewer layers means fewer places
  for a mystery.
- **Write the decision down.** Architecture decisions, phase exits and open items
  live in files, not in my head, so a month later the "why" is still there.

## Toolchain

| Layer | What I reach for |
| --- | --- |
| Languages | C, C++ (small utilities), Python 3, JavaScript, Shell, CMake, Make |
| Reversing | Ghidra, IDA Pro, gdb, `objdump`, `strings`, `strace` |
| Linux work | pacman-based distros, `mkarchiso`, `squashfs`, systemd-boot, UEFI, Calamares |
| Web / services | Node.js, discord.js, Vercel serverless, MongoDB |
| Daily | Linux, keyboard first, terminal open |

---

<div align="center">

<img width="440" src="https://github-readme-stats.vercel.app/api?username=muhemmed0634&show_icons=true&hide_title=true&hide_border=true&theme=dark&bg_color=0d1117&title_color=3fb950&icon_color=3fb950&text_color=c9d1d9" alt="GitHub stats">
<img width="400" src="https://streak-stats.demolab.com?user=muhemmed0634&theme=dark&hide_border=true&border_radius=8&background=0d1117&ring=3fb950&fire=3fb950&currStreakLabel=3fb950" alt="Commit streak">

<br>

<img width="380" src="https://github-readme-stats.vercel.app/api/top-langs/?username=muhemmed0634&layout=donut&hide_border=true&theme=dark&bg_color=0d1117&title_color=3fb950&langs_count=8" alt="Top languages">

<br>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=muhemmed0634&bg_color=0d1117&color=3fb950&line=3fb950&point=ffffff&area=true&hide_border=true" alt="Activity graph">

</div>

---

<div align="center">

<sub>If you want a binary reversed, a crackme broken down step by step, or a Linux problem narrowed to one line — email is the fastest way to reach me.</sub>

</div>
