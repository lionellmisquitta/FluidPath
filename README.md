# FluidPath

**Follow the flow. Find the loss.**

FluidPath turns funnel data into an animated, top-to-bottom water story. Each stage shows how much continues and where the flow leaks, helping an audience feel the journey instead of reading a wall of conversion numbers.

## Live app

[Open FluidPath](https://lionellmisquitta.github.io/FluidPath/)

## What it does

- Shows a working example before asking users to configure anything
- Accepts summarized stage totals or request-level event data
- Automatically suggests the order of event stages from average first-arrival time
- Lets users reorder, rename, remove, and visually merge stages
- Calculates unique stage reach for event-level data
- Animates flow and leakage from top to bottom
- Includes loop, flow-speed, and end-pause controls
- Supports custom colours and transparent backgrounds for presentation decks
- Exports presentation-ready PNG and animated GIF files
- Runs entirely in the browser; uploaded data does not leave the device

## Data options

### 1. Stage totals

Use one row per funnel stage:

```csv
stage,value
Applied,1043
Screened,721
Interviewed,384
Offered,146
Joined,112
```

### 2. Request-level events

Use one row for each request reaching a stage:

```csv
request_id,stage,timestamp
REQ-001,Applied,2026-01-03T09:00:00Z
REQ-001,Screened,2026-01-04T11:30:00Z
REQ-001,Interviewed,2026-01-08T14:00:00Z
REQ-002,Applied,2026-01-03T09:20:00Z
REQ-002,Screened,2026-01-05T10:15:00Z
```

FluidPath counts each request once per stage. Repeated status events therefore do not inflate stage reach.

## Use FluidPath when

- A hiring team wants to show where candidates leave a recruitment journey
- A sales team wants to communicate lead-to-customer conversion loss
- A service team wants to reveal where requests stall or drop out
- An onboarding team wants to show customer progress through activation
- A claims or approvals team wants to explain throughput across process stages

## Privacy

FluidPath is a self-contained browser app. CSV processing, animation, and export happen locally in the browser.
