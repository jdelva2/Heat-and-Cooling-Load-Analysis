# Heat-and-Cooling-Load-Analysis

## Purpose
This Project served as a Final Group Project contributed by Dione David, Jeff Wittenburg, and Jose Luis Del Valle Jr. The purpose for choosing this dataset was to work on Data Analysis and building a linear Model that would serve for the prediction of Heating and Cooling Loads within city buildings. Given certain features, we preformed data-processing,hypothesis test, normality tests, Bivariate correlations and predictive modeling.

## Shapiro Wilk Test for Normality
```Markdown
Heating_Load Cooling_Load
[1,]       18.675      17.5125
Normality test for  Relative_Compactness
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.93341, p-value < 2.2e-16

Normality test for  Surface_Area
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.94967, p-value = 1.628e-15

Normality test for  Wall_Area
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.9269, p-value < 2.2e-16

Normality test for  Roof_Area
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.74595, p-value < 2.2e-16

Normality test for  Overall_Height
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.63658, p-value < 2.2e-16

Normality test for  Glazing_Area
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.84349, p-value < 2.2e-16

Normality test for  Glazing_Area_Distribution
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.91551, p-value < 2.2e-16

Normality test for  Heating_Load
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.9121, p-value < 2.2e-16

Normality test for  Cooling_Load
	Shapiro-Wilk normality test

data:  my_data[, ix]
W = 0.90904, p-value < 2.2e-16

Normality test for log converted Relative_Compactness
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.94618, p-value = 4.31e-16

Normality test for log converted Surface_Area
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.94362, p-value < 2.2e-16

Normality test for log converted Wall_Area
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.94216, p-value < 2.2e-16

Normality test for log converted Roof_Area
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.76583, p-value < 2.2e-16

Normality test for log converted Overall_Height
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.63658, p-value < 2.2e-16

Normality test for log converted Glazing_Area
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = NaN, p-value = NA

Normality test for log converted Glazing_Area_Distribution
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = NaN, p-value = NA

Normality test for log converted Heating_Load
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.9328, p-value < 2.2e-16

Normality test for log converted Cooling_Load
	Shapiro-Wilk normality test

data:  log(my_data[, ix])
W = 0.9191, p-value < 2.2e-16

Normality test for Revised variables Relative_Compactness
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.88914, p-value = 4.807e-16

Normality test for Revised variables Surface_Area
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.89131, p-value = 7.036e-16

Normality test for Revised variables Wall_Area
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.92068, p-value = 2.301e-13

Normality test for Revised variables Roof_Area
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.75014, p-value < 2.2e-16

Normality test for Revised variables Overall_Height
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.63652, p-value < 2.2e-16

Normality test for Revised variables Glazing_Area
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.82739, p-value < 2.2e-16

Normality test for Revised variables Glazing_Area_Distribution
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.91705, p-value = 1.046e-13

Normality test for Revised variables Heating_Load
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.89673, p-value = 1.873e-15

Normality test for Revised variables Cooling_Load
	Shapiro-Wilk normality test

data:  (revised.cool_load.dat[, ix])
W = 0.88614, p-value = 2.859e-16

Normality test for Revised variables Relative_Compactness
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.89144, p-value = 7.209e-16

Normality test for Revised variables Surface_Area
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.88888, p-value = 4.593e-16

Normality test for Revised variables Wall_Area
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.93094, p-value = 2.464e-12

Normality test for Revised variables Roof_Area
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.75036, p-value < 2.2e-16

Normality test for Revised variables Overall_Height
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.63652, p-value < 2.2e-16

Normality test for Revised variables Glazing_Area
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.83164, p-value < 2.2e-16

Normality test for Revised variables Glazing_Area_Distribution
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.91699, p-value = 1.032e-13

Normality test for Revised variables Heating_Load
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.86468, p-value < 2.2e-16

Normality test for Revised variables Cooling_Load
	Shapiro-Wilk normality test

data:  (revised.heat_load.dat[, ix])
W = 0.92496, p-value = 6.018e-13
```
## Bi Variate Correlation for each feature.
```Markdown
The correlation of Relative compactness with Surface_Area is -0.991901461613886  
The correlation of Relative compactness with Wall_Area is -0.203781680321038  
The correlation of Relative compactness with Roof_Area is -0.868823407704476  
The correlation of Relative compactness with Overall_Height is 0.827747316838428  
The correlation of Relative compactness with Glazing_Area is 7.61739963332367e-20  
The correlation of Relative compactness with Glazing_Area_Distribution is 0  
The correlation of Relative compactness with Heating_Load is 0.62227193567777  
The correlation of Relative compactness with Cooling_Load is 0.634339066335359  
The correlation of Surface Area with Wall_Area is 0.19550163278939  
The correlation of Surface Area with Roof_Area is 0.880719516684842  
The correlation of Surface Area with Overall_Height is -0.858147673029019  
The correlation of Surface Area with Glazing_Area is 4.66413950990947e-20  
The correlation of Surface Area with Glazing_Area_Distribution is 0  
The correlation of Surface Area with Heating_Load is -0.65811991706542  
The correlation of Surface Area with Cooling_Load is -0.672998933354486  
The correlation of Wall Area with Roof_Area is -0.292316466194891  
The correlation of Wall Area with Overall_Height is 0.280975743474508  
The correlation of Wall Area with Glazing_Area is 0  
The correlation of Wall Area with Glazing_Area_Distribution is 0  
The correlation of Wall Area with Heating_Load is 0.455671365375227  
The correlation of Wall Area with Cooling_Load is 0.427116997667133  
The correlation of Roof Area with Overall_Height is -0.972512237018586  
The correlation of Roof Area with Glazing_Area is -1.19718678029136e-19  
The correlation of Roof Area with Glazing_Area_Distribution is 0  
The correlation of Roof Area with Heating_Load is -0.861828051579043  
The correlation of Roof Area with Cooling_Load is -0.862546603524974  
The correlation of Overall Height with Glazing_Area is 0  
The correlation of Overall Height with Glazing_Area_Distribution is 0  
The correlation of Overall Height with Heating_Load is 0.889430464435639  
The correlation of Overall Height with Cooling_Load is 0.89578516889245  
The correlation of Glazing Area with Glazing_Area_Distribution is 0.21296422075719  
The correlation of Glazing Area with Heating_Load is 0.269841685302837  
The correlation of Glazing Area with Cooling_Load is 0.207504991160362  
The correlation of Glazing Area Distribution with Heating_Load is 0.08736845962962  
The correlation of Glazing Area Distribution with Cooling_Load is 0.0505251188056757  
The correlation of Heating Load with Cooling_Load is 0.975861739143769  
```

