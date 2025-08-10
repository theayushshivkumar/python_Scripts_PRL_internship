Some useful Python scripts I wrote at PRL for my project on studying jets and outflows from young massive stars using science-ready ALMA data cubes.

1) astrodendro.ipynb
   -
   - The script utilizes a Python package called astrodendro.
   - The algorithm uses the method of dendrogram trees based on peak flux, scans through the entire spatial extent of the file, and identifies the compact sources along with their flux, centers, ra, and dec.

   
2) SpectralCube.ipynb
   -
   - Extract spectra from the FITS cube file. Make spectral slabs to study the region for particular spectral line transitions. Write these slabs to separate FITS cube files for further analysis.
   - Generate Moment 0, 1, and 2 maps for various ALMA data cubes. Write these to separate FITS files.
   - Includes visualisation of FITS cube files and unit transformation scripts of the spectral axis of the FITS cube.
   - Many more. A bit unorganized.

3) CoreMassSize.ipynb
   -
   - The compact sources identified by the astrodendro algorithm is saved to a table along with all its relavant info such as flux, ra, and dec.
   - Relavant equations are then used in this script to compute the properties of these compact objects, such as radius, mass, surface and number density.

4) OutflowParameters.ipynb
   -
   - Script to compute the parameters of the jets traced by the SiO v = 0 (J = 8-7) rotational transition.
   - Computes the jet column density, mass of the jet, jet velocity, jet momentum, jet energy, dynamical timescale of the jet, and finally the rate of outflow of mass.
  
5) CoreMasking.ipynb
   -
   - Python script to create a polygon mask around the compact sources identified by the astrodendro algorithm.
