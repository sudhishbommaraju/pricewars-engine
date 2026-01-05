# PriceWars Engine
### A pricing simulation for local competitive markets

PriceWars is a project I built to explore how prices change over time in real local markets when businesses react to each other instead of setting prices in isolation.

Most pricing tools treat prices as fixed inputs. This project does the opposite: it models how businesses **respond** when a competitor raises or lowers prices, and how those reactions shape the entire market over time.

I was interested in questions like:
- What actually causes price wars?
- When do markets settle into stable pricing?
- When is cutting prices a bad idea?
- How much pricing power does a business really have?

---

## Why I Built This

Local businesses make pricing decisions all the time, often without knowing how competitors will respond. I wanted to understand pricing as a **system**, not just a single decision.

This project is my attempt to combine ideas from:
- microeconomics (supply, demand, elasticity)
- business strategy
- simple simulation and modeling

The goal isn’t to predict exact outcomes, but to understand **patterns and incentives**.

---

## What the Simulation Does

For a given local market (for example: coffee shops, gyms, tutoring centers), the engine simulates multiple businesses competing over time.

Each business has:
- a price
- a quality level
- limited capacity
- some level of customer loyalty
- resistance to changing prices too quickly

Customers choose between businesses based on price, quality, and other factors. As demand shifts, each business can decide whether to change its price the next day based on a chosen strategy.

Prices evolve **endogenously**, meaning businesses react to each other rather than staying fixed.

---

## What You Can See From the Results

Each simulation run shows:
- how prices change day by day
- how market shares move between competitors
- which businesses gain or lose profit
- whether the market stabilizes or becomes unstable

This makes it possible to test ideas like:
- “What happens if one business cuts prices by 10%?”
- “Is it better to compete on price or quality?”
- “Who actually has market power in this market?”

---

## How the Model Works (High Level)

- Customer demand is split using a probabilistic choice model
- Prices affect demand through elasticity and substitution effects
- Businesses update prices using simple behavioral rules
- Random shocks can be added to reflect real-world noise
- Simulations run over many days to show longer-term effects

The simulation logic is kept separate from the interface so it can be tested and reused.

---

## What This Project Is (and Isn’t)

This is:
- a learning and exploration tool
- a way to visualize competitive dynamics
- a simplified model of real markets

This is not:
- financial advice
- a real pricing recommendation engine
- a complete representation of any specific market

All results depend on assumptions, which are meant to be questioned.

---

## Current Status

The core simulation engine is under active development.  
Planned improvements include:
- better strategy comparisons
- clearer stability metrics
- more realistic elasticity calibration
- counterfactual “what if” comparisons

---

## About Me

I’m **Sudhish**, a high school student interested in economics, finance, and business systems. I like building projects that help me understand how real-world decisions and incentives interact.

If you’re interested in the model, code, or results, feel free to reach out.
