# Fluorescent Reader README

The project envisions a real-time PCR fluorescent reader system.

Wavelengths:

- Single channel or dual channel?  Single should suffice for now (needs to detect FAM).
![](https://www.thermofisher.com/us/en/home/technical-resources/technical-reference-library/real-time-digital-PCR-instruments-support-center/7500-real-time-pcr-systems-support/7500-real-time-pcr-systems-support-getting-started/jcr:content/MainParsys/accordion_2e43/itemspar/accordionitem_e431/itemParsys/image_dabc/foregroundimg.img.320.high.jpg/1548183793593.jpg)
- https://support.chaibio.com/hc/en-us/articles/360004016834-Single-Channel-or-Dual-Channel-Open-qPCR-

Can be adapted from other open source projects?

- Open source plate reader (U Penn):  
    - https://pubs.acs.org/doi/10.1021/acs.biochem.8b00952 
    - "In the baseline low-cost version here, we use a CCD-based Ocean Optics visible-range detector because of its available open-source drivers and overall balance of sensitivity, full-spectrum and monochromatic detection, and relatively low cost compared to those of monochromator-coupled photomultiplier tubes (PMTs)."
    - "The fluorescence of NIST-traceable fluorescein could be measured with an ∼10 nM limit of detection with the low-cost detector. Such a detection limit is sufficient for common fluorescence assays as intended, albeit greater than the ∼10 pM limit of commercial systems that use PMTs."
    - Total primer in CDC test kit is 22.5 nmol, so may nee photomultiplier (PMT) for accurate detection.
    - How to get faster speed?
    - "The OSP acquires a full spectrum in ∼11 s per well (inclusive of the movement to the well). Because the CCD detector captures all wavelengths simultaneously, the acquisition time for a full spectrum is the same as that of a single wavelength measurement."  This seems slow for the number of specimens.
    
- Chai bio:  https://www.chaibio.com/openqpcr (hardware may not be open source)

