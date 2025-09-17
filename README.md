# Paper-Helicopter-DOE
This project applies Design of Experiments (DOE) methodology to a simple paper helicopter experiment to study the effects of design factors on flight time. The analysis is done in R using a 2³ full factorial design.
# Experiment Oerview
Objective: Identify which design factors maximize the flight time of a paper helicopter.
Factors studied:
Rotor Length (7.5 cm vs 8.5 cm)
Rotor Width (3.5 cm vs 5.0 cm)
Paper Clip (0 vs 2 clips)
Design: Full factorial 2³ design
Replicates: 3 per treatment combination
Total runs: 24
Response: Flight time (seconds) from release to ground contact
# Analysis Overview
Data Collection: Measured flight times across 24 runs with different factor settings.

Factor Coding: Converted factors to coded levels (-1, +1) for DOE analysis.

Exploratory Analysis: Boxplots and summary statistics for treatments and factors.

ANOVA (Analysis of Variance): Tested significance of main effects and interactions.

Model Diagnostics: Checked ANOVA assumptions (residuals, normality, homoscedasticity).

Final Model: Main-effects linear regression model for prediction.

Optimal Settings: Identified the best combination of factor levels.
# Results
Significant Factors:

Rotor Length: Longer rotors increase flight time.
Rotor Width: Narrower rotors increase flight time.
Paper Clips: Adding clips decreases flight time.

Optimal Helicopter Design:

Rotor Length = 8.5 cm (long)
Rotor Width = 3.5 cm (narrow)
Paper Clip = 0 (no clip)
→ Predicted flight time: ~4.15 s

# Packages Used
R (tidyverse, ggplot2, plotly, car, broom, GGally, patchwork)
Quarto / RMarkdown for report generation

# Conclusion
Even a simple classroom experiment demonstrates how DOE methods help identify the most influential factors and optimize performance. In this case, the optimal helicopter design is:
Long rotors, narrow width, and no clips → longest flight time.
