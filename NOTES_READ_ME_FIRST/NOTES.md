
# Limitations and Feedback Loops

## Nature of the Model Output

The Net Primary Productivity (NPP) calculated by this model represents a **potential or virtual NPP**. It is derived from the assumption that the entire available irradiance is efficiently captured by phytoplankton in a clear water column, without self-induced attenuation.

This means the NPP value corresponds to the *maximum possible productivity* under optimal conditions (e.g. pre-bloom, winter-clear water), and does **not** account for natural growth limitations such as:

- **Self-shading** due to increasing algal biomass
- **Light attenuation feedback**, where higher turbidity reduces available light for deeper cells
- **Nutrient limitations**, especially nitrogen or phosphorus
- **Zooplankton grazing** and food web interactions

## Feedback Mechanism

As algal biomass increases, it contributes to water turbidity. This increase in turbidity raises the attenuation coefficient (k), reducing the depth of the photic zone (Zeu) and the total irradiance available for photosynthesis.

This results in a **negative feedback loop**:

> High NPP potential → More algae → Increased turbidity → Higher k → Lower Zeu → Reduced irradiance → Lower actual NPP

The model currently does **not dynamically simulate** this loop. However, this conceptual framework is essential to interpret the output properly.

## Recommendation

This model is best used:
- As an educational/scientific exploration tool
- For comparative scenarios (clear vs. turbid waters)
- In conjunction with **manual k adjustments** based on real turbidity feedback

For dynamic simulations, coupling this model with a time-stepped ecological model is recommended (e.g., logistic growth with turbidity-dependent light attenuation).
