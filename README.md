
# WebR Trial Sequential Analysis (TSA) Engine

A serverless Trial Sequential Analysis calculator for Living Meta-Analyses.

## The Bottleneck
Living Meta-Analyses (like those on the Tiba dashboard) recalculate their pooled statistics every time a new trial is published. This constant "peeking" at the data massively inflates the Type I Error rate (false positives), similar to stopping a clinical trial early without statistical penalties.

## The Solution
This zero-backend WebR application runs Trial Sequential Analysis directly in the browser. 
It calculates the Required Information Size (RIS) and dynamically plots O'Brien-Fleming alpha-spending boundaries. If a living meta-analysis crosses the traditional p < 0.05 threshold, this engine verifies if it has also crossed the TSA boundary, preventing premature, fragile conclusions.

