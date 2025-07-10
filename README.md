# VitaCare
This is a medical chat bot using generative AI.

# How to run VitaCare:

Step 1: Clone the repository
<br>
Step 1.5: Create a folder "data" and insert the medical book pdf you will use for data. Name it "medical_book.pdf". I was unable to upload mine because the file is too big.
<br>

Step 2: Create a conda environment after opening the repository
```bash
conda create --name llmpp python=3.10 -y
```
```bash
conda activate llmpp
```
Step 3: Install the requirements
```bash
pip install -r requirements.txt
```

### Create a `.env` file in the root directory and add your Pinecone & openai credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```


### Techstack Used:

- Python
- LangChain
- Flask
- Cohere LLM
- Pinecone