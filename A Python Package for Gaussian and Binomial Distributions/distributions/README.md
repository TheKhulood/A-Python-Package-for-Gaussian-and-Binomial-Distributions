Distributions Package

Overview:
This package provides classes to model and visualize two common probability distributions: Binomial and Gaussian (Normal). These classes allow you to perform statistical calculations and visualize distributions using the Matplotlib library.

Features:
1. Binomial Distribution:

Calculate the mean and standard deviation based on probability (p) and number of trials (n).
Replace statistics (p and n) with data.
Plot bar charts and probability distribution function (PDF) for the Binomial distribution.
Add two Binomial distributions together (with the same p value).

2. Gaussian Distribution:
Calculate the mean and standard deviation from data.
Plot histograms and probability density functions (PDF) for the Gaussian distribution.
Add two Gaussian distributions together.

Installation:
You can install the package using the following command:
pip install git+<repository-url>

Usage:
1. Import the Package
from distributions import Binomial, Gaussian

2. Binomial Distribution Example

# Create a Binomial distribution
binom = Binomial(prob=0.4, size=50)

# Calculate mean and standard deviation
mean = binom.calculate_mean()
stdev = binom.calculate_stdev()

# Plot a bar chart of the distribution
binom.plot_bar()

# Plot the probability distribution function (PDF)
binom.plot_bar_pdf()

# Add two Binomial distributions
binom2 = Binomial(prob=0.4, size=30)
binom_sum = binom + binom2

3. Gaussian Distribution Example
# Create a Gaussian distribution
gauss = Gaussian(mu=10, sigma=2)

# Calculate mean and standard deviation
mean = gauss.calculate_mean()
stdev = gauss.calculate_stdev()

# Plot a histogram of the data
gauss.plot_histogram()

# Plot the probability density function (PDF)
gauss.plot_histogram_pdf()

# Add two Gaussian distributions
gauss2 = Gaussian(mu=5, sigma=1)
gauss_sum = gauss + gauss2


Classes:

1. Binomial
This class is designed for calculating and visualizing the binomial distribution.

Methods:
__init__(prob=0.5, size=20): Initializes the binomial distribution with a probability of success p and n trials.
calculate_mean(): Returns the mean of the binomial distribution.
calculate_stdev(): Returns the standard deviation of the binomial distribution.
replace_stats_with_data(): Replaces the current p and n with values calculated from the data.
plot_bar(): Plots a bar chart of the distribution.
pdf(k): Returns the probability mass function (PMF) for a given value k.
plot_bar_pdf(): Plots the probability mass function (PMF).
__add__(other): Adds two Binomial distributions (with the same p).
__repr__(): Returns a string representation of the Binomial distribution.

2. Gaussian
This class is designed for calculating and visualizing the Gaussian distribution.

Methods:
__init__(mu=0, sigma=1): Initializes the Gaussian distribution with a mean mu and standard deviation sigma.
calculate_mean(): Returns the mean of the Gaussian distribution.
calculate_stdev(sample=True): Returns the standard deviation of the Gaussian distribution.
plot_histogram(): Plots a histogram of the data.
pdf(x): Returns the probability density function (PDF) for a given value x.
plot_histogram_pdf(n_spaces=50): Plots the PDF and histogram.
__add__(other): Adds two Gaussian distributions.
__repr__(): Returns a string representation of the Gaussian distribution.

Dependencies:
matplotlib: For plotting graphs and visualizing distributions.
math: For mathematical operations.

License:
This project is licensed under the MIT License - see the LICENSE file for details.