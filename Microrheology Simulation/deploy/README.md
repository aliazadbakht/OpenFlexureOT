# Optical Tweezers Microrheology Simulation

An interactive simulation demonstrating passive microrheology using optical tweezers. Probe the viscoelastic properties of different media by analyzing the Brownian motion of a trapped bead.

## Features

🔬 **Multiple Media Types**

1. Launch the simulation by opening this page.
2. Select a medium from the dropdown to change fluid properties.
3. Observe the bead motion across different media.
4. Analyze results:
   - MSD curve shows particle displacement behavior
   - G' and G'' show elastic vs viscous contributions
   - Compare different media to understand viscoelasticity

### Complex Viscosity

```
|η*(ω)| = √(G'² + G''²) / ω
```

For Newtonian fluids: `|η*| = η` (constant)
For viscoelastic fluids: `|η*|` decreases with frequency (shear thinning)

## Medium Properties

| Medium | η (Pa·s) | G₀ (Pa) | τ (s) | Behavior |
|--------|----------|---------|-------|----------|
| Water | 0.001 | 0 | — | Newtonian |
| 50% Glycerol | 0.006 | 0 | — | Newtonian |
| 80% Glycerol | 0.06 | 0 | — | Newtonian |
| PEO 0.1% | 0.003 | 0.5 | 0.01 | Weak viscoelastic |
| PEO 1% | 0.01 | 5 | 0.1 | Moderate viscoelastic |
| PEO 5% | 0.05 | 50 | 1.0 | Strong viscoelastic |
| Agarose 0.1% | 0.002 | 10 | 10 | Soft gel |
| Agarose 1% | 0.005 | 500 | 100 | Stiff gel |

## What to Explore

### 1. Newtonian vs Viscoelastic
- Start with Water: G' ≈ 0, only G'' (viscous loss)
- Switch to PEO 1%: Both G' and G'' are significant
- Notice the crossover frequency where G' = G''

### 2. Viscosity Effects
- Compare Water → 50% Glycerol → 80% Glycerol
- Watch how Brownian motion slows dramatically
- |η*| increases but remains frequency-independent

### 3. Gel Behavior
- Try Strong Gel (Agarose 1%)
- G' >> G'' at all frequencies (solid-like)
- Very restricted particle motion

### 4. Relaxation Time
- Compare polymers with different τ values
- Short τ (PEO 0.1%): Crossover at high frequency
- Long τ (Agarose): Crossover below measurement range
| PEO 1% | 0.01 | 5 | 0.1 | Moderate viscoelastic |
| PEO 5% | 0.05 | 50 | 1.0 | Strong viscoelastic |
| Agarose 0.1% | 0.002 | 10 | 10 | Soft gel |
| Agarose 1% | 0.005 | 500 | 100 | Stiff gel |

## What to Explore

### 1. Newtonian vs Viscoelastic
- Start with **Water**: G' ≈ 0, only G'' (viscous loss)
- Switch to **PEO 1%**: Both G' and G'' are significant
- Notice the crossover frequency where G' = G''

### 2. Viscosity Effects
- Compare **Water** → **50% Glycerol** → **80% Glycerol**
- Watch how Brownian motion slows dramatically
- |η*| increases but remains frequency-independent

### 3. Gel Behavior
- Try **Strong Gel (Agarose 1%)**
- G' >> G'' at all frequencies (solid-like)
- Very restricted particle motion

### 4. Relaxation Time
- Compare polymers with different τ values
- Short τ (PEO 0.1%): Crossover at high frequency
- Long τ (Agarose): Crossover below measurement range

## Files

| File | Description |
|------|-------------|
| `microrheology_simulation.html` | PyScript web version (standalone) |
| `microrheology_simulation.py` | Python/Matplotlib version |
| `microrheology_simulation.jsx` | React component version |
| `README.md` | This documentation |
>>>>>>> 9b4f15eb00e7bf64c8dd839cd200d67b0a9d2a33

## Applications

This simulation demonstrates principles used in:

- **Biophysics**: Cell mechanics, cytoplasm rheology
- **Soft Matter**: Polymer solutions, hydrogels
- **Pharmaceutical**: Drug delivery gel characterization
- **Food Science**: Texture analysis
- **Materials Science**: Complex fluid characterization

## Technical Details

- **Bead diameter**: 2 µm (silica)
- **Trap stiffness**: 1 pN/µm
- **Temperature**: 293 K (20°C)
- **Simulation**: PyScript (Python in browser)

## License

This simulation is part of the OpenFlexure Optical Tweezers project and is licensed under the CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S v2).

---

**Questions?** Open an issue on the GitHub repository!
