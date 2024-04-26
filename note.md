---
class: middle

```{r, fig.cap="Figure: Measurement errors in PRISM total precipitation (1984-2020)", fig.dim=c(8, 7), out.width = '100%'}
knitr::include_graphics(here(base_dir, "images", paste0("plot_all_obs_me_tot_ppt_v2.png")))
```

---
class: middle

```{r, fig.cap="Figure: Measurement errors in PRISM EDD (1984-2020)", fig.dim=c(7, 6), out.width = '100%'}
knitr::include_graphics(here(base_dir, "images", paste0("plot_all_obs_me_edd_v2.png")))
```



---
class: middle

# Motivation: Measurement Error problems

Long history in the discussion of measurement error problems: 

For examples: 

.content-box-green[**Labor economics:**] 

+ `r Citet(bib, "duncan1985investigation")`: earning report of the Panel Study of Income Dynamics: 

+ `r Citet(bib, "bound1991extent")`: Measurement errors in income report of Current Population Survey

.content-box-green[**Development economics:**]

+ `r Citet(bib, "blattman2017reducing")` and <`r Citet(bib, "karlan2012list")`: Measurement errors in survey in development studies

<br>

<span style="color:blue">Measurement error problems is not much discussed in environmental economics.</span>


???

+ Measurement error issues have long history and the research is still actively going on, like the study in the APEC seminar last Friday (Professor Daniel Millimet). 

+ The understanding of the measurement error issues has been mainly developed in the field of labor and development economics, and people proposed many ideas how to overcome the problems. 
+ These study mostly talk about measurement errors in linear regression case. 

+ Even if the presence of measurement errors, if we still have the treatment estimate is still statistically significant and it is reasonable to assume the measurement error is random, then we can conclude that the treatment is effective. 

+ Meanwhile the measurement error issues are much less discussed in econometric analysis of environmental literature.

+ **One feature of the econometric analysis in environmental economics is that, sometimes we want to know more than whether the impact is significant or not.** For example, in climate change literature, it is obvious that climate change affects our economy, given that, we want to know what is the damage function is, say what is degree of the curvature of damage function of temperature, by estimating the coefficient of nonlinear term like quadratic term. 

+ To do so, more precise coefficient estimate. Thus, the presence of measurement errors are more influential in such cases. 


+ Current Population Survey data, It turned out that the measurement errors in CPS the results indicate that errors are serially correlated over 2 years and negatively correlated with true earning

+ Likewise, the measurement error in the earnings report in the Panel Study of Income Dynamics (PSDI) is correlated with the level of job tenure

+ The amounts of these measurement errors differ for the various measures in question and the length of the recall periods. 
  + The ratio of error-to-true variance for 1-year recall earnings and unemployment hours, for instance, is only half as large as the corresponding ratios if the recall period is 2 years

+ If you believe that measurement errors is classical, then the error attenuates the OLS estimates.
+ Like in the reduced form with linear functional form, if you see the positive statistically significant estimate with , 


for example, you can do:
+ See Duncan and Hill (1985), what did they do to investigate measurement error problems, 
+ Some Implications for Model Estimation
+ Amounts of Error Variance

+ One thing that should be noted is that these seminal studies 
+ Lots of people think that the measurement error problems are just a data problem. Yes, that's is absolutely true. 



# Measurement Errors 

Considering the correlation between measurement errors and observed weather outcome, I assume that measurement errors is a function of weather outcomes. 

$$u_{i,}$$

+ For each state and year, create a bins of measurement errors weather outcomes. 



+ Randomly sample from 

For example, 

+ For measurement errors in precipitation for firm $j$ in 

For each iteration, I randomly sampled observed measurement errors and use it 

$u^{w}_{}$: measurement error for weather variable $w$ in firm $i$ in state $j$ in year $t$, 



+ $\mathbf{ME}^{w}_{t,j}$ is the set of observed measurement errors in weather variable $w$ at stations in state $j$ in year $t$. 
  + For example, 

+ Then for each field $i$ located in the same state $j$, 


I take a random sample of measurement errors 


 field For measurement errors in weather variable $w$ of farm-field $i$ in state $j$

+ 