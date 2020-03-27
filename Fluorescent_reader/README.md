# Fluorescent Reader README

The project envisions a real-time PCR fluorescent reader system.

Wavelengths:

- Single channel or dual channel?  Single should suffice for now (needs to detect FAM).
![](https://www.thermofisher.com/us/en/home/technical-resources/technical-reference-library/real-time-digital-PCR-instruments-support-center/7500-real-time-pcr-systems-support/7500-real-time-pcr-systems-support-getting-started/jcr:content/MainParsys/accordion_2e43/itemspar/accordionitem_e431/itemParsys/image_dabc/foregroundimg.img.320.high.jpg/1548183793593.jpg)
- [6-FAM](https://www.sigmaaldrich.com/technical-documents/articles/biology/choosing-the-right-probe.html) Max. EX 495 nm, Max. EM 520 nm; Compatible Quenchers: HQ-1, TAMRA.
- https://support.chaibio.com/hc/en-us/articles/360004016834-Single-Channel-or-Dual-Channel-Open-qPCR-

[Photomultiplier tube](https://en.wikipedia.org/wiki/Photomultiplier_tube) vs. [silicon photomultiplier](https://en.wikipedia.org/wiki/Silicon_photomultiplier) vs. CCD vs. CMOS sensors:

- Must have enough sensitivity to detect liberated fluorophore.
- Must be capable to rapidly query large number of specimens (fast indiviudal query vs. massive parallel query).
- CCD may lack sensitivity (see U Penn open source project below).
- Photomultiplier (tube vs. silicon) may be required.

Can be adapted from other open source projects?

- Leverage design sourced from silicon photomultiplier used in [desktop muon detector](http://cosmicwatch.lns.mit.edu/about)?
    - Uses [ON Semiconductor SiPM MicroFC-60035-SMT](https://www.mouser.com/ProductDetail/on-semiconductor/microfc-60035-smt-tr1/?qs=byeeYqUIh0MxSRIaBcfS6g%3D%3D&countrycode=US&currencycode=USD) silicon photomultiplier chip.
    - https://arxiv.org/abs/1606.01196
    - https://github.com/spenceraxani/CosmicWatch-Desktop-Muon-Detector-v2
    
- Open source plate reader (U Penn):  
    - https://pubs.acs.org/doi/10.1021/acs.biochem.8b00952 
    - "In the baseline low-cost version here, we use a CCD-based Ocean Optics visible-range detector because of its available open-source drivers and overall balance of sensitivity, full-spectrum and monochromatic detection, and relatively low cost compared to those of monochromator-coupled photomultiplier tubes (PMTs)."
    - "The fluorescence of NIST-traceable fluorescein could be measured with an ∼10 nM limit of detection with the low-cost detector. Such a detection limit is sufficient for common fluorescence assays as intended, albeit greater than the ∼10 pM limit of commercial systems that use PMTs."
    - Total primer in CDC test kit is 22.5 nmol for 1000 tests at 20 μL each (22.5 pmol / 20 μL = 1.125 μM), so either CCD or photomultiplier may be sufficient.
    - How to get faster speed?
    - "The OSP acquires a full spectrum in ∼11 s per well (inclusive of the movement to the well). Because the CCD detector captures all wavelengths simultaneously, the acquisition time for a full spectrum is the same as that of a single wavelength measurement."  This seems slow for the number of specimens.
    
- Chai bio:  https://www.chaibio.com/openqpcr (hardware may not be open source)

Reference:

- http://www.gene-quantification.de/real-time-pcr-handbook-life-technologies-update-flr.pdf
