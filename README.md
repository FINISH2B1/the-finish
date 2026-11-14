# The Finish

Lucypatina — The Finish. A painter's finish companion, built under International AIDAY623 LLC. Built for NEAR HACKATHON (Privacy & Private AI track).

## What it is

A working prototype. A painter enters the surface, the paint, the temperature,
and the humidity. The Finish returns the finish call: the right primer, the
right paint, the cure schedule — dry to touch, safe to recoat, fully cured —
computed from real cure math, with honest warnings when the conditions will
ruin the work.

A cure tracker logs each coat and counts down to touch, recoat, and full cure,
so nobody has to guess.

## Private by design

There is no account, no cloud, and no tracking. Every job lives in the
device's own storage and nowhere else. Nothing typed here is sent anywhere,
because there is nowhere to send it to. A painter's jobs are the painter's.

## How to run

Open `index.html` in any browser. No build step, no dependencies, no server.

## The engine

Base cure times are set at 70°F / 50% relative humidity and adjusted for the
job's actual temperature and humidity:

| Paint | Dry to touch | Safe to recoat | Fully cured |
|-------|--------------|----------------|-------------|
| Latex / acrylic | 1 hr | 4 hrs | 14 days |
| Oil / alkyd | 8 hrs | 24 hrs | 7 days |
| Epoxy | 6 hrs | 16 hrs | 7 days |
| Lacquer | 30 min | 1 hr | 1 day |
| Stain | 2 hrs | 6 hrs | 3 days |

Cold slows the cure (about 1.8x per 10°F below 70°F). High humidity stretches
it further. The app warns plainly when the conditions will fail a finish —
latex below 50°F does not form a film at all, and it will tell you to wait
for a warmer day or switch to oil.

## Built by

William Jaworske — a painter of 27 years, Cleveland, Ohio. He formed International AIDAY623 LLC. His lifelong decisions to become and stay a painter led to her build and synthesis. The finish is never finished — it is
always curing.

## License

MIT
