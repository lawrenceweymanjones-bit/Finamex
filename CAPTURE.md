# Capturing screens into Figma

Every screen can be opened directly with a deep link, and `&capture` renders it as a bare 393-wide phone at full length:

    http://localhost:PORT/?screen=<name>.<key>=<value>&capture

`chk` takes several values separated by `|`. Serve the folder locally (e.g. `python3 -m http.server 5197`), then ask Claude Code to capture with the Figma MCP `generate_figma_design` tool, using selector `.phone`. The page loads Figma's capture script itself when the URL carries a `#figmacapture=` hash.

Target: Finamex-Design (`GnAIyi1xRAcDQhfrNxEByi`), Sketches page, section "Wireframes v3 (Basis Grotesque)" (`314:1243`). Frames are named `WF – <screen>`.

## App

| Frame | Deep link |
|---|---|
| Home | `home` |
| Portfolio | `portfolio` |
| Explore | `explore` |
| Activity | `activity` |
| Notifications | `notif` |
| Menu drawer | `home.menu=1` |
| Goals | `goals` |
| Instrument detail | `instrument` |
| Order ticket | `order` |
| Action review | `review.code=5` |
| Confirmation & receipt | `receipt` |
| Stock detail · line | `stock.stock=WALMEX` |
| Stock detail · candles | `stock.stock=WALMEX.ctype=Candles` |
| Position detail | `position` |
| Deposit | `deposit` |

## Onboarding

| Frame | Deep link |
|---|---|
| Welcome | `welcome` |
| Location permission | `obLocation` |
| What you'll need | `obPrep` |
| 1 Create account | `ob1.chk=terms` |
| 2 Verify phone | `ob2.otp=3` |
| 3 Scan ID | `ob3.scan=1` |
| 4 Check details | `ob4.proof=1` |
| 5 Work & income | `ob5` |
| 6 Investing plans | `ob6.plan=Up to $50,000.freq=1–2 times a month` |
| 7 Bank account | `ob7` |
| 8 Review & sign | `ob8.chk=true|own|agree.plan=Up to $50,000` |
| Account open · add money | `obDone.notify=1.plan=Up to $50,000` |
| Prospect home (dropped out) | `prospect.obStep=5` |
| Locked action | `locked.obStep=5` |
| Location off | `obNoLoc` |
| Outside Mexico | `obOutside` |
| Demo home | `home.mode=demo` |
| Demo receipt | `receipt.mode=demo` |
