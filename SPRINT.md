# Sprint

**Author:** Troy

Eval-first. Fine-tune is not this sprint.

Landscape stays in [SPEC.md](SPEC.md). This file is the order.

**Freeze the eval before any train.**

## This sprint

1. **`eval/v0.jsonl`.** 20–40 lines. English, Tagalog, affixed Taglish (`nag-meeting`, `i-submit`, `ina-update`), particles (`po`, `opo`, `na`, `pa`), at least one non-Manila note. Version `v0`. Frozen. Do not train against it after freeze.

2. **Optional listen-able peek.** Meta MMS `facebook/mms-tts-tgl` reading a subset. Label those clips **NC** (CC-BY-NC 4.0). Skip if no GPU — the eval file alone is a legal peek.

## Done

`eval/v0.jsonl` is on main. An NC-labeled MMS peek is extra, not required. That is the sprint.

Training waits for a later named sprint.

## Kill

- Train
- LoRA
- Discord-as-community
- Voice clone
- MOS
- Swapping the MMS baseline
- Calling an MMS fine-tune community-usable
