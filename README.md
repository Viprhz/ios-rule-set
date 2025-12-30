# ios-rule-set

Personal Surge rule sets with **semantic-first design**.

This repository contains self-maintained RULE-SETs for Surge,
aimed at solving real-world traffic classification issues that
generic third-party rule lists cannot cover well.

---

## Rule Sets

### 🎬 YouTube-Plus.list (v1.0)

**Purpose**

Full semantic & runtime coverage for YouTube traffic, including:

- Video playback & CDN
- YouTube internal APIs
- Google APIs used by YouTube runtime
- Account / Auth / Notification dependencies

This rule-set is designed to be placed **before Google.list** to
avoid being hijacked by generic `googleapis.com` rules.

**Usage (Surge)**

```ini
RULE-SET,https://raw.githubusercontent.com/<yourname>/ios-rule-set/main/surge/YouTube-Plus.list,"🎬 Streaming",no-resolve
