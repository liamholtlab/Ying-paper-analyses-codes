# Ying-paper-analyses-codes

These MATLAB codes are used in the paper of Xie et al. "Polysome collapse and RNA condensation fluidize the cytoplasm".

There are two folders for different sets of codes. One is "Vacuole volume analyses", which analyzes the vacuole volume using Z stacks of fluorescently labeled vacuole imaging files. The inputs include subfolders containing both individual tiff files of the Z stacks and a csv file containing center positions of vacuoles, which can be acquired using the multi-point selection tool and saved as ROI in FIJI software. This set of codes were modified from original codes developed by Mark Chan, who is an associate professor from San Francisco State University. The main call function is "Combine_Chan_edge_Tong_modified.m", which would save the vacuole information within an excel file.

The other one is "Velocity autocorrelation analyses", which analyzes the velocity autocorrelation of tracked particle trajectories. The main call function is "result_difusion_modi_Tong.m", which uses the output csv files of particles trajectories saved from FIJI plugin 'Mosaic'. The outputs of this main call function include "tracked_..." files. These files are the inputs for the function of "Velocity_correlation.m", which calculates the normalized velocity autorrelation for the trajectories. Additionally, "Raw_data_extraction_MD_simulation.m" and "Velocity_correlation_MD_simulation.m" are used to calculate normalized velocity autocorrelation using particle trajectory outputs from MD simulations.
