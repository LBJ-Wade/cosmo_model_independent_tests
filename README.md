# Model independent tests of Cosmology
Repository of the codes and data files to perform model-independent tests of Cosmology using real H(z) measurements as well as Euclid and SKA simulations.

The python code 'model_ind_tests.py' carries out Gaussian Processes reconstructions with GaPP (https://github.com/astrobengaly/GaPP) in order to obtain model-independent cosmological measurements such as: 
  - Hubble Constant H0 
  - deceleration parameter q0
  - null tests of the LCDM model, namely the Om and Lm tests as in [https://arxiv.org/abs/0807.3548], [https://arxiv.org/abs/0807.4304] (see also [https://arxiv.org/abs/0712.3457])

Data files in this repository consist of: 
  - Real H(z) measurements from galaxy ages, aka Cosmic Chromoneters, and radial BAO mode SDSS redshift survey
  - Simulated radial BAO measurements from Euclid galaxy survey, and SKA band 1 and band 2 21cm Intensity Mapping. Fiducial Cosmology follows Planck 2018 (TT, TE, EE+lowE+lensing) best-fits 

The code receives the number of data points and name of the survey containing Hz measurements as inputs
  - For real data: nz1 refers to the number of CC data points, nz2 to the BAO ones. Put 0 in nz2 in case you just want the former 
  - For simulations: nz1 refers to the number of Euclid or SKA band 1 data points, nz2 to the SKA band 2. Put 0 in nz2 if you do not want to include band 2 simulations
  - survey refers to 'euclid', 'ska', or 'cc'

Examples of the reconstructions assuming SKA band1 + band 2 and observational CC + SDSS radial BAO are also provided in this repository. 

I hope this code is helpful for students and anyone interested in performing this analysis in the future. If you use it, slease refer to the following papers

Null tests of the concordance model in the era of Euclid and the SKA 
Carlos A. P. Bengaly, Chris Clarkson, Martin Kunz, Roy Maartens
https://arxiv.org/abs/2007.04879 
Phys. Dark. Univ. accepted

Evidence for cosmic acceleration with next-generation surveys: A model-independent approach
Carlos A. P. Bengaly
https://arxiv.org/abs/1912.05528
MNRAS, Volume 499, Issue 1, November 2020, Pages L6-L10; 10.1093/mnrasl/slaa040

The Hubble constant tension with next-generation galaxy surveys
Carlos A. P. Bengaly, Chris Clarkson, Roy Maartens
https://arxiv.org/abs/1908.04619
JCAP05(2020)053; 10.1088/1475-7516/2020/05/053

Please contact carlosbengaly@on.br or carlosap87@gmail.com for further enquiries. Reasonable suggestions are always welcome. 
