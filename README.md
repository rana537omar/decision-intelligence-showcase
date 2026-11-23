<p align="center"><img src="media/banner.png" alt="Decision Intelligence for Industrial Operations (Operations Optimization Platform): schedules, stock policy, routes and rosters, computed, approved and executed on autopilot" width="100%"></p>

# Decision Intelligence for Industrial Operations (Operations Optimization Platform)

**It computes the best operational plan it can find, then runs it for you.** Production schedules, stock policy, delivery routes and store rosters are worked out from your data, checked against guardrails you set, and approved and executed with no one involved. Your team only sees the exceptions.

> **This is a product showcase.** The software and its source code are proprietary and are **not** included in this repository. See [License](#license).

**Showcase website:** https://rana537omar.github.io/decision-intelligence-showcase/

<p align="center"><a href="https://wa.me/201208562225?text=Hello%2C%20I%20saw%20Decision%20Intelligence%20for%20Industrial%20Operations%20(Operations%20Optimization%20Platform)%20and%20I%20would%20like%20to%20get%20the%20full%20system%20and%20the%20source%20code."><img src="media/whatsapp-button.svg" alt="Get the full system and source code: chat on WhatsApp, +20 120 856 2225" width="380"></a></p>

## Demo video

<p align="center"><a href="https://rana537omar.github.io/decision-intelligence-showcase/#demo"><img src="media/video-poster.png" alt="Watch the product demo (3:28)" width="100%"></a></p>

A captioned walkthrough of 3 minutes 28 seconds, in 1080p. A visitor runs a real engine on the public site and books a session. Then the console: autopilot and its guardrails, each decision with today's practice beside the optimised plan, a line breakdown re-planned and executed with no one involved, a truck failure that autopilot holds for a person, and the data, API and reports behind it. **[Watch it on the showcase website](https://rana537omar.github.io/decision-intelligence-showcase/#demo)**.

## How it works

1. **Encode the operation.** Jobs, lines, SKUs, vehicles, stops, shifts and demand, kept current by API or CSV.
2. **Set the trade-offs.** What a late order, a changeover minute, a stock-out or an hour of overtime costs you.
3. **Compute and compare.** The engine returns the best plan it finds, always next to what today's practice would cost.
4. **Let it run itself.** Plans that pass your guardrails are approved and executed. The rest are held and raised as alerts.

## Features

### Five decisions
- **Manufacturing**: production sequencing across lines with family changeovers, maintenance windows, due dates and time-of-use energy tariffs.
- **Supply chain**: order quantity, safety stock and reorder point per SKU, with an optional working-capital budget.
- **Logistics**: vehicle routing with capacity, delivery windows, customer tiers and driver overtime.
- **Retail**: store rosters that follow hourly demand.
- **Demand**: a weekly forecast per SKU, checked against a naive forecast.
- **Decision chain**: the forecast feeds stock policy, replenishment becomes work orders, and the demand signal resizes routes and rosters, in one run.

### Autopilot
- **Manual, supervised or autonomous**, set per decision.
- **Re-computes** on a schedule, on every data change and on every logged disruption.
- **Guardrails**: minimum saving, maximum late jobs, maximum unserved stops, minimum on-time, fill rate and coverage.
- **Data-health checks** on every table; a critical issue blocks unattended execution.
- **One switch** pauses all automation.

### Exceptions only
- **Disruptions**: line breakdown, rush order, vehicle failure, same-day order, demand spike.
- **Alerts** for held plans and failed executions, with an optional webhook for team chat.
- **Audit trail** of every compute, approval and execution.

### Around it
- **API**: systems push data and events and read the plan in force.
- **Reports**: savings, autonomy rate, held decisions and daily volume, with CSV export and a print layout.
- **Public site** with a live demo that runs the real engines, and self-booked discovery sessions that are scored automatically.
- **Roles**: admin, operator, viewer.
- **Runs on your own server.** The engines are deterministic and run locally; no online AI service is used.

### Good to know
- The scheduling, routing and rostering engines are heuristic searches. They return the best plan found, not a mathematical proof of optimality.
- The ERP, MES, WMS, fleet and workforce connectors in this version are demo adapters that write to an outbox. A webhook connector sends decisions out for real; integrations with specific systems are built per client.
- The platform does not send email. A booked session is confirmed on screen with a calendar file.

## Screenshots

### Runs itself

| | |
|---|---|
| ![Command center](media/command-center.png) **Command center**: what ran, and what it is worth. | ![Autopilot](media/autopilot.png) **Autopilot**: mode, schedule and guardrails per decision. |
| ![Re-planned schedule](media/reoptimised-schedule.png) **Re-planned** around a breakdown and executed. | ![Held decision](media/held-decision.png) **Held**: outside the guardrails, so a person decides. |
| ![Alerts](media/alerts.png) **Alerts**: only what needs a person. | ![Monitor](media/monitor.png) **Monitor**: log a disruption, see what was sent out. |

### The decisions

| | |
|---|---|
| ![Production schedule](media/production-schedule.png) **Production schedule**: the optimised sequence. | ![Today's practice](media/production-baseline.png) **Today's practice**: late orders outlined in red. |
| ![Route plan](media/route-plan.png) **Route plan**: capacity, windows and tiers respected. | ![Stock policy](media/inventory-policy.png) **Stock policy**: per SKU, with what to order now. |
| ![Store roster](media/store-roster.png) **Store roster**: cover that follows demand. | ![Demand forecast](media/demand-forecast.png) **Demand forecast**: per SKU, with its error. |
| ![Decision chain](media/decision-chain.png) **Decision chain**: five linked decisions in one run. | ![Production decision](media/production-decision.png) **A decision page**: trade-offs on the left, result on the right. |

### Data, reports and the public site

| | |
|---|---|
| ![Encoded data](media/encoded-data.png) **Encoded data**: editable, with health checks. | ![Integrations and API](media/integrations-api.png) **Integrations and API**: connectors and keys. |
| ![Reports](media/reports.png) **Reports**: savings, autonomy rate, daily volume. | ![Discovery requests](media/discovery-requests.png) **Discovery requests**: self-booked and scored. |
| ![Live demo](media/site-live-demo.png) **Live demo** on the public site, no sign-up. | ![Booking](media/site-booking.png) **Self-serve booking** with a calendar file. |
| ![Public site](media/site-hero.png) **Public site**: the landing page. | ![Sign in](media/sign-in.png) **Sign in** to the console. |

<p align="center"><img src="media/phones.png" alt="The public site, command center and autopilot on phones" width="80%"></p>

The company, products, customers, people and figures in these screenshots and the video are fictional demo data created for this showcase. Savings are measured against simple rule-of-thumb planning on that demo data and are not real results or a promise of results.

## Get the full system

Want this platform for your operation or your clients, a live demo, or the complete source code? Message me on WhatsApp: **+20 120 856 2225**.

<p align="center"><a href="https://wa.me/201208562225?text=Hello%2C%20I%20saw%20Decision%20Intelligence%20for%20Industrial%20Operations%20(Operations%20Optimization%20Platform)%20and%20I%20would%20like%20to%20get%20the%20full%20system%20and%20the%20source%20code."><img src="media/whatsapp-button.svg" alt="Get the full system and source code: chat on WhatsApp, +20 120 856 2225" width="380"></a></p>

## License

**Copyright © 2026 Rana Omar. All rights reserved.** The text, screenshots, images and video in this repository are shared for viewing only. No license is granted to copy, reuse, modify, republish or use them, or the software they show, for any personal or commercial purpose. See [LICENSE](LICENSE).