```Markdown
Coefficients:
                               Estimate Std. Error t value Pr(>|t|)    
(Intercept)                    0.367598   2.921165   0.126 0.899892    
my_data$Relative_Compactness -19.996672   3.369180  -5.935 4.45e-09 ***
my_data$Wall_Area              0.018562   0.004776   3.887 0.000111 ***
my_data$Overall_Height         5.736372   0.207608  27.631  < 2e-16 ***
my_data$Glazing_Area          14.817971   0.879566  16.847  < 2e-16 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 3.245 on 763 degrees of freedom
Multiple R-squared:  0.8842,	Adjusted R-squared:  0.8836 
F-statistic:  1457 on 4 and 763 DF,  p-value: < 2.2e-16

Analysis of Variance Table

Response: my_data$Cooling_Load
                              Df  Sum Sq Mean Sq F value    Pr(>F)    
my_data$Relative_Compactness   1 27931.9 27931.9 2652.32 < 2.2e-16 ***
my_data$Wall_Area              1 22419.6 22419.6 2128.88 < 2.2e-16 ***
my_data$Overall_Height         1  8040.1  8040.1  763.46 < 2.2e-16 ***
my_data$Glazing_Area           1  2988.9  2988.9  283.82 < 2.2e-16 ***
Residuals                    763  8035.3    10.5                      
---
```
## Conclusion
  Our results point to our models being reliable for predicting cooling-load and heating-load. We suspect however that drawbacks to our data-set may have been incurred by poor data collection efforts. We suspect this poor data collection effort led to a lack of variation in some of the predictor variables. For example, there are only 2 unique building heights across 768 observations. 
  This being said, our initial hypothesis was correct. Our initial hypothesis is validated by our R-squared values; the model for cooling-load has an R-sq of 0.884 2 and the model for heating-load has an R-sq of .9133. 
  Also, it is worth noting that the predicition error for each model was best for the full models. However, prediction error had a minor change from the full model to the final-reduced model for each outcome. Prediction error changes from full to reduced models for heat and cooling load are 2.1699-2.0673 and 2.293-2.247 respectively with the reduced model prediction error being represented by the first variable in each comparison.
