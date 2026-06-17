# Free LLM Coding Credits

> A curated list of LLM inference platforms that hand out free credits you can use as AI coding models. *Updated regularly.*

> **Last updated:** 17 Jun 2026, 03:01 GMT

## What is this?

This repository tracks **LLM inference sites** that currently give away **free credits** usable for AI-assisted coding — limited-time model promos, free signup credits, trial tiers, and the like. The goal: keep a fresh stack of free/cheap providers so you can keep coding with strong models for as little as possible *right now*.

> **Don't underestimate "just $1."** It sounds tiny, but with today's **cheap-yet-capable Chinese models** (DeepSeek V4 Flash/Pro, Qwen3.6/3.7 Plus/Max, GLM, MiMo 2.5/2.5 Pro, MiniMax, etc.) a single dollar stretches a *surprisingly* long way — these models are genuinely powerful now, not toys. Then **aggregate the free credits across all the providers below**, and suddenly you've got a *lot* of real coding capacity for free.

> **This is a living list, not a "free forever" promise.** These are time-sensitive offers. As promos and signup-credit deals expire, those entries get **removed**, and newly discovered offers get **added**. Always check each provider's current terms before relying on it.

> **How entries are vetted:** Almost every provider here is **personally tested whenever possible** before it's added — confirming the free offer is real, the API key actually works, and the model is usable for coding. This list deliberately **skips dubious LLM aggregators / key resellers** (e.g., *AgentRouter*, *BluesMinds*, and similar) where reliability is low — think flaky auth (`UNAUTHENTICATED` errors), inconsistent uptime, models that don't match their labels, or sketchy "$200–300 free credit" hooks. As a rule of thumb, prefer first-party providers or well-known gateways over no-name resellers, and never paste your own paid API keys into an unknown aggregator.

## The strategy

The real power comes from combining these platforms together.

