### Project Overview
This project implements the PLANNER model, which is designed to generate diversified paragraphs using a latent language diffusion model. The model combines latent semantic diffusion with autoregressive generation to produce fluent text while maintaining global control over the content. The project is based on the methodology and code presented in the base paper "PLANNER: Generating Diversified Paragraph via Latent Language Diffusion Model" by Yizhe Zhang et al., 2024 (see the attached PDF for more details).

### Running the Project
- Unzip the Project Folder:
- Download and unzip the project folder to your local machine.
- Open Jupyter Notebook:
- Navigate to the unzipped project folder and open the train_sample.ipynb file using Jupyter Notebook. You can start Jupyter Notebook by running the following command in your terminal:
	- jupyter notebook
	- Run the Notebook:
- Execute all the cells in the train_sample.ipynb notebook. This notebook contains all the commands needed to train and evaluate the PLANNER model. The notebook also includes the output of a successful run at the end.

### Dependencies
Ensure that you have the following dependencies installed before running the notebook:

- Python 3.7 or higher
- PyTorch
- Transformers (Hugging Face)
- Numpy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

You can install the necessary dependencies using pip:

- pip install torch transformers numpy scikit-learn matplotlib jupyter

### Project Structure
- train_sample.ipynb: Jupyter Notebook containing the code for training and evaluating the model.
- data-bin/: Directory containing any required datasets (if applicable).
- text_autoencoder/: Directory where all the python files are being saved, and used for training the model
- outputs/: Directory where the model outputs and logs are saved.
- figures/: Directory where the images are being stored
- README.md: This file.


### Challenges and Limitations
#### Experienced Challenges
**Computational Resources**:
The primary challenge faced during the development of this project was the lack of sufficient computational resources. Training the PLANNER model requires significant GPU memory and computational power. This limitation affected the training time and the size of the datasets we could use.

#### Upcoming Challenges
**Scalability**:
Scaling the model to handle larger datasets and more complex text generation tasks could present further computational challenges.

**Fine-tuning**:
Fine-tuning the model for specific applications or domains may require substantial experimentation with hyperparameters and architecture adjustments.

**Deployment**:
Deploying the model in a production environment may require optimization to reduce inference time and computational load.

##### Perceived Limitations
**Fluency vs. Diversity**:
While the model aims to generate diversified lyrics, there may be trade-offs between the fluency and diversity of the generated lyrics. Ensuring high-quality output across various use cases remains a challenge.

**Repetition**:
Despite improvements over autoregressive models, the diffusion process can still lead to repetitive outputs, especially for longer texts.

**Resource-Intensive**:
The diffusion model, by its nature, involves multiple iterations over the text, making it more resource-intensive compared to simpler autoregressive models.

#### References
For more detailed information about the model and its implementation, please refer to the base paper included in this project: PLANNER: Generating Diversified Paragraph via Latent Language Diffusion Model by Yizhe Zhang et al., 2024.

For any questions or further assistance, please feel free to mail  us
