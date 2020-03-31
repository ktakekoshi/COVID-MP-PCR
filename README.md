# COVID-19:  Massively Parallel Clinical Testing Platform for Pandemic Polymerase Chain Reaction (PCR) Testing

The COVID-19 epidemic has exposed the need for a high-throughput clinical polymerase chain reaction (PCR) platform for epidemic / pandemic testing. 

It is proposed that current automated PCR clinical testing systems are designed for automated flexibility in types of tests to be performed simultaneously (e.g. large test menu), while sacrificing on cost and throughput. Such automated systems are well-suited for clinical testing where a large and diverse menu of tests must be accessed on-demand, but are not designed for repeated / parallel execution of the same test over a very large number of specimens.  Nor are such highly engineered, high-cost clinical automated systems economical for intermittent use in a pandemic setting.

A very high throughput design such as the one herein proposed, is likely not economically viable in the ordinary clinical setting, as under normal circumstances there is not sufficient demand for extremely high throughput of a single test. This repository is directed towards open-source "maker"-like development of a high-throughput single-test clinical testing platform.  

## Objectives include:

- Moderated cost suitable for intermittent use during epidemics / pandemics.
- Use of readily available off-the-shelf components.
- Dispensibles easily sourced and resistant to supply chain disruption.
- Can process large numbers of specimens simultaneously.
- Open source development of hardware and software.

## The provisional proposal envisions:

