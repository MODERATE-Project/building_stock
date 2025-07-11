# ModerateBuildingStock
This is the repository to create synthetic time-series building operational data for the MODERATE Horizon EU project. 
The files in this repository are reqired to run time-series simulations using EnergyPlus models. The EnergyPlus models use IDF as inputs; these inputs have been determined using national/regional building stock cluster data (obtained from WP3). There are also two jupyter notebooks demonstrating the use of EnergyPlus within a Python Environment. 

Description of files are as follows:
1. BrusselsIWEC.epw and 3.epw: EnergyPlus weather files required for simulation in E+UseCase.ipynb and EnergyPlusParametricRuns.ipynb. 
2. E+UseCase.ipynb: Use this notebook to run your first E+ simulation (Dependencies: HPSFD.idf and BrusselsIWEC.epw). Make sure to set the path for your .idd file (E+ installation directory in your local computer).
3. EnergyPlusParametricRuns.ipynb: Use this notebook to change building parameters in your idf file and run N number of simulations (Dependencies: PVHPSFD and 3.epw). Again make sure to edit the path to your files.
4. HPSFD.idf and PVHPSFD.idf: EnergyPlus input files representing single family dwellings (SFD) with Heat Pumps (HPs) and with Solar PV and Heat Pumps.
5. Disaggregation_method.ipynb: these series of notebooks include different approaches in decomposing the aggregated energy consumption
