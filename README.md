# E2E - Inference Endpoints Hugging Face

In today's assignment, we'll be creating an Open Source LLM-powered LangChain RAG Application.

There are 2 main sections to this assignment:

### Deploy LLM and Embedding Model to SageMaker Endpoint Through Hugging Face Inference Endpoints

Select "Inference Endpoint" from the "Solutions" button in Hugging Face:

![image](https://i.imgur.com/6KC9TCD.png)

Create a "+ New Endpoint" from the Inference Endpoints dashboard.

![image](https://i.imgur.com/G6Bq9KC.png)

Select the `meta-llama/Meta-Llama-3-8B-Instruct` model repository and name your endpoint. Select N. Virginia as your region (`us-east-1`). Give your endpoint an appropriate name.

Select the following settings for your `Advanced Configuration`.

![image](https://i.imgur.com/c0HQ7g1.png)

Create a `Protected` endpoint.

![image](https://i.imgur.com/Ak8kchZ.png)

If you were successful, you should see the following screen:

![image](https://i.imgur.com/IBYG3wm.png)

You'll repeat the same process for your embeddings model!

> #### NOTE: PLEASE SHUTDOWN YOUR INSTANCES WHEN YOU HAVE COMPLETED THE ASSIGNMENT TO PREVENT UNESSECARY CHARGES.

### Create RAG Pipeline with LangChain & LangSmith

We'll work through this week's notebook after setting up our endpoints!

The notebook will be broken into the following parts:
 
The Colab link is provided [here](https://colab.research.google.com/drive/1CVHGdSDFhfeyGl20ZK-f52lst3xqKVCf?usp=sharing)

### Terminating Your Resources

Please head to the settings of each endpoint and select `Delete Endpoint`. You will need to type the name of the endpoint to delete the resources.
