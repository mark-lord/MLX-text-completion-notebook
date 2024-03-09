# MLX-text-completion-notebook
A simple Jupyter Notebook for learning QLoRA MLX text-completion fine-tuning.

### Brought to you by the Curriculum Protocol squad at [ValleyDAO](https://valleydao.bio)!

[**Quickstart**](#quickstart) | [**Roadmap**](#roadmap)

![https://valleydao.bio](valleydao.png)


## Quickstart

### Install
1. Follow these instructions to [install Jupyter Lab](https://jupyter.org/install)
2. Download this repo (or just the `.ipynb` file and the `requirements.txt`) to a folder on your Mac
3. Right click on the folder containing the files and select Open in Terminal
4. (Optional) Install [Virtualenv](https://sourabhbajaj.com/mac-setup/Python/virtualenv.html) to set up a virtual environment before installing the requirements.txt
5. (Optional) In the terminal, type `virtualenv venv` and then `source venv/bin/activate` to activate the virtual env
6. Run the command `pip3 install -r requirements.txt`
7. In the terminal, type `jupyter lab`
8. Open up the `.ipynb`

### Running the Notebook
1. Instructions are in the Notebook - go to Run > Run All Cells
2. Once you've run all cells, you've officially fine-tuned a model in MLX!
3. (Optional) Swap out the dataset for your own dataset


## Roadmap
As MLX becomes more advanced and different loss functions become possible, we'll release more Notebooks (such as for Instruction-tuning, DPO, PPO, etc.)
It's currently possible to target the MLP weights in MLX QLoRA, but it requires manually editing a file in the MLX-lm QLoRA tuner directory - which is a bit faffy. Once that becomes editable via config we'll release an updated Notebook.


## Citing MLX

The [MLX software suite](https://github.com/ml-explore/mlx/) was initially developed with equal contribution by Awni
Hannun, Jagrit Digani, Angelos Katharopoulos, and Ronan Collobert. If you find
MLX useful in your research and wish to cite it, please use the following
BibTex entry:

```
@software{mlx2023,
  author = {Awni Hannun and Jagrit Digani and Angelos Katharopoulos and Ronan Collobert},
  title = {{MLX}: Efficient and flexible machine learning on Apple silicon},
  url = {https://github.com/ml-explore},
  version = {0.0},
  year = {2023},
}
```
