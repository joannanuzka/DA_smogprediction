
## Checklist for project Grading

When grading each of criterions you have to **write** justification why the points were given. 

1. Problem formulation [5/5 pts]:
  - is the problem clearly stated [1/1 pt]
    - Yes the problem is clearly stated. 
  - what is the point of creating model, are potential use cases defined [1/1 pt]
    - analyzing air quality and it's impact on health
  - where do data comes from, what does it containt [1/1 pt]
    - visualcrossing.com and powietrze.gios.gov.pl 
  - DAG has been drawn [1/1 pt]
    - Yes, it is drawn.
  - confoundings (pipe, fork, collider) were described [1/1 pt]
    - Yes. 
2. Data preprocessing [2/2 pts]:
  - is preprocessing step clearly described [1/1 pt]
    - Yes. 
  - reasoning and types of actions taken on the dataset have been described [1/1 pt]
    - Yes. 
3. Model [4/4 pts]
  - are two different models specified [1/1 pt] 
    - normal distribution and student’s t-distribution.  
  - are difference between two models explained [1/1 pt]
    - Yes. Student’s t-distribution has lower peak and higher tails than normal distribution. 
  - is the difference in the models justified (e.g. does adding aditional parameter makes sense? ) [1/1 pt]
    - Yes. Data are characterized by big variety so trying another model may improve performance.
  - are models sufficiently described (what are formulas, what are parameters, what data are required ) [1/1 pt]
    - Yes. 
4. Priors [4/4 pts] 
  - Is it explained why particular priors for parameters were selected [1/1 pt]
    -Yes. Parameters has influence on the smog.
  - Have prior predictive checks been done for parameters (are parameters simulated from priors make sense) [1/1 pt]
    -No. [ 0/1 pt]
  - Have prior predictive checks been done for measurements (are measurements simulated from priors make sense) [1/1 pt]
    -The ppc for the smog has been done.
  - How prior parameters were selected [1/1 pt] 
    - Yes. Calculations were done for specific prior parameters.
5. Posterior analysis (model 1) [4/4 pts] 
  - were there any issues with the sampling? if there were what kind of ideas for mitigation were used [1/1 pt]
    - No sampling problems. 
  - are the samples from posterior predictive distribution analyzed [1/1 pt]
    - peak is significantly lower and shifted.
  - are the data consistent with posterior predictive samples and is it sufficiently commented (if they are not then is the justification provided) [1/1 pt]
    - densities have peak in the same place and tails are similar. 
  - have parameter marginal disrtibutions been analyzed (histograms of individual parametes plus summaries, are they diffuse or concentrated, what can we say about values) [1/1 pt]  
    - No. [ 0/1 pt ]
6. Posterior analysis (model 2) [4/4 pts] 
  - were there any issues with the sampling? if there were what kind of ideas for mitigation were used [1/1 pt]
    - No sampling problems
  - are the samples from posterior predictive distribution analyzed [1/1 pt]
    - peak is quite lower and shifted.
  - are the data consistent with posterior predictive samples and is it sufficiently commented (if they are not then is the justification provided) [1/1 pt]
    - densities have peak in the same place and tails are similar. 
  - have parameter marginal disrtibutions been analyzed (histograms of individual parametes plus summaries, are they diffuse or concentrated, what can we say about values) [1/1 pt]  
    - No. [ 0/1 pt ]
7. Model comaprison [4/4 pts]
  - Have models been compared using information criteria [1/1 pt]
    - Yes. 
  - Have result for WAIC been discussed (is there a clear winner, or is there an overlap, were there any warnings) [1/1 pt]
    - Smog Fit T_Student Model has a lower elpd_waic and a higher number of
    effective parameters  compared to the Smog Fit Normal Model. Smog Fit Normal Model has a higher elpd, indicating better out-of-sample prediction accuracy.
  - Have result for PSIS-LOO been discussed (is there a clear winner, or is there an overlap, were there any warnings) [1/1 pt]
    - Yes. Smog Fit T_Student Model performs better in terms of the expected predictive performance.
  - Was the model comparison discussed? Do authors agree with information criteria? Why in your opinion one model better than another [1/1 pt]
    - Model comparison was discussed and authors agree with information criteria.

Total grade will be converted to percentage.
 Total grade: 24/27 Percentage: 89%

Graded by: Jakub Majcher and Rafał Skrzypek :>


