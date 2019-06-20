# Exotic_Option_Pricing
Bermuda and Knock-out European Barrier Option pricing with Crank-Nicolson finite difference approximation

All options satisfy the Black-Scholes equation. What differs among these options are the boundary
conditions. Different options come with different sets of boundary conditions.

Using Crank-Nicolson method, price and calculate Delta, Gamma, and Theta for the following options:
  1. Bermuda Call and Put options of the following parameters:
    (𝑆0,𝐾, 𝜎, 𝑟, 𝑑) = (100, 100, 40%, 2.5%, 1.75%)
    
    Options are exercisable monthly with the final Maturity = 1 year (you want to have these
    exercise times coincide with time grid points)
    
  2. Knock-out European Barrier Options, 𝐻 is the level of the barrier (You want to set up your grids
    so the barrier(s) coincide with a grid point(s)).
      a. Up-and-out call: (𝑆0,𝐾, 𝐻, 𝑇, 𝜎, 𝑟, 𝑑) = (100, 110, 120, 1.0, 50%, 2.5%, 1.75%)
      b. Up-and-out put: (𝑆0,𝐾, 𝐻, 𝑇, 𝜎, 𝑟, 𝑑) = (100, 90, 120, 1.0, 50%, 2.5%, 1.75%)
      c. Double knock-out put:
        (𝑆0,𝐾, 𝐻𝑢𝑝, 𝐻𝑑𝑜𝑤𝑛, 𝑇, 𝜎, 𝑟, 𝑑) = (100, 90, 120, 80, 1.0, 50%, 2.5%, 1.75%)
        Plot Gamma vs. stock price on the evaluation date for this double knock-out put.
