# Markov-Churn-Subscription-Model
About this Project I built this model to find the Terminal Value of a subscription business (like Netflix) by calculating the steady-state equilibrium of its customer base. Most models just assume constant growth, but this model accounts for how the mix of customers changes over time.

How it Works

Eigenvector Analysis: The core of the model is a 4x4 transition matrix (Basic, Premium, Inactive, Churned). I used Eigenvector and Eigenvalue analysis to mathematically solve for the point where the subscriber mix stabilizes.

S-Curve Growth: I built a population growth vector that follows an S-curve (saturation) rather than infinite growth, making the long-term revenue projections more realistic.

Saturation Metrics: The model compares the current month's data against the calculated eigenvector to determine how close the business is to its revenue cap.
