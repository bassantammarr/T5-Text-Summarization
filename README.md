# T5-Text-Summarization
## Project Overview
This project fine-tunes a T5 transformer model for sequence-to-sequence tasks such as summarization. It leverages Hugging Face’s Transformers and Datasets libraries to build a complete pipeline from raw text data to a deployable model.

## Project Workflow
**1. Data Preparation**

- Collected and structured text data into input (source text) and target (summary text) fields.

- Converted the dataset into Hugging Face’s Dataset format for efficient handling.

- Split the data into training and validation sets.

**2. Model & Tokenizer Setup**

- Loaded a pretrained T5-small model and its tokenizer from Hugging Face.

- Defined a preprocessing function to tokenize and format the data for model input and output.

**3. Preprocessing**

- Applied tokenization to both input and target texts.

- Padded and truncated sequences to ensure uniform length.

- Aligned labels with input sequences for supervised training.

**4. Training Configuration**

- Defined training hyperparameters such as learning rate, batch size, epochs, and evaluation strategy.

- Set up logging, checkpoint saving, and best-model tracking.

**5. Model Training**

- Trained the T5 model on the tokenized dataset using Hugging Face’s Trainer API.

- Evaluated performance on the validation set at regular intervals.

**6. Model Evaluation**

- Assessed the model’s performance using validation metrics.

- Monitored training logs to ensure convergence and avoid overfitting.


