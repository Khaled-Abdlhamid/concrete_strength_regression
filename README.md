## [Concrete Compressive Strength Data Set](https://code.datasciencedojo.com/datasciencedojo/datasets/tree/master/Concrete%20Compressive%20Strength)
- Overview: This data set has 1030 rows and 9 columns. Concrete is the most important material in civil engineering. The concrete compressive strength is a highly nonlinear function of age and ingredients The actual concrete compressive strength (MPa) for a given mixture under a specific age (days) was determined from laboratory. Data is in raw form (not scaled). 

### Column Dictionary:
- Cement (component 1)(kg in a m3 mixture) : Cement   (component 1) -- Kilogram in a meter-cube mixture -- Input Variable.
- Blast Furnace Slag (component 2)(kg in a m3 mixture) : Blast Furnace   Slag (component 2) -- kg in a m3 mixture -- Input Variable
- Fly Ash (component 3)(kg in a m3 mixture) : Fly Ash   (component 3) -- kg in a m3 mixture -- Input Variable
- Water  (component 4)(kg in a m3   mixture) : Water   (component 4) -- kg in a m3 mixture -- Input Variable
- Superplasticizer (component 5)(kg in a m3 mixture) : Superplasticizer   (component 5) -- kg in a m3 mixture -- Input Variable
- Coarse Aggregate  (component 6)(kg   in a m3 mixture) : Coarse   Aggregate (component 6) -- kg in a m3 mixture -- Input Variable
- Fine Aggregate (component 7)(kg in a m3 mixture) : Fine Aggregate   (component 7) -- kg in a m3 mixture -- Input Variable
- Age (day) : Age -- Day   (1-365) -- Input Variable
- Concrete compressive strength(MPa, megapascals) : Concrete   compressive strength -- MegaPascals -- Output Variable

#### EDA:
- Changed the column names.
- Plotted some graphs to better understand the data.
- Log-transformed the skewed features.
- plotted a correlation heatmap to visualize the underlying relation between features.
- calculated Variance_inflation_factor to check highly correlated features to avoid multicollinearity.
- Created new feature (water per cement).
- Dropped the unnecassary columns.

#### Training:
- Trained **LinearRegression** and got an RMSE of 10.92 and R^2 of 0.57.
- Trained **AdaBoostRegressor** with GridSearch and got RMSE of 7.51 and R^2 of 0.79
- Trained **RandomForrestRegressor** with GridSearch and got RMSE of 7.85 and R^2 of .78