# DESIGN.md

## Overview

Control / Room is a dark-first status snapshot with a service matrix, incident log, and one clearly labeled advisory state. It is intentionally operational rather than celebratory.

## Colors

- Graphite `#101210` is the control-room ground; panel `#181b18` carries the matrix.
- Paper `#e7e5d6` is the primary reading color.
- Green `#b6d33c` means operational and clear.
- Amber `#f3b84f` means monitoring/advisory; red remains reserved for future incidents.

## Typography

- Trebuchet MS supplies the compact control-room UI voice.
- Courier New is reserved for telemetry labels, status states, and sample-data boundaries.
- Headings are heavy and compressed; table values stay tabular and easy to scan.

## Layout

- The hero establishes the operational thesis and current snapshot.
- A signal strip sets overall, services, incidents, and time window before the matrix/log split.
- Mobile stacks service matrix and incident log while preserving the advisory beneath both.

## Elevation & Depth

Panel boundaries use one-pixel rules and a single-axis scanline texture. There are no shadows, blur, or simulated live chart effects.

## Shapes

Rectangular panels, square state markers, hairline rules, and small outlined range controls. The system should feel like a control surface, not a rounded analytics dashboard.

## Components

- Time-window buttons for 24h, 7d, and 30d sample views.
- Service matrix with uptime, state, and status markers.
- Empty incident log with clear sample-data explanation.
- Advisory strip showing a non-green monitoring state without inventing an incident.

## Do's and Don'ts

- Do label every metric as sample data and keep status semantics explicit.
- Do use green/amber/red as meaning-bearing state colors, never decoration.
- Don't claim live monitoring, notifications, uptime guarantees, or incident history.
- Don't turn the matrix into a hero-metric card collection.
