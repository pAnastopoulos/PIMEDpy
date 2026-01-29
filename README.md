# PIMEDpy – Probabilistic Implementations for Marine Engineering Dynamics in Python

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Planning-orange)

**A Python toolkit for simulation of marine environment excitations and probabilistic dynamics of ships and other floating structures.**



## About

PIMEDpy is a Python toolkit focused on **probabilistic and statistical analysis of marine engineering system dynamics**. It provides practical tools for:

- Simulating marine environment excitations such as waves, wind, and currents, with emphasis on extreme events.  
- Estimating motions of ships and other floating structures based on practical models.  
- Assessing dynamic behaviour through probability calculation and uncertainty quantification.

The toolkit is intended for research and applied studies. Resulting workflows enable inferences based on minimal input data.



## Features

- Probabilistic modelling of marine environmental loads — including waves, wind, and currents.  
- Time-domain simulation of dynamic responses of marine engineering systems.  
- Statistical post-processing of simulation results for performance assessment.  
- Flexible application to ships and offshore structures.  
- Pure Python implementation — easy to install, extend, and integrate with other workflows.



## Installation

Installation instructions will be provided with the first release, including options for installation from **PyPI** or directly from **GitHub**.



## Quick Example / Usage

```python
import pimedpy

# Define environmental conditions and ship/floating structure data
environment = {
    'waves': {'spectrum': 'JONSWAP', 'significant_height': 3.0, 'peak_period': 8.0},
    'wind': {'mean_speed': 10.0},
    'current': {'speed': 1.0}
}

ship_data = {
    'length': 100.0,
    'beam': 20.0,
    'draft': 6.0,
    'engine_power': 5000.0
}

# Run a probabilistic simulation
response = pimedpy.simulate_response(environment, ship_data, n_realizations=1000)

# Perform statistical post-processing
summary = pimedpy.analyze_response(response)
print(summary)
```



## Documentation & Support

Full documentation, examples, and support resources will be provided with the first release.



## Author & Maintainer

Panayiotis A. Anastopoulos, PhD (Naval and Marine Engineering NTUA)  
All development, design, and research for PIMEDpy have been carried out by the author.  
Contributions and collaborations are welcome. Early access and questions are encouraged.  

**Contact:** pa_anasto@yahoo.gr



## License

PIMEDpy will be released under the MIT License.
