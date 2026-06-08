# Macroeconomic Time Series Analysis (VECM)

This project applies a Vector Error Correction Model (VECM) to real monthly macroeconomic time series data sourced from ARMSTAT (Statistical Committee of Armenia), including Inflows, Outflows, USD, EUR, RUR exchange rates, and the EA_index.

- The dataset is preprocessed and time-aligned to ensure consistent monthly frequency.
- Stationarity tests are performed to confirm that variables are integrated of order I(1).
- Johansen cointegration testing is used to identify long-run equilibrium relationships and justify the VECM framework.
- VAR-based lag selection is applied to capture appropriate short-run dynamics in the system.
- Structural breaks around 2014-08-01 and 2022-02-01 are included to account for major economic and geopolitical shocks, with evidence of increased volatility in inflows and outflows during war-related periods driven by uncertainty and capital reallocation effects.

The estimation output is stored in `report.md`, which contains the full VECM results including short-run equations, error-correction (alpha) coefficients, and long-run cointegration (beta) relationships. The alpha coefficients describe the speed at which variables adjust back to equilibrium, while the beta vectors define the long-run equilibrium relationships between variables.
