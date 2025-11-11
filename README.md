# eStarlight_JPsi_dataset
Dataset for study of JPsi with Estarlight, relating on studies of TCS with the ePIC detector.


Input cards are provided for J/psi production at similar kinematics of the existing TCS files, for the study of background physics as well muonID with the ePIC detector.


The eStarlight generator is used to generate J/psi MC events. \
Author: Samuel Heppelman, et. al. \
Link (src, installation and usage): https://github.com/eic/estarlight 


Files are output from the generators in hepmc ascii format. These must be afterburned (available in eic-shell), and then converted to hepmc root format (availabe in eic software stack):\
abconv -p 0 eslight_jpsi_18x275.hepmc ab_eslight_jpsi_18x275.hepmc\
hepmc3ascii2root ab_eslight_jpsi_18x275.hepmc ab_eslight_jpsi_18x275.root\


These afterburned hepmc3 (ee and mumu) root files are currently available at\
/gpfs/mnt/gpfs02/eic/gpenman/ \
under straightforwardly named directories: \
JPsi_18x275/  JPsi_muon_18x275/ 
