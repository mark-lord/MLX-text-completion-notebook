# MLX Text-completion Finetuning Notebook
A simple Jupyter Notebook for doing text-completion fine-tuning using QLoRA in the [MLX framework](https://github.com/ml-explore/mlx/). By default this Notebook fine-tunes TinyLlama 1.1b on 500 entries of the TinyStories dataset. It should be useable by any Apple Silicon MacBook with at least 16GB RAM.

### Brought to you by the Curriculum Protocol squad at [ValleyDAO](https://valleydao.bio)!

[**Quickstart**](#quickstart) | [**Roadmap**](#roadmap)

![https://valleydao.bio](ValleyDAO.png)


## Quickstart

### Install
1. Follow these instructions to [install Jupyter Lab](https://jupyter.org/install).
2. Download this repo (or just the `.ipynb` file and the `requirements.txt`) to a folder on your Mac.
3. Right click on that folder - i.e. the one containing your files - and select Open in Terminal.
4. (Optional) Install [Virtualenv](https://sourabhbajaj.com/mac-setup/Python/virtualenv.html) to set up a virtual environment before installing the requirements.txt.
5. (Optional) In the terminal, type `virtualenv venv` and then `source venv/bin/activate` to activate the virtual env.
6. Run the command: `pip3 install -r requirements.txt`.
7. In the terminal, type `jupyter lab`. The UI should open automatically - if it doesn't, there should be a URL in the terminal that you can copy and paste into your browser.
8. Once the UI is up, open up the `.ipynb` file (i.e. the Notebook).

### Running the Notebook
1. Instructions are in the Notebook! In short, simply click Run in the top left. There should be a drop down - select Run All Cells.
2. Once you've run all cells, you've officially fine-tuned a model in MLX!
3. (Optional) Swap out the dataset for your own dataset.


## Roadmap
- As the fantastic team behind MLX continues to work on bringing more features to MLX-lm and different loss functions become possible, we'll release more Notebooks (such as for Instruction-tuning, DPO, PPO, etc.)
- Additionally, it's currently possible to target the MLP weights and train at much higher rank in MLX QLoRA, but it requires manually editing a file in the MLX-lm QLoRA tuner directory - which is a bit faffy. Once that becomes editable via config we'll release an updated Notebook.
- The [mlx-tuning-fork](https://github.com/chimezie/mlx-tuning-fork) repo offers a few cool features - namely learning rate scheduling. Would be good to release an updated Notebook that makes use of the scheduler.
- Making a dataset from scratch with no coding knowledge can be more than half the battle when getting started. Would be great to release a Notebook that can either explain the process of creating a task-specific dataset in more accessible terms, or else abstract away the complexity of doing dataset curation. Or both. The [Augmentoolkit API fork](https://github.com/e-p-armstrong/augmentoolkit/tree/api-branch) is a great starting point for this sort of thing.


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
