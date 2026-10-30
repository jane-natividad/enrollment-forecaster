# Enrollment Forecaster

Simulates site start up and recruitment 2,000 times and shows the odds of hitting target by your deadline.

**[Try the live demo](https://enrollment-forecaster.vercel.app)**. It works straight away with no setup, runs entirely in your browser, and stores nothing. All data is fictional or synthetic.

## Why I built it

Every enrollment plan I've seen starts as a straight line on a slide. Then sites open late, a few never recruit, and the date slips. I wanted the plan to come with honest odds from day one, and a quick way to test which fix is worth paying for.

## The problem

Enrollment plans assume every site opens on time and recruits at the average rate. In reality some sites open late, some never recruit and performance varies widely, so the planned date often has far worse odds than anyone realises.

## What I built

A Monte Carlo forecaster using the standard Poisson Gamma recruitment model. Set sites, activation timing, recruitment rate, site variability, non performing sites and screen failure, then see the odds of finishing on time, a range of outcomes, a rescue scenario side by side and which lever matters most.

## Who it's for

Clinical operations, study start up and R&D program leaders who need to know how likely an enrollment plan really is.

## What it does

- Set the plan: target, deadline, sites, activation window, recruitment rate, site variability, non performers and screen failure
- See the odds of finishing on time, likely finish months and a chart of 2,000 simulated trials
- Compare a rescue scenario such as adding sites or opening them sooner
- See which lever moves the odds the most

## Decisions that shaped it

1. **Odds first:** the chance of finishing on time leads the page.
2. **A recognised model:** Poisson Gamma recruitment captures how unevenly sites perform.
3. **Fair comparisons:** every scenario uses the same random draws, so differences come from the change itself.

## Key takeaway

The headline is a probability. A plan that 'finishes in month 15' may only have even odds.

## Built with

- HTML, CSS and JavaScript in a single file
- A seeded random number generator, so every run is reproducible

## Run it locally

Open `index.html` in any browser. There's nothing to install.

## About this project

This is a working prototype I built to explore a real problem space. It uses illustrative, fictional data and isn't connected to any organisation's systems. You can find more of my work at [jane-natividad.github.io](https://jane-natividad.github.io).

Built by [Jane Natividad](https://github.com/jane-natividad).
