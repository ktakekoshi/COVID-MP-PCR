# COVID-19:  Massively Parallel Clinical Testing Platform for Pandemic Polymerase Chain Reaction (PCR) Testing

The COVID-19 epidemic has exposed the need for a high-throughput clinical polymerase chain reaction (PCR) platform for epidemic / pandemic testing. 

It is proposed that current automated PCR clinical testing systems are designed for high flexibility in range of tests to be performed simultaneously (e.g. large test menu), while sacrificing on cost and throughput. Such automated systems may be well-suited for clinical testing where a large and diverse menu of tests must be accessed on demand basis, but are not  designed for repeated / parallel execution of the same test over a very large number of specimens.  Nor are such highly engineered, high costs clinical automated systems suited for intermittent use as in a pendemic setting.

A very high throughput design such as the one herein proposed, is likely not economically viable in the ordinary labratory test setting, as there is usually not demand for extemely high throughput testing of a single test.

This repository is directed towards open-source "maker space" -like development such a high-throughput single-test clinical testing platform.  

## Objectives include:

- Moderated cost suitable for intermittent use during epidemics / pandemics.
- Use of readily available off-the-shelf components.
- Capable of processing large numbers of specimens in a short amount of time.
- Open source development of hardware and software.

## The provisional proposal envisions:

-  A large, thin disposable sheet of [vacuum thermoformed](https://youtu.be/DWWq2hH7imA?t=84) plastic sheet having an array of 900 - 10,000 wells, with each well serving as an individual PCR reaction chamber.
-  A vacuum form mold to create the impression of the well array in the thermoformed sheet.
- A bar code reader and X-Y robotic transfer / dispensing system to aliquot patient specimens into recorded wells.
- At least three water baths at different temperatures – denaturation, annealing, and extension – with additional water baths if needed (e.g. reverse transcription, final elongation).
- A device to read the results.

## The provisional procedure envisions the following process:

- The vacuum form mold is used to create a single vacuum thermoformed disposable plastic sheet with array of wells.
- The sheet is cleaned using hydrolyzing reagents to remove residuals of nucleic acids.
- The sheet is placed on a loader.
- Wells in the sheet are loaded with reagents.
- The loader is equipped with X-Y robotic transfer / dispensing system that transfers patient specimens to wells and records the locations of each patient specimen.
- The sheet if necessary is manually transferred to a water bath set a temperature appropriate for reverse transcription.
-  The sheet is manually transferred by laboratory technicians between the three or more water baths at different temperatures – denaturation, annealing, and extension – to accomplish the PCR amplification, according to protocol appropriate to the testing reagents.
- The sheet is placed on a reader device at the end and/or during the procedure.
- Results are reported, or confirmed using an alternative method for additional specificity if necessary.
