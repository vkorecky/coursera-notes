# Gaussian distribution

**What makes the Gaussian distribution useful and important?**

1. Only two parameters are needed to specify the Gaussian. They are called the **mean** and **variance**, and they capture the essense of the distribution. They are also easy to compute and interpret.
2. Mathematically the distribution has some nice properties. For example, product of Gaussian distributions forms another Gaussian. So you don't need to worry about encountering other forms of distributions when you perform operations on the Gaussian model.
3. More theoretically, the central limit theorem tells us that the expectation of the mean of any random variable converges to the Gaussian distribution.

*Gaussian is a proper choice for modeling noise and uncertainty.*

## 1D Gausian distribution
Gaussian distribution is expressed as an exponential term multiplied by a scalar.

We want to know the probability that **$x$**, the variable, lies within our Gaussian distribution. We call this probability density function. We use **$p(x)$** to write this. **$\mu$** is the mean of our Gaussian and **$\sigma$** is its standard deviation. We call **$\sigma^2$** variance.

\[
p(x) = \frac{1}{\sqrt{2\pi\sigma}}\exp\Big\{-\frac{(x-\mu)^2}{\sqrt{2\sigma^2}}\Big\}
\]

- **$x$** variable
- **$\mu$** mean
- **$\sigma^2$** variance
- **$\sigma$** standard deviation
- **$p(x)$** probability that the variable **$x$**, lies within our Gaussian distribution

### Gaussian distribution with different **$\mu$** mean and **$\sigma^2$** variance

![We'll first consider when a distribution has zero mean and univariance. This is a often called the **standard normal distribution**. If you'll look at the graph and look inside the exponential parts of the expression, you will see this distribution is symmetric about the mean, which is 0 in this case. Also you should notice that the value of **$p(x)$** gets very small as **$x$** goes far from the mean. This is due to the minus sign inside the exponential function. The last thing to notice is the scalar term outside the exponential function. Remember Gaussian is a probability distribution and thus its integral, the integral of p(x), must be 1. Now let's consider other cases with different values for the mean.](images/gaussian_distribution_01.png)

![The gray curve is a standard Gaussian curve. Compared to this, when the mean is -1, the curve is shifted to the left by 1.](images/gaussian_distribution_02.png)

![If the mean is 1, the graph is shifted to the right by 1. The mean value determines the center of the distribution. Critically, the actual shape has not been changed, only shifted.](images/gaussian_distribution_03.png)

![If the variance increases to 2, the curve spreads out as compared to the standard Gaussian curve. Also, the peak value decreases so that the integral is still 1, which fulfills the properties of a probability density function.](images/gaussian_distribution_04.png)

![Conversely, a smaller variance tightens the curve and the peak value becomes bigger as well. So that the integral remains 1.](images/gaussian_distribution_05.png)

![We have seen the two parameters of the Gaussian distribution. The mean mu represents the center of the distribution. And the variance sigma squared represents the spread of the distribution.](images/gaussian_distribution_06.png)
