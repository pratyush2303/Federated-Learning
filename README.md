# Federated-Learning

•	Engineered distributed deep learning framework by leveraging homomorphic encryption, customized for large-scale language models.
•	Fine-tuned language models (eg. BERT, MiniLM, Roberta, Deberta) for MRPC tasks within the GLUE benchmark, enhancing proficiency in natural language to 89.71% F-1 score in recreated model and averaged weights of data subsets in a federated model.

## MiniLM_Recreation file
In this notebook, I tried to recreate the MiniLM model by tuning the hyperparameters from Hugging Face under the GLUE benchmark for MRPC tasks.

## Dataset_split file
In this notebook, I divided the dataset into 8 shards for the model to learn on 8 different sets.

## MiniLM_FL file
Here, I trained the model on 8 shards and collected their learned weights.

## MiniLM_Federated_Averaging file
Here I averaged the weights from the previous 8 different trained models to a new Federated model and then tested the performance on the MRPC task.
