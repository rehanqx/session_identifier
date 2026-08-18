# Smart Money Concepts — Clean Session Engine (v6)

A high-performance, clutter-free Pine Script (v6) session tracking engine designed for ICT/SMC traders. It dynamically plots key trading session ranges, tracks liquidity sweeps in real time, and auto-manages chart memory.

---

## 🌟 Key Features

* **Multi-Session Tracking:** Full support for Asian, London, New York, and London Close sessions with custom active hours and colors.
* **Real-time Liquidity Sweep Detection:** Session High/Low levels extend forward until price sweeps liquidity, then automatically freeze and turn dotted.
* **Clean & Minimal UI:** Single-label session identification placed cleanly above ranges, avoiding chart clutter.
* **Auto-Memory Cleanup:** Built-in history limiter (`history_days`) automatically purges old drawings to stay well within TradingView buffer limits (`max_lines_count`, `max_boxes_count`).
* **Live Status Dashboard:** Optional on-chart table showing active/inactive session states in real time.
* **Pine Script v6 Architecture:** Built using User-Defined Types (UDT) and array-based level tracking for speed and accuracy.

---

## 🕒 Default Session Hours (America/New_York)

| Session | Default Hours | Default Status |
| :--- | :--- | :--- |
| **Asian Session** | `20:00 - 00:00` | Enabled |
| **London Session** | `03:00 - 11:00` | Enabled |
| **New York Session** | `08:00 - 17:00` | Enabled |
| **London Close** | `11:00 - 13:00` | Disabled |

---

## ⚙️ Configuration & Inputs

* **Timezone & Lookback:**
  * `Timezone Selection`: Choose between `America/New_York`, `UTC`, `Europe/London`, `Asia/Tokyo`, or `Exchange`.
  * `Max Historical Days`: Restrict drawn boxes and lines (1 to 14 days) to keep charts fast and clean.
* **Visual Styling:**
  * `Show Session Shading Boxes`: Toggle range boxes.
  * `Show High/Low Lines`: Toggle session high and low lines.
  * `Extend Lines to Current Bar`: Projects key levels forward.
  * `Truncate Lines When Swept`: Freezes lines at the exact sweep candle.
  * `Show Status Dashboard`: Displays live session indicators in the top-right corner.

---

## 🚀 Installation & Usage

1. Open **TradingView** and navigate to the **Pine Editor** tab at the bottom.
2. Click **Create New Indicator** and remove any boilerplate code.
3. Paste the entire Pine Script v6 code into the editor.
4. Click **Save** and then click **Add to Chart**.
5. Adjust your preferred timezone and session timings from the indicator settings menu.

---

## 📜 License

Distributed under the MIT License. Feel free to use, modify, and integrate into your trading workflows.