- A large, thin disposable [vacuum thermoformed](https://youtu.be/DWWq2hH7imA?t=84) plastic sheet having an array of 900 - 10,000 wells, with each well serving as an individual PCR reaction chamber.
- A vacuum thermoform mold to create the impression of the well array in the thermoformed sheet.
- A bar code reader and X-Y liquid handling robotic transfer / dispensing system to aliquot patient specimens into recorded wells.
- At least three water baths at different temperatures – denaturation, annealing, and extension – with additional water baths if needed (e.g. reverse transcription, final elongation).
- A fluorescent reader device to read the results.

## The provisional procedure envisions the following process:

- The vacuum form mold is used to create a single-piece [vacuum thermoformed](https://youtu.be/DWWq2hH7imA?t=84) disposable plastic sheet with array of wells.
- The sheet is cleansed using hydrolyzing reagents to remove nucleic acid residuals / contaminants.
- The sheet is placed on a loader.
- Reaction wells in the sheet are loaded with reagents (primers, polymerases, nucleotide mixes, fluorescent reagents).
- The loader is equipped with bar code reader and X-Y liquid handling robotic transfer / dispensing system that transfers patient specimens to wells and records the locations of each patient specimen.
- The sheet if necessary is manually transferred by laboratory technicians to a water bath set at a temperature appropriate for reverse transcription.
- The sheet is manually transferred by laboratory technicians between the three or more water baths at different temperatures – denaturation, annealing, and extension – to accomplish the PCR amplification, according to protocol appropriate to the testing reagents.
- An alternative automated water-based thermocycling system will also be proposed. In this implementation, there will be a specimen water bath, and three or more resevoirs of water held at different temperatures. To thermocycle, water from each of the resevoirs is drawn or pumped rapidly into the specimen resevoir for the appropriate period of time for the cycle, then disposed of or drawn back into the resevoir from which it originated. In one implementation of this principle, the specimen water bath drains rapidly by gravity into a temporary toilet. The specimen water bath is then filled from the appropriate temperature water bath, either by gravity or by pump. Simultaneously, water from the toilet is pumped back into the water bath from which it originated. This helps to keep the water baths at constant temperature. It is proposed that the system of pumps and/or valves will be easier to cheaply construct using off-the-shelf components, and implement on temperary or expedient basis than alternative heat pump-based systems.
- The sheet is placed on a reader device at various points during the procedure and / or at the end of the procedure.
- Using this massively parallel batch-based testing system, it is proposed that anywhere from 300 - 10,000 or more test results could be obtained in a single run.
- Depending on performance characteristics, follow-up testing of positive results using standardized testing may be performed for confirmation.

## Possible hurdles to implementation:

- Production of RNA using RNA extraction kits from patient specimens is time consuming, and is often performed using proprietary reagents (e.g. Qiagen, Roche MagNA, bioMérieux, Abbott mSample). Shortages of RNA isolation kits have occurred during the current pandemic. Methods of RNA isolation more resistant to supply chain discruption should be investigated.

- Loading of specimens in massively parallel format may require an excess of time. RNA is particularly susceptible to hydrolysis / disruption. If necessary, one possible solution is to perform reverse transcription as soon as loading occurs or prior to loading specimen, as DNA is more resistant to hydrolysis than RNA. Alternatively, specimens may be frozen, or the vaccum-formed well array may be loaded while on a cold surface, so specimens freeze as they are loaded into their respective wells.

- During large-scale pandemic, laboratories in the U.S.A. implementing laboratory-developed tests that utilize the open source platform will require [Emergency Use Authorization (EUA)](https://www.fda.gov/emergency-preparedness-and-response/mcm-legal-regulatory-and-policy-framework/emergency-use-authorization) from the FDA. Regulations in other jurisdictions will vary.

## Comparisons with established platforms:

Current proprietery platforms are capable of running ~100 tests per batch, with each batch requiring 2 - 8 hours to complete. The current proposal is to expand batch processing to many hundreds or thousands of tests per batch.

- [Abbott m2000sp / m2000rt](https://www.molecular.abbott/us/en/products/instrumentation/m2000-realtime-system) -  96 well microtiter format, performs “[many hundreds](https://www.youtube.com/watch?v=IAU1BC21RsY) of specimens per day.”
- [Applied Biosystems 7500](https://www.thermofisher.com/us/en/home/life-science/pcr/real-time-pcr/real-time-pcr-instruments/7500-fast-real-time-pcr-system.html)  - 96 well microtiter format.
- [Roche 6800-8800](https://diagnostics.roche.com/us/en/products/systems/cobas-8800-system.html) - 96 well microtiter format.

High throughput platforms currently in development will likely be proprietary and expensive:
- [Hologic](https://www.hhs.gov/about/news/2020/03/09/hhs-supports-development-of-first-high-throughput-covid-19-diagnostic-test.html) - Development with assistance from HHS Office of the Assistant Secretary for Preparedness and Response (ASPR) / Biomedical Advanced Research and Development Authority [(BARDA)](https://www.phe.gov/about/barda/Pages/default.aspx).

## Additional information:

"WHO COVID-19 test kit:"

- One test (Charité Virology, Berlin, Germany) uses [Fluorescein amidite (FAM)](https://en.wikipedia.org/wiki/Fluorescein_amidite) reporter with BBQ quencher (FAM-CAGGTGGAACCTCATCAGGAGATGC- BBQ; FAM-ACACTAGCCATCCTTACTGCGCTTCG- BBQ).
- 45 cycles.
- https://www.who.int/emergencies/diseases/novel-coronavirus-2019/technical-guidance/laboratory-guidance
- https://www.who.int/docs/default-source/coronaviruse/protocol-v2-1.pdf?sfvrsn=a9ef618c_2

CDC COVID-19 test kit:

- During the extension phase of the PCR cycle, the 5’ nuclease activity of Taq polymerase degrades the probe, causing the reporter dye to separate from the quencher dye, generating a fluorescent signal.
- Apparently uses [Fluorescein amidite (FAM)](https://en.wikipedia.org/wiki/Fluorescein_amidite) reporter.
- [May use](https://www.cdc.gov/coronavirus/2019-ncov/lab/rt-pcr-panel-primer-probes.html) BHQ1 quencher.
- Uses Applied Biosystems 7500 Fast Dx Real-Time PCR Instrument; "Reporter set to FAM and the Quencher is set to (none)," "Reps should be set to 45."
- https://www.cdc.gov/coronavirus/2019-ncov/lab/tool-virus-requests.html
- https://www.fda.gov/media/134922/download