1. **Aggregate the free credits** from each platform listed below. Although some might need their own harness tools and/or doesn't expose API keys, most of them have API keys and/or can be connected with 9router.
2. **Route everything through [9router](https://9router.com)** — use it as your single API-key layer so your coding tools talk to one endpoint while you draw from many providers behind it.
3. **Pick cheap-but-strong Chinese models** that punch well above their cost, for example:
   - **DeepSeek V4 Pro / V4 Flash**
   - **MiniMax M3**
   - **MiMo 2.5 / 2.5 Pro**
   - **Kimi K2.6**

Stacked together, this setup will **last you many tasks essentially for free** while still giving you frontier-level coding help.

> Tip: spread your usage across providers so no single free tier runs dry — 9router makes this seamless behind one API key.

## Platforms (free credits)

*The list below will be filled in and updated regularly as each platform is researched.*

1. [**Qoder**](https://qoder.com) (by Alibaba)
   - **Free credits:** 200 free Qwen3.7-Max calls/day, reset at midnight; after 200, the half-price rate still applies. Limited-time promo (started Jun 1, 2026, end date TBA).
   - **Usable models:** Qwen3.7-Max (1M context, OpenAI/Anthropic-compatible).
   - **Coding-ready?** Yes — agentic coding IDE; Qwen3.7-Max excels at multi-file engineering.
   - **Eligibility:** All users (Community, Pro Trial, Pro/Pro+/Ultra/Teams). Available on Qoder Desktop, JetBrains plugin, and CLI. Auto-activated — just log in and select Qwen3.7-Max.
   - **9router — supported, but questionable:** Qoder doesn't hand you a raw API key, so 9router routes it via an **unofficial OAuth login** (intercepting the IDE/CLI subscription through its OAuth / cookie / MITM bridge). This login method is **not sanctioned by Qoder** and can **trigger an account / IP / device ban**. So while it *technically* works, the **official harness is strongly preferred** — use the free Qwen3.7-Max quota directly in Qoder Desktop, the JetBrains plugin, or the CLI.

2. [**TokenRouter**](https://www.tokenrouter.com) (by [PaleBlueDot.AI](http://PaleBlueDot.AI))
   - **Free credits:** Limited-time promo — **MiniMax M3 free**, plus all MiniMax models 50% off. (New-user developer credits also advertised.)
   - **Usable models:** MiniMax-M3 (free), plus 50+ others (DeepSeek, Kimi, GPT, Claude, Gemini, GLM, Qwen, Nemotron) via one unified, OpenAI-compatible gateway.
   - **Coding-ready?** Yes — MiniMax M3 is a frontier open-weight coding/agentic model (1M context, ~59% SWE-Bench Pro).
   - **API key:** Exposes a standard API key (base URL `https://api.tokenrouter.com/v1`, model `MiniMax-M3`), so it **works with 9router** and any OpenAI-compatible coding tool.

3. [**0G Private Computer**](https://pc.0g.ai) (by 0G Labs)
   - **Free credits:** **100% FREE MiniMax M3** during a 3-day launch campaign, **June 15–18, 2026 (12:00 UTC)**. $0 cost — you just need ~1 $0G in your account to verify you're a real user. No application flow.
   - **Usable models:** MiniMax-M3 (free during the campaign), plus other models (e.g., GLM) on the decentralized compute network.
   - **Coding-ready?** Yes — MiniMax M3 is a frontier coding/agentic model (1M context, ~59% SWE-Bench Pro).
   - **API key:** Exposes an OpenAI-compatible Router endpoint (base URL `https://router-api.0g.ai/v1`, API key `sk-...`), so it **works with 9router**. It's a decentralized/on-chain platform — inference runs inside hardware-isolated TEE enclaves (private + verifiable).
   - **Note:** The free MiniMax M3 window is short (Jun 15–18). After it ends, it reverts to pay-per-use (payable via crypto or, per 0G, credit/debit card).

4. [**SiliconFlow**](https://www.siliconflow.com)
   - **Limited-time FREE: [Nex-N2-Pro](https://www.siliconflow.com/models/nex-n2-pro)** — currently **$0.00 / M tokens** (both input *and* output) on SiliconFlow serverless. This is the headline deal: a frontier open-weight agentic coding model running for free right now.
     - **Why it matters:** Nex-N2-Pro (by Nex AGI, Apache 2.0, 397B MoE / 17B active, built on Qwen3.5) rivals GPT-5.5 & Claude Opus 4.7 on coding — **80.8 SWE-Bench Verified, 75.3 Terminal-Bench 2.1, 58.8 SWE-Bench Pro**, with a **262K context**. Plug-and-play with Claude Code, Cursor, and agentic harnesses.
     - **Note:** The $0 pricing is promotional/limited-time — grab it while it lasts. (Also available free on OpenRouter as `nex-agi/nex-n2-pro:free`.)
   - **Free credits:** **$1 in free credits** on signup, no minimum commitment — usable on its 200+ pay-as-you-go models (incl. DeepSeek V4 Pro, GLM-5.1, Kimi, Qwen3-Coder, MiniMax). Plus a handful of **permanently free** models.
   - **Other currently free models:** small open models such as `Qwen/Qwen3-8B`, `deepseek-ai/DeepSeek-R1-Distill-Qwen-7B`, and `deepseek-ai/DeepSeek-OCR` (free list changes over time — look for models marked "Free" in the model list).
   - **Coding-ready?** Partially — the *permanently free* models are small; for strong coding, spend the $1 credit on a bigger model (e.g., DeepSeek V4 Pro / Kimi K2.6).
   - **Rate limits:** Free models capped at ~50 req/day; a small lifetime top-up (>=10 CNY) raises it to ~1,000 req/day.
   - **API key:** Exposes a standard API key (base URL `https://api.siliconflow.com/v1`), so it **works with 9router**.

5. [**Xiaomi MiMo**](https://platform.xiaomimimo.com) (Xiaomi MiMo API Open Platform)
   - **Free credits:** ~**$0.72 welcome bonus** on signup, plus an extra **$2** if you redeem another user's invite code or your friend redeems your invite code → **~$2.72 total** to start. (Xiaomi's official *Refer & earn*: both the inviter and invitee get **$2** in trial credits, granted instantly.)
     - **Repo owner's invite code: `GVLMCK`** — enter it when you sign up to (hopefully) grab the extra $2. *Not guaranteed:* the free-$2 reward is capped at **30 redemptions per code**, so if this one is already full it won't pay out. The code here will be **swapped/refreshed/deleted** once it fills up.
   - **Usable models:** `mimo-v2.5-pro` (flagship — 1T params / 42B active, **1M context**, MIT-licensed, rivals Claude Opus 4.6 on agentic coding) and `mimo-v2.5` (native multimodal, 1M context), plus the older V2 series.
   - **Why ~$2.72 stretches far:** MiMo took a **permanent price cut (up to ~99%)**, and it's *especially* cheap on **cache hits** — MiMo-V2.5-Pro runs ~$1.31/M input (cache miss) & $2.61/M output, but only **~$0.011/M on a cache hit**; MiMo-V2.5 drops to **~$0.003/M on a cache hit**. Agentic coding tends to hit cache often, so that small bonus goes a long way. (Cache *writes* are temporarily free.)
   - **Coding-ready?** Yes — built for agentic/long-horizon coding; works out-of-the-box with Claude Code, OpenClaw, OpenCode, KiloCode, and Cline.
   - **API key:** Exposes a standard OpenAI- & Anthropic-compatible API key (base URL `https://api.xiaomimimo.com/v1`), so it **works with 9router**.
   - **No-login option — MiMo Code + "MiMo Auto":** Xiaomi's open-source terminal coding agent [**MiMo Code**](https://github.com/XiaomiMiMo/MiMo-Code) ships with a built-in **"MiMo Auto"** channel that's *free for a limited time*, zero-config, and *fully anonymous — no login, no API key*. It runs **MiMo-V2.5** (1M context), so you can start coding instantly. Install with `curl -fsSL https://mimo.xiaomi.com/install | bash` (macOS/Linux) or `npm install -g @mimo-ai/cli` (Windows). **Routable via 9router, but questionable:** 9router can pull it in via an **unofficial OAuth / cookie / MITM-bridge interception** that isn't sanctioned and can **trigger an account / IP / device ban**. So while it works, the **official harness is strongly preferred** — run the free MiMo-V2.5 quota directly inside MiMo Code.
   - **Notes:** Requires a *Xiaomi account* to sign up. Each invitee can redeem *only one* code. The free-$2 signup reward is capped at the **first 30 redemptions per inviter** (Xiaomi's "signup-credit quota: 30 slots") — after that, neither side gets the $2. Bindings beyond 30 are still allowed, and those later invitees still get **10% off** their first Token Plan order while the inviter earns **10% credits back** on a friend's first paid order (first 30 paid orders, within a 30-day window). So your invitees' *purchases* keep paying off even after the free-$2 slots run out.

6. [**ZenMux**](https://zenmux.ai) (enterprise LLM gateway)
   - **Free credits:** Two **limited-time FREE** model promos running right now ($0 while they last):
     - **StepFun Step 3.7 Flash — free for ~1 month** (per StepFun's own announcement). A 198B sparse-MoE **vision-language** model (~11B active/token), **256K context**, up to ~400 tok/s, with 3 selectable reasoning levels (low / medium / high).
     - **Kimi K2.7 Code — limited 7-day free trial** (per ZenMux). Moonshot's most capable coding model: **+21.8% Kimi Code Bench v2**, +11% Program Bench, +31.5% MLS Bench Lite vs K2.6, with **~30% fewer reasoning tokens** (less overthinking). A HighSpeed variant (~180–260 tok/s) is also listed.
   - **Usable models:** 200+ in total (Claude, GPT, Gemini, GLM, MiMo, DeepSeek, Qwen, Kimi...), but the genuinely *free* ones right now are the **two above**.
   - **Coding-ready?** Yes — both promo models are built for agentic coding and work with Claude Code, OpenClaw, Cursor, and other OpenAI/Anthropic-compatible tools.
   - **API key:** Standard OpenAI- & Anthropic-compatible API key (base URL `https://zenmux.ai/api/v1`, plus `https://zenmux.ai/api/anthropic`), so it **works with 9router**. Bonus: ZenMux offers "AI Model Insurance" that compensates you for subpar/hallucinated output.
   - **Notes:** Both deals are *time-boxed* (Step 3.7 Flash ~1 month, Kimi K2.7 Code 7 days) — after they end, those models revert to paid. ZenMux's *general* free tier is **tight** (reportedly ~$0.16 per rolling 5-hour window, and you must keep a positive balance), so treat this as "free **for these two models, for now**," not an unlimited free tier.

7. [**Novita AI**](https://novita.ai) (AI-native cloud / model gateway)
   - **Nex-N2-Pro — currently Free / Free** here too (same limited-time $0 deal as on SiliconFlow).
   - **Free credits:** **$1 free credit** granted automatically on signup (no credit card; sign up with Google / GitHub / Hugging Face / email). New accounts also get **$100 in Agent Sandbox credits** (valid 90 days) if you build agents there.
   - **Why it's great for cheap Chinese models:** Novita hosts 200+ open models and is one of the cheapest places to run the strong Chinese ones. Standout cheap picks (serverless, per 1M tokens):
     - **DeepSeek V4 Flash** — **$0.14 in / $0.28 out** (cache read $0.028), **1M context** — absurdly cheap flash-class model.
     - **DeepSeek V4 Pro** — $1.6 in / $3.2 out (cache $0.135), 1M context.
     - **MiMo-V2.5** — $0.168 in / $0.336 out (cache $0.0034); **MiMo-V2.5-Pro** $0.522 / $1.044.
     - **Kimi K2.6** — $0.8 / $3.4; **Kimi K2.7 Code** $0.95 / $4.
   - **Coding-ready?** Yes — use Nex N2 Pro and pair the $1 credit with a dirt-cheap model (DeepSeek V4 Flash, etc) and it stretches into millions of tokens.
   - **API key:** OpenAI-compatible (base URL `https://api.novita.ai/openai`), so it **works with 9router** and any OpenAI-style coding tool.
   - **Note:** The $1 is a *one-time* signup credit (not recurring) — but on these cheap models that's still a lot of tokens. Prices above change over time; check the live pricing page before relying on them.

8. [**Z Code (ZCODE)**](https://zcode.z.ai) (by [Z.ai](http://Z.ai) / Zhipu)
   - **Free credits:** A **limited-time launch promo** tied to the GLM-5.2 release (Jun 13, 2026): a generous **free daily quota** inside [Z.ai](http://Z.ai)'s own coding harness — reportedly **~3M tokens/day of GLM-5.2** and **~2M tokens/day of GLM-5-Turbo**, running **until ~June 19, 2026**.
   - **What is ZCODE?** [Z.ai](http://Z.ai)'s own **agentic development environment** — a GUI desktop app (macOS/Windows) plus coding CLI that can run **multiple collaborating agents**, work over SSH / remote machines, and use built-in **skills** (e.g. an auto-triggered "frontend design" skill) and **MCP** services.
   - **Usable models:** **GLM-5.2** (flagship — **1M context**, two thinking-effort levels High/Max, MIT open weights announced; rivals Claude Opus-tier coding) and **GLM-5-Turbo** (fast, agent-optimized variant for long execution chains).
   - **Coding-ready?** Yes — purpose-built for agentic coding; GLM-5.2 is one of the strongest open Chinese coding models right now.
   - **9router compatibility — caution:** Unlike most entries here, this free quota is best used **directly inside ZCODE / officially supported tools**. [Z.ai](http://Z.ai)'s GLM Coding Plan terms **restrict usage to officially supported tools** and explicitly warn that **SDK-based or third-party access may have benefits throttled or blocked**. So routing the free quota through 9router (or other proxies) risks getting restricted — treat ZCODE as a use-it-in-the-harness deal, not a 9router source. (If you do want API access, the GLM Coding Plan endpoint is `https://api.z.ai/api/coding/paas/v4`, Anthropic/OpenAI-compatible.)
   - **Note:** This is a short launch-window freebie (~until Jun 19). After it ends, GLM-5.2 / GLM-5-Turbo revert to consuming normal Coding Plan quota (paid subscription, from ~$3–$18/mo for the Lite tier).

9. [**UniModel.ai**](http://UniModel.ai) (NewAPI-based unified gateway)
   - **Free credits:** **~$10 in free credits** on signup *(per the current promo — confirm in-app, as the exact amount isn't published on the landing page)*.
   - **What it is:** A unified API **gateway** built on the open-source **NewAPI** stack — it aggregates **50+ upstream providers** and **100+ models** behind one OpenAI / Anthropic / Gemini-compatible endpoint (`/v1/chat/completions`), with multi-key routing, load balancing, and real-time usage tracking.
   - **Usable models:** A broad mix routed from upstreams — GPT, Claude, Gemini, plus the cheap Chinese models (DeepSeek, Qwen, GLM, Kimi, MiniMax). Spend the free credit on the cheap Chinese ones for maximum mileage.
   - **Coding-ready?** Yes — OpenAI/Anthropic-compatible; works with Claude Code, Cherry Studio, CC Switch, and similar tools.
   - **API key:** Standard OpenAI-compatible key, so it **works with 9router** and any OpenAI-style coding tool.
   - **Note:** UniModel is a NewAPI-style management platform (you configure channels/keys), and the **$10 figure is promo / user-reported** — verify the current welcome credit after signing up.

10. [**Zyloo**](https://zyloo.io) (unified API at "the cheapest price")
    - **Free credits:** **$5 free** welcome credit on signup.
    - **Supports Claude (paid, not free):** Yes — **9 Anthropic models** are available, e.g. Claude Fable 5 / Opus 4.7–4.8 at **$5 / $25** per 1M, **Opus 4.6 at $3 / $20**, down to a cheaper Claude at **$1 / $5** (200K ctx). All pay-per-token from your $5 credit.
    - **Usable models:** **34 models across 10 providers** behind one OpenAI-compatible endpoint — Anthropic (9), OpenAI (6), Google (2), xAI (3), DeepSeek (3), Moonshot/Kimi (3), Qwen (3), Zhipu/GLM (1), MiniMax (2), Xiaomi/MiMo (2).
    - **Cheapest picks to stretch the $5:** DeepSeek at **$0.098 / $0.20** per 1M, Xiaomi MiMo at **$0.14 / $0.28**, DeepSeek $0.20 / $0.30, MiniMax $0.20 / $0.80 — all strong value for coding.
    - **Coding-ready?** Yes — frontier coding models (Claude Opus, GPT-5.5, Kimi) are all available; just swap your `baseURL`.
    - **API key:** Standard OpenAI-compatible key (base URL `https://zyloo.io/v1`, key `sk-zy-...`), so it **works with 9router**.

11. [**Berget AI**](https://berget.ai) (EU / Swedish sovereign inference)
    - **Free credits:** **€5 free starting credits** on the Free plan (pay-as-you-go after that; any leftover balance rolls over).
    - **Optimal pick — Kimi K2.6:** open-weight **SOTA coding / agent** model (1T params, **256K context**, agent-swarm capable) at roughly **~88% cheaper than Claude Opus** — the best value here for serious coding.
    - **Usable models (open only):** **Kimi K2.6**, **GLM-4.7** (confirmed in their lineup), DeepSeek, Llama 3.3 70B, Mistral Small 3.1, Qwen3, GPT-OSS 120B, plus rerank / moderation / speech models. *(Berget hosts open models only — no GPT / Claude / Gemini. The list changes, so check their models page.)*
    - **Coding-ready?** Yes — purpose-built for agentic apps; pair the €5 with Kimi K2.6. There's also a dedicated **"Berget Code"** agentic-coding product (OpenCode / Pi integrations, currently waitlist).
    - **API key:** OpenAI-compatible (base URL `https://api.berget.ai/v1`; set up via `npx berget auth login` then `npx berget api-keys create`), so it **works with 9router**.
    - **Bonus:** EU-hosted, **100% fossil-free** electricity, and data stays inside EU borders — the privacy / sovereignty-friendly option.

12. [**TokenLab**](https://tokenlab.sh) (agent-first AI gateway)
    - **Free credits:** **~$1 in trial credits** on signup (no card) — enough to make real calls and test fit before topping up pay-as-you-go.
    - **What it is:** A one-key **AI gateway** to **200+ models** (text, image, *and* video) with both **native and OpenAI-compatible routes**, auto-failover, agent-readable errors, and a claimed **30–70% lower cost** than going direct.
    - **Usable models:** GPT 5.5, **Claude 4 family** (Sonnet / Opus / Haiku 4.x — incl. 4.5 / 4.6), Gemini 3, DeepSeek, Meta (Llama), Mistral, Perplexity, Cohere — plus image/video (Nano Banana, Flux, Veo 3, Seedance, Midjourney, Luma).
    - **Coding-ready?** Yes — frontier coding models (GPT 5.5, Claude 4.6, DeepSeek) are available; spend the $1 on a cheap model to stretch it.
    - **API key:** Standard OpenAI-compatible key (point your `baseURL` at TokenLab with a TokenLab key; endpoint `/v1/chat/completions`), so it **works with 9router**. *(Tip: for native Claude/Gemini features like prompt caching & thinking mode, use the matching native routes.)*
    - **Note:** The $1 is a one-time trial credit; on premium models (GPT / Claude) it won't go far — pair it with a cheap model for real mileage.

13. [**Inference.net**](http://Inference.net) (full-stack LLM lifecycle platform)
    - **Free credits:** **~$1 free credit** on signup to make real API calls, then pay-as-you-go.
    - **What it is:** A deploy / observe / train / evaluate platform for production agents, serving open models through **OpenAI-compatible APIs** (SOC 2 Type II).
    - **The coding pick — Nemotron 3 Super:** NVIDIA's open **hybrid Mamba-Transformer MoE** (120B total / 12B active, **1M context**, tool calling, fully open weights) built for **agentic reasoning** — **the only model here strong enough for real coding**. Priced **$2.50 / $5.00** per 1M tokens.
    - **Other models (specialized, not general coding):** *Schematron V2 Turbo* ($0.03 / $0.15) & *Small* ($0.05 / $0.25) — structured-output / JSON reasoning models; *ClipTagger 12B* ($0.30 / $0.50) — a vision model for video understanding. There's also a dedicated-GPU deploy catalog (Kimi K2.5, MiniMax-M2.5, GLM-5, GPT-OSS 120B at ~$9.98/hr on B200) if you'd rather self-host.
    - **Coding-ready?** Yes, via **Nemotron 3 Super** — the rest are small / task-specific. At $2.50 / $5 it's pricier than the cheap Chinese models, so $1 ≈ a few hundred K tokens; best for focused agentic runs.
    - **API key:** OpenAI-compatible, so it **works with 9router** and any OpenAI-style coding tool.

14. [**Avian**](https://avian.io) (fast, affordable inference API)
    - **Free credits:** **~$1 free** to start (add credits, no subscription) — pay-per-token after.
    - **What it is:** A speed-focused inference API — all models run on **NVIDIA B200 GPUs with speculative decoding**, claiming the **fastest DeepSeek V3.2 inference** (~489 tok/s, ~4× OpenAI) with **no rate limits**. Built-in vision, web search / reader, and native tool calling.
    - **Usable models (per 1M tokens, in / out):**
        - **DeepSeek V4 Flash** — **$0.105 / $0.21** (1M ctx) — cheapest pick.
        - **DeepSeek V3.2** — $0.23 / $0.33 (163K); **DeepSeek V4 Pro** — $1.305 / $2.61 (1M ctx).
        - **MiniMax M2.5** — $0.27 / $1.08 (196K).
        - **GLM-5** — $0.95 / $2.55 (205K); **GLM-5.1** — $1 / $3.2 (202K).
        - **Kimi K2.5** — $0.45 / $2.2 (262K); **Kimi K2.6** — $0.95 / $4 (262K).
    - **Coding-ready?** Yes — works with **Claude Code, Cursor, Cline, Windsurf, Kilo Code, Aider** (20+ tools); pair the $1 with DeepSeek V4 Flash for a *lot* of fast tokens.
    - **API key:** OpenAI-compatible (base URL `https://api.avian.io/v1`, model e.g. `DeepSeek-V3.2`), so it **works with 9router**.

15. [**EmberCloud**](https://embercloud.ai) (serverless GPU inference)
    - **Free credits:** **~$1 free** on signup — serverless, **zero cold starts**, pay only for what you generate.
    - **What it is:** Serverless GPU inference for **open-source models** with drop-in OpenAI APIs — effectively a **GLM specialist**, with very cheap **cached-input** rates.
    - **Usable models (per 1M tokens, in / out):**
        - **GLM 4.7 Flash** (30B MoE) — **$0.060 / $0.400** (200K) — cheapest.
        - **Qwen3 Coder Next** — $0.108 / $0.675 (262K); **GLM 4.5 Air** — $0.130 / $0.850 (131K).
        - **GLM 4.6** (Code) — $0.380 / $1.55 (200K); **GLM 4.7** (355B MoE) — $0.380 / $1.98 (200K).
        - **GLM 5** (745B MoE) — $0.720 / $2.30 (203K); **GLM 5.1** — $0.931 / $2.93 (203K).
        - **Kimi K2.5** — $0.405 / $1.98 (262K); **MiniMax M2.5** — $0.200 / $1.20 (196K); plus **GLM 4.5 / 4.5V** (vision).
    - **Coding-ready?** Yes — strong GLM coding line (GLM 4.6 "Code", GLM 5 / 5.1) plus **Qwen3 Coder Next**; cached input is dirt cheap (e.g. GLM 4.7 Flash $0.010/M cached), so agentic loops stretch the $1 far.
    - **API key:** OpenAI-compatible (base URL `https://api.embercloud.ai/v1`, key `ember_sk_...`, model e.g. `glm-4.7`), so it **works with 9router**.

16. **OrcaRouter** (by Continuum AI)
    - **Free credits:** **$1 in free tokens** on signup with **GitHub** (no credit card). Key kicker: **zero markup** — you spend it at each provider's *exact* published rate, so $1 goes further than on gateways that add a 5–20% spread.
    - **What it is:** An OpenAI-compatible **meta-router** over **200+ models** that grades each prompt and routes it (`orcarouter/auto`) to the best frontier or open model. MIT-licensed open core (OrcaRouter Lite), backed by published research and independently audited — so it clears the "no sketchy reseller" bar.
    - **Sampled catalog (provider cost price, per 1M in / out):** `deepseek-v4-flash` **$0.147 / $0.294** (1M ctx, cheapest pick), `deepseek-v4-pro` $0.456 / $0.910, `qwen3.7-plus` $0.350 / $1.42, `kimi-k2.7-code` $0.950 / $4.00 (262K), `glm-5.2` $1.40 / $4.40. Frontier also available at direct price (Claude Opus 4.8, GPT-5.5, Gemini 3.5 Flash).
    - **Coding-ready?** ✅ Yes — works with Cursor, Cline, OpenClaw, and Claude Code; spend the $1 on DeepSeek V4 Flash for millions of tokens.
    - **✅ API key:** OpenAI-compatible (base URL `https://api.orcarouter.ai/v1`, key `sk-orca-...`, model e.g. `orcarouter/auto`), so it **works with 9router**.
    - **⚠️ Note:** The $1 is a **one-time** signup credit; as a router, latency/availability ride on upstream providers (auto-failover across 200+ models helps).

## Contributing

This list is maintained continuously and intentionally **churns**: expired promos and ended signup-credit offers are **deleted**, freshly discovered ones are **added**, and existing entries are updated when terms change. If an offer here has ended, it'll be pruned on the next update.

---

*Disclaimer: Free-credit offers, model availability, and provider terms change frequently. Always verify current terms on each provider's site before relying on them.*
