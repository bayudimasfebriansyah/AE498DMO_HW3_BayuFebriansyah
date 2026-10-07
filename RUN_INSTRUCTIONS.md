# Run my HW3 notebooks

I use Python 3.12 and install the packages in `requirements.txt`:

```powershell
python -m pip install -r requirements.txt
python -m jupyter lab
```

I select the same Python environment as the notebook kernel and run each notebook from top to bottom.

- I use `hw3_pytorch.ipynb` for Problem 1. Its first run downloads ResNet-18 weights and CIFAR-10 into `data/`, so I need internet access for those downloads. Later runs reuse the cache.
- I use `hw3_bts.ipynb` for Problem 2. I keep `T_ONTIME_REPORTING.csv` and `hw3_split_indices.npz` in the same folder. The split file stores the exact row indices for training, validation, cutoff calibration, and testing.

I use the fixed NN and KNN settings shown in Problem 2. I train the NN for nine epochs and calculate the final test results after cutoff calibration. Both notebooks include refreshed outputs from a complete run. Timings can vary across machines, and exact numerical results can vary across package versions or hardware.

I submit both notebooks through the assignment repository and submit that repository on Gradescope, following `README.md`.
