# NumExMLContest
ML tool to predict first 10 NumEX input parameter combinations with best NPVs.

## Getting Started

* *5_point_system.ipynb* - imports data from *Results(4000).csv* and fits **4 CatBoost models for each Well_type**. Models are then saved to */5_point_full_trained_catboosts* folder
* *5_point_system_executable* - allows to input validation data from *input_5_point.csv* and to compare **10 best predicted NPV combinations** and **10 best NumEx NPV combinations**
* *5_point_system_cycle* - iteratively splits data into train/test (90% to 10%) and then makes 4 final histograms of **best predicted NPV combinations**

## Dependencies
Conda main repo:
 * ***scikit-learn 0.19.0*** - data processing
 * ***numpy 1.14.2*** - data processing

Conda-forge repo:
 * ***catboost 0.12.1.1*** - used for regressions
 * ***tqdm 4.28.1*** - progressbar
 * ***matplotlib 3.0.1*** - plotting
 * ***pandas 0.23.4*** - data processing
