# PyPSA AC–DC Network Optimization

This project examines electricity generation, wind curtailment, and investment decisions in a simplified European power system using PyPSA.

## Tasks

1. **Network Optimization and Generator Dispatch:** Optimize the meshed AC–DC network and examine generator dispatch decisions.

2. **Generation, Curtailment, and Storage:** Compare generation with electricity demand, identify wind curtailment, and discuss the potential role of energy storage.

3. **Single-Node Optimization and Investment Sensitivity:** Convert the network to a single node and examine how Norway Wind's capital cost affects investment in wind and gas capacity.

## Main Findings

- **Generator dispatch:** Wind supplies most electricity demand, while Frankfurt Gas operates at 05:00 and 09:00 to cover wind shortfalls.
- **Wind curtailment:** Significant wind curtailment occurs during some hours, highlighting the potential role of energy storage.
- **Investment sensitivity:** In the single-node model, Norway Wind begins replacing Frankfurt Gas when its capital cost falls below approximately 114.67.

## Tools

Python, PyPSA, HiGHS, pandas, NumPy, Matplotlib, and Jupyter Notebook.

## Reproducing the Analysis

Install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Then open `notebooks/meshed_ac_dc_network.ipynb` and run all cells.

## Reference

[PyPSA Meshed AC–DC LOPF Example](https://docs.pypsa.org/latest/examples/ac-dc-lopf/)