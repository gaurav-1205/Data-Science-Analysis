# Data-Science-Analysis
These are the assignments of Data-Science-analysis coures offered by the Department of Astrophysics, IIT Hyderabad

### 1. Gaussianizing using BoxCox transformation
Download the eccentricity distribution of exoplanets from the exoplanet catalog http://exoplanet.eu/catalog/. Look for the column titled e,which denotes the eccentricity. Draw the histogram of this distribution. Then redraw the same histogram after Gaussianizing the distribution using Box-transformation either using scipy.stats.boxcox or from first principles using the equations in arXiv:1508.00931.
Ref : https://en.wikipedia.org/wiki/Power_transform#Box%E2%80%93Cox_transformation


### 2. CLT for Chi-Square-Distribution
Produce a plot for a sample drawn the from chi-square distribution with degrees of freedom equal to 3, for samples drawn once, 5 times, and 10 times and verify the Central Limit Theorem.
Ref : AstroML book fig 3.20


### 3. Histograms of bootstrap samples
Draw a similar histogram of median of 10,000 bootstrap samples drawn from the same Gaussian distribution. Refer to http://tinyurl.com/h6p43o8 for the details. Overlay a Gaussian distribution on top of the histogram with mean equal to the mean
of the generated data sample and standard deviation equal to the standard
deviation of the median. 


### 4. Chi-square curve fitting
Use Chi-square minimization to obtain best fit values for b and m for exercise 1 on page 5 in arxiv:1008.4686


### 5. Frequentist analysis
Download the data corresponding to x, y, and σy from http://www.iith.ac.in/~shantanud/testdata.dat. Find the best-fit values after fitting the data to linear, quadratic, and cubic polynomials. Find out which model fits the data best from frequentist model comparison as well as using AIC and BIC. For frequentist model comparison, using the linear model as the null hypothesis, find out the p value corresponding to the preferred model. Also show a plot overlaying the data with best fit solutions from linear, quadratic and cubic functions with different line styles for each of the fits.


### 6. Shapiro-Wilk Test
Download the asteroid dataset from http://astrostatistics.psu.edu/datasets/asteroid_dens.dat. Apply the Shapiro-Wilk test to both the asteroid density values and the natural logarithm of the density values. From the p values, which of these is closer to a Gaussian distribution? Verify this by plotting histograms of both density and its logarithm and overlaying the best-fit normal distribution.


### 7. 2 Sample T-test
Download the Hipparcos star catalog from http://astrostatistics.psu.edu/datasets/HIP_star.dat. Detailed explanation of the columns in this dataset can be found in http://astrostatistics.psu.edu/datasets/HIP_star.html under “Dataset”. Calculate using two-sample t-test whether the color of the Hyades stars differs from the non-Hyades ones. The Hyades stars have Right Ascension between 50◦ and 100◦ , declinations between 0 and 25◦ , proper motion in RA between 90 and 130 mas/year, proper motion in DEC between -60 and -10 mas/year, measurement parallax error less than 5 mas, and color of star less than 0.2 mag. Any other star which does not satisfy any of the above conditions is considered a non-Hyades star.


### 8. MCMC
For exercise 1 in arXiv:1008.4686, calculate the 68% and 95% joint confidence intervals on b and m.


### 9. Detecting Outliers using Bayesian analysis
Fit the data in Table 1 of arXiv:1008.4686 to a straight line, after including all the data points, (after ignoring σx and ρxy ) using both maximum likelihood analysis and using a Bayesian analysis to identify the outliers, using the same procedure as in the second of Jake VanDerPlas blog article. Show graphically the best fit line using both maximum likelihood analysis and also using Bayesian analysis, including the outlier points.
Ref : http://jakevdp.github.io/blog/2014/06/06/frequentism-and-bayesianism-2-when-results-differ/


### 10. Metropolis-Hastings MCMC algorithm
write a very simple M-H MCMC sampler. Sample in a single parameter x and give the sampler as its density function p(x) a Gaussian density with mean 2 and variance 2. Give the sampler a proposal distribution q(x0 | x) a Gaussian pdf for x0 with mean x and variance 1. Initialize the sampler with x = 0 and run the sampler for more than 104 steps. Plot the results as a histogram, with the true density over-plotted sensibly
Ref : arXiv:1710.06068


### 11. Using Kernel Density Estimation (KDE)
Download the SDSS quasar dataset from http://astrostatistics.psu.edu/datasets/SDSS_quasar.dat. Plot the KDE estimate of the quasar redshift distribution (the column with the title z) using a Gaussian and also an exponential kernel (with bandwidth=0.2) from -0.5 to 5.5.


### 12. Angular two-point correlation
Calculate the angular two-point correlation function of galaxies (including errors obtained by 10 bootstrap resamples) using subset of data from the Blanco Cosmology Survey in the 5 hour field with r-band magnitude between 17 and 20, and using 16 logarithmic-spaced angular bins from 1/60◦ to 1◦ . Use a linear scale for Y-axis. Galaxies in Blanco Cosmology Survey have spread model > 0.002. This data can be downloaded from http://www.iith.ac.in/~shantanud/BCS05hr_reduced.txt 
Ref : AstroML book fig 6.17
