# A-Python-Package-for-Gaussian-and-Binomial-Distributions
This repository contains a Python package that allows users to perform calculations and visualize Gaussian and Binomial distributions, offering easy-to-use methods for statistical operations and plotting.

# Distributions: Gaussian and Binomial Distributions Package

This repository contains a Python package for creating, calculating, and visualizing Gaussian (Normal) and Binomial distributions. The package provides methods to calculate the mean, standard deviation, and probability density or mass functions. Users can also visualize these distributions using the Matplotlib library.

## Features

- **Binomial Distribution:**
  - Compute the mean and standard deviation.
  - Generate bar charts and probability mass function (PMF) plots.
  - Add two Binomial distributions together (if they have the same `p` value).

- **Gaussian Distribution:**
  - Compute the mean and standard deviation from data.
  - Visualize data with histograms and probability density function (PDF) plots.
  - Add two Gaussian distributions together.

## Installation

To install the package, clone the repository and use the following command:

```bash
pip install .
```

Alternatively, you can install the package directly from the repository:
pip install git+<repository-url>

Usage
1. Import the package
from distributions import Binomial, Gaussian

2. Using the Binomial Distribution
**Create a Binomial distribution**

binom = Binomial(prob=0.4, size=50)

**Calculate mean and standard deviation**

print(binom.calculate_mean())   # Output: mean value
print(binom.calculate_stdev())  # Output: standard deviation

**Plot a bar chart**

binom.plot_bar()

**Plot the probability distribution function**

binom.plot_bar_pdf()


3. Using the Gaussian Distribution


**Create a Gaussian distribution**

gauss = Gaussian(mu=10, sigma=2)


**Calculate mean and standard deviation**

print(gauss.calculate_mean())   # Output: mean value

print(gauss.calculate_stdev())  # Output: standard deviation


**Plot histogram**

gauss.plot_histogram()


**Plot the probability density function**

gauss.plot_histogram_pdf()


## Dependencies

matplotlib: Used for plotting charts and visualizing distributions.

math: Used for mathematical operations.
