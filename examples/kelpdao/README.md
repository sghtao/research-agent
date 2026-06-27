# KelpDAO rsETH / LayerZero Reference Case

This directory documents the KelpDAO rsETH / LayerZero incident context as a reference case for the future `research-agent` workflow.

This is not a verified incident report. It is a structured starting point for future research fixtures, source collection, provenance tracking, and uncertainty labeling.

The legacy prompt at `prompts/kelp_rsETH_aave_composability.txt` is preserved as prior working material. It should not be treated as validated project output.

## Observed Facts

These are high-level facts that should be verified with citations before they appear in a final research note:

- KelpDAO issues or has issued rsETH as a liquid restaking-related asset.
- LayerZero is relevant to cross-chain messaging and bridge-related asset movement in the reference case.
- Aave-style lending markets are relevant to the analysis because collateral value, liquidity, oracle behavior, and liquidation mechanics can transmit stress.
- The reference case is intended to study composability risk across protocols, assets, and infrastructure layers.

## Questions to Verify

Future research should collect sources and answer:

- What exact event or incident is being analyzed?
- Which contracts, chains, bridges, markets, and assets were involved?
- What timeline is supported by primary sources?
- What official statements, governance posts, or postmortems exist?
- Which claims come from on-chain records, and which come from secondary analysis?
- Were lending markets directly affected, indirectly exposed, or only hypothetically exposed?
- What prices, oracle updates, liquidity changes, liquidations, or bad-debt figures are independently verifiable?
- Which claims conflict across sources?

## Analytical Hypotheses

These are possible lines of analysis, not historical facts:

- Cross-chain messaging or bridge assumptions may create delayed recognition of asset stress.
- Liquid restaking assets may carry risk from underlying validators, restaking protocols, liquidity venues, and bridge infrastructure.
- Lending markets may amplify stress when collateral assumptions change faster than liquidation liquidity.
- Oracle design, market depth, and withdrawal latency may determine whether stress remains isolated or propagates.
- Integrations that treat wrapped or bridged representations as equivalent may need explicit provenance and redemption-risk analysis.

## Simulated Stress-Test Ideas

These are modeling ideas only. They should not be presented as observed outcomes:

- Model a sudden rsETH price discount under different liquidity-depth assumptions.
- Simulate delayed oracle updates and compare liquidation timing.
- Estimate lending-market sensitivity under different collateral-factor assumptions.
- Compare outcomes when bridge redemption is immediate, delayed, paused, or uncertain.
- Stress-test downstream protocol exposure using manually supplied, cited market data.

Any future stress test should state assumptions, data sources, and limitations clearly.
