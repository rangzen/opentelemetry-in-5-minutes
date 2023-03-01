---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss

defaults:
  layout: 'center'

---

![Logo](/opentelemetry-horizontal-color.svg)

# Open Telemetry in 5 minutes

Software Crafters - Montreal - 2023-03-01


<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/rangzen" target="_blank" alt="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---

# Observability

> Observability is the ability to understand the internal state of a system by observing its external behavior.

- Logs (events in time)
- Metrics (time series)
- Traces (from Spans, unit of work)

<img src="/waterfall_trace.png" class="h-70 rounded shadow" />

---

# Open Telemetry (OTel)

> OpenTelemetry is a collection of tools, APIs, and SDKs.
> You can use it to instrument, generate, collect, and export telemetry data (metrics, logs, and traces)
> for analysis in order to understand your software's performance and behavior.

- Open Standard, so vendor-agnostic (no lock-in) through the SDK (all main languages) or the collector.
- Does not provide a backend nor a UI.
- Status:
  - Stable for tracing
  - Stable for metrics (SDK mixed)
  - Draft for logs.

See https://opentelemetry.io

---
layout: image
image: /otel_diagram.png
---