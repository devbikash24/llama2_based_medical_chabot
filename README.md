# llama2-based medical chatbot

# How to run?
### STEPS:

### STEP 01- Clone the repository


### STEP 02- Create and activate a virtual environment after opening the repository


### STEP 03- install the requirements

```bash
pip install -r requirements.txt
```

### step 04- Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### step 05- Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

### step 06- In pinecone database, create a index with name "medical-chatbot-1" and dimension :

### step 07- Run store_index.py to create embedding and store embedding in pineconde database :

```bash
# run the following command
python store_index.py
```

### step 08- Run app.py to run the application

```bash
# Finally run the following command
python app.py
```


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- Pinecone


### Few Screenshots

![app1](https://github.com/user-attachments/assets/8769d193-92a8-4bdc-8d61-0de1cc15e7e7) 

![app2](https://github.com/user-attachments/assets/11eedb40-c7ba-4d6a-9718-e743975df2bf)


