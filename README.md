# Online Companion to "Flexible Ramping Product Procurement in Day-Ahead Markets" 
The online companion to the publication

> O. Yurdakul, E. Ela, and F. Billimoria, "Flexible Ramping Product Procurement in Day-Ahead Markets," 
> submitted to IEEE Transactions on Energy Markets, Policy and Regulation, 2024.

In this online companion, we furnish the results of the case studies reported in our publication. In our case studies, we generated the in-sample scenarios (i.e., the net load scenarios used in solving the stochastic unit commitment problem of the first market pass), and the out-of-sample scenarios (i.e., the net load scenarios used in simulating real-time market clearing) under different autocorrelation levels. The results obtained under the proposed st-FRP method, as well as the four other tested benchmark methods (nf-FRP, 90-FRP, 95-FRP, and 99-FRP) for different autocorrelation (ρ) levels are provided in

1. [ρ = 0.0](/results/rho_0.0)
2. [ρ = 0.2](/results/rho_0.2)
3. [ρ = 0.4](/results/rho_0.4)
4. [ρ = 0.6](/results/rho_0.6)
5. [ρ = 0.8](/results/rho_0.8)


In the folders corresponding to each ρ value, we provide the
- scenarios used by the first market pass of the st-FRP (proposed method) and the nf-FRP benchmark method (folders named `scenario_inputs`)
- inputs to the day-ahead market clearing models under each method (folders named `input_files`)
- real-time market clearing results obtained out-of-sample under each method (folders named `output_files`)

We provide the inputs and outputs under each method for different number of in-sample scenarios tested in our performance assessments, comprising `7`, `14`, `31`, `61`, `100`, and `150` in-sample scenarios. The inputs and outputs corresponding to each number of in-sample scenarios are provided in the folders starting with `snum_` inside the `scenario_inputs`, `input_files`, and `output_files` folders.

For the real-time market clearing results of each method obtained under each number of in-sample scenarios, we provide the 
- total system operation cost results in the `cost_results.json` file
- involuntary load shedding results in the `curtailment_results.json` file
- payments to the generators in the `payment_results.json` file
- payments by the loads in the `load_payment_results.json` file
- locational marginal price (LMP) results in the `lmp_results.json` file
- up-FRP price results in the `up_frp_price_results.json` file
- down-FRP price results in the `down_frp_price_results.json` file
which are located in the `output_files` folder of each experimental setup.

