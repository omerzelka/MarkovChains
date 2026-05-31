# Regional Migration Model: Markov Chain Simulation 🏙️🏡🌳

This project is an interactive web simulation that models the movement of a population across three different regions (City, Suburb, Rural) as a **Markov Chain**, and analyzes the long-run behavior (steady-state) of this population.

> 🚀 **Live Application:** Click [Here](INSERT_YOUR_GITHUB_PAGES_LINK_HERE) to run the simulation directly in your browser. No installation required!

## 📌 Project Purpose & Theoretical Background

The primary objective of this study is to demonstrate that the long-run behavior of a Markov chain is governed entirely by the eigenvalues and eigenvectors of its transition matrix:

* **Steady-State:** The eigenvalue $\lambda = 1$ — which every stochastic matrix possesses — yields the steady-state distribution as its eigenvector. In our model, this theoretical equilibrium is calculated as $(9/28, 3/7, 1/4)$.
* **Rate of Convergence:** The remaining eigenvalues (e.g., $\lambda = 0.3$ and $\lambda = 0.2$), all of magnitude less than $1$, control how fast the population converges to that steady state (the spectral gap).

Even if the starting population is radically concentrated in a single region (for instance, everyone initially in the City: $\mathbf{x}_0 = (1, 0, 0)^T$), the system strictly converges to the theoretical equilibrium limits within a few iterations (years).

## 🛠️ Application Features

The simulation runs entirely on the client-side (in the browser) and is developed using HTML, JavaScript, and Chart.js.

* **Interactive Matrix Input:** You can dynamically update the $3 \times 3$ transition matrix of the project.
* **Dynamic Population Distribution:** Test different scenarios by allocating the initial population across the City, Suburb, and Rural areas.
* **Graphical Convergence:** Observe the evolution of the population over the years and its settlement into asymptotic limits through dynamic line charts.
* **Data Table:** For analytical verification, an evolution table provides a breakdown of each iteration ($t=0, 1, 2, ...$) rounded to $3$ decimal places. The table also calculates the ultimate limit state at $t = \infty$.

## 💻 How to Run

### Option 1: Via Web (Recommended)
You can instantly test the application without downloading any files:
👉 **[Go to Live Simulation](INSERT_YOUR_GITHUB_PAGES_LINK_HERE)**

### Option 2: Local Machine
If you prefer to run the project offline on your local computer:
1. Download or clone this repository to your machine.
2. Double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Safari, etc.).

---
*This project was created for the practical demonstration of Markov Chains and Linear Algebra principles through numerical simulations.*
