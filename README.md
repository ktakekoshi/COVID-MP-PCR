# COVID-19:  Massively Parallel Clinical Testing Platform for Pandemic Polymerase Chain Reaction (PCR) Testing

The COVID-19 epidemic has exposed the need for a high-throughput clinical polymerase chain reaction (PCR) platform for epidemic / pandemic testing. 

It is proposed that current automated PCR clinical testing systems are designed for high flexibility in range of tests to be performed simultaneously (e.g. large test menu), while sacrificing on cost and throughput. Such automated systems may be well-suited for clinical testing where a large and diverse menu of tests must be accessed on demand basis, but are not  designed for repeated / parallel execution of the same test over a very large number of specimens.  Nor are such highly engineered, high-cost clinical automated systems suited for intermittent use as in a pandemic setting.

A very high throughput design such as the one herein proposed, is likely not economically viable in the ordinary setting, as under normal circumstances there is not sufficient demand for extremely high throughput of a single test. This repository is directed towards open-source "maker"-like development of a high-throughput single-test clinical testing platform.  

## Objectives include:

- Moderated cost suitable for intermittent use during epidemics / pandemics.
- Use of readily available off-the-shelf components.
- Dispensibles easily sourced and resistant to supply chain disruptions.
- Can process large numbers of specimens simultaneously.
- Open source development of hardware and software.

## The provisional proposal envisions:

- A large, thin disposable [vacuum thermoformed](https://youtu.be/DWWq2hH7imA?t=84) plastic sheet having an array of 900 - 10,000 wells, with each well serving as an individual PCR reaction chamber.
- A vacuum thermoform mold to create the impression of the well array in the thermoformed sheet.
- A bar code reader and X-Y robotic transfer / dispensing system to aliquot patient specimens into recorded wells.
- At least three water baths at different temperatures – denaturation, annealing, and extension – with additional water baths if needed (e.g. reverse transcription, final elongation).
- A fluorescent reader device to read the results.

## The provisional procedure envisions the following process:

- The vacuum form mold is used to create a single-piece vacuum thermoformed disposable plastic sheet with array of wells.
- The sheet is cleansed using hydrolyzing reagents to remove nucleic acids residuals / contaminants.
- The sheet is placed on a loader.
- Reaction in the sheet are loaded with reagents (primers, polymerases, nucleotide mixes, fluorescent reagents).
- The loader is equipped with an X-Y robotic transfer / dispensing system that transfers patient specimens to wells and records the locations of each patient specimen.
- The sheet if necessary is manually transferred by laboratory technicians to a water bath set at a temperature appropriate for reverse transcription.
- The sheet is manually transferred by laboratory technicians between the three or more water baths at different temperatures – denaturation, annealing, and extension – to accomplish the PCR amplification, according to protocol appropriate to the testing reagents.
- The sheet is placed on a reader device at the end and/or at various points during the procedure.
- Using this massively parallel batch-based testing system, it is proposed that anywhere from 300 - 10,000 or more test results could be obtained in a single run.
- Depending on performance characteristics, follow-up testing of positive results using standardized testing may be performed for confirmation.

## Possible hurdles to implementation:

Production of RNA using RNA extraction kits from patient specimens is time consuming, and is often performed using proprietary reagents (e.g. Qiagen, Roche MagNA). Shortages of RNA isolation kits have occurred during the current pandemic. Methods more resistant to supply chain discruptino should eb investigated.

## Comparisons with established platforms:

Current proprietery platforms are capable of runnign ~100 tests per batch, with each batch requiring many hourse to complete. The current proposal is to expand batch processing to many hundreds or thousands of tests per batch.

- Abbott m2000sp / m2000rt -  96 well microtiter format, performs “many hundreds of specimens per day.”
- Applied Biosystems 7500  - 96 well microtiter format.
- Roche 6800-8800 - 96 well microtiter format.

