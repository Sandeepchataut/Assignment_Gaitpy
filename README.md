# Analaysis of bout counts with respect to strides in gait analysis

## What is Gaitpy?
GaitPy is a Python package that provides tools for analyzing and modeling human gait data. It reads and processes raw vertical accelerometry data and extract clinical gait characteristics. It is primarily used in biomechanics research to analyze and understand the movement patterns of human subjects during walking. The GaitPy package offers various features to analyze and process gait data, such as calculating gait events, computing gait parameters, and performing statistical analysis. It also provides functions for visualizing and plotting gait data, which can aid in understanding and interpreting the results of the analysis.
Some of the specific functionalities of GaitPy include:
* Extraction of gait events such as heel strike and toe-off
* Calculation of temporal and spatial gait parameters, such as gait speed, step length, and cadence
* Visualization of gait data using plots such as gait cycles, time series, and histograms
* Statistical analysis of gait data, including computing means, standard deviations, and confidence intervals

* **The following steps were performed for the analysis of bout counts with respect to strides:**
* 1. A new virtual environment was created for the gaitpy.
* 2. Using the IMU-data-10-17-2022 data, preprocessing was done to extract just the vertical acceleration. 
* 3. The timestamp data was converted to Unix-timestamp and only vertical acceleration and unix timestamp were saved as final.csv file.
* 4. The csv file was executed through gaitpy pipeline.
* 5. Following this, the gait bouts were classified and gate features were extracted.
* 6. The gait features were saved as final_gait.csv file.
* 7. The data were grouped together with respect to column 'bout_number' .
* 8. Mean (average) of each data was calculated based on the column 'bout_number'.
* 9. After that, the stride data was extracted dividing each steps by 2.
* 10. The stride data was saved as final_stride.csv.
* 11. Following this, data bins were created and the counts were made.
* 12. The following results were obtained as bouts vs strides: 
* ![Bout_vs_strides](https://user-images.githubusercontent.com/130417028/231067288-a680342a-0e08-43e9-b086-3d6943febf8e.png)

  
