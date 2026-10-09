# tennis-ball-rig
A personal engineering project building a rig to measure and restore the internal pressure of 'dead' tennis balls, prolonging their lifetime and reducing waste.


## 1. Problem

- Tennis balls lose internal pressure over time due to air diffusing through the rubber shell.
- This happens at a slow rate under ambient conditions but is greatly accelerated when the balls are being repeatedly hit and bounced during play.
- The internal pressure of a tennis ball has a huge impact on how it plays - a 'fresh' ball will be noticeably faster and bouncier than a 'dead' one.
- In professional tournaments, new balls are introduced every 9 games (every 45 minutes roughly) to keep the conditions consistently 'fresh' for the players.
- Replacing balls so frequently is wasteful and very expensive for recreational players such as myself.


## 2. Aims

- Build a repeatable way to quantitatively test the internal pressure of tennis balls in order to gauge their 'freshness' against a benchmark.
- Track the internal pressure of a given ball through time with periodic testing.
- Build a pressurised storage vessel that can increase the internal pressure of 'dead' tennis balls back towards 'freshness'.
- Develop a data model that can predict the required storage pressure and duration for a ball to return to its original condition, based on its current pressure deficit.


## Part A: Pressure testing rig



### A.1 Design decisions

Table below gives an overview of and justification for each decision taken during the design process so far.

|ID| Date | Subject | Options considered | Decision and why |
|---|------|----------|---------------------|---------------|
|DA1| 24/09 | Measurement method | Force-deformation test / Shell buckling test | Force-deformation test chosen for continuous data output whereas buckling shows only one threshold |
|DA2| 24/09 | Test procedure | Custom force target(s) / Use ITF TB 03/01 values (forward and return deformation at 95.64N total load) | ITF TB 03/01 chosen because it is regulation approved, provides credible reference data and already has a known compliance band for test results |