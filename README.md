
# Swaption

This repository contains examples and practical code related to **Swaptions**.  
A swaption is an option that grants the right to enter into an **Interest Rate Swap**  
under predefined conditions at a specific point in time (maturity).

## Basic Structure of a Swaption
- **Payer Swaption**: The right to enter into a swap at maturity where you **pay** a fixed rate and **receive** a floating rate.
- **Receiver Swaption**: The right to enter into a swap at maturity where you **receive** a fixed rate and **pay** a floating rate.

In the simplest example, the payoff can be calculated by comparing a single-period fixed rate ($K$) with a single floating rate ($F$):

- **Payer Swaption Payoff**  
  ${Payoff} = N \times \tau \times \max(F - K, 0)$
  - $N$: Notional
  - $\tau$: Year fraction for the period (e.g., 0.5 = 6 months)
  - $F$: Floating rate (Forward rate)
  - $K$: Strike rate

- **Receiver Swaption Payoff**  
  $
  \text{Payoff} = N \times \tau \times \max(K - F, 0)
  $

## File Structure
- `README.md`: Explanation of the basic concepts of swaptions and folder structure
- `simple_swaption_example.ipynb`: Example code for calculating a simple swaption payoff (Jupyter Notebook)

## How to Use
1. Clone or download this repository.
2. Run Jupyter Notebook from the terminal (or command prompt):
   ```bash
   jupyter notebook
   ```
