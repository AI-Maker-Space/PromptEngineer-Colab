# E2E - Inference Endpoints Hugging Face

In today's event, we'll create an E2E Application through Hugging Face Inference Endpoints!

There are 2 main sections to this event:

### Deploy LLM and Embedding Model to SageMaker Endpoint Through Hugging Face Inference Endpoints

Select "Inference Endpoint" from the "Solutions" button in Hugging Face:

![image](https://i.imgur.com/6KC9TCD.png)

Create a "+ New Endpoint" from the Inference Endpoints dashboard.

![image](https://i.imgur.com/G6Bq9KC.png)

Select the `ai-maker-space/gen-z-translate-llama-3-instruct-v1` model repository and name your endpoint. Select N. Virginia as your region (`us-east-1`). Give your endpoint an appropriate name.

Select the following settings for your `Advanced Configuration`.

![image](https://i.imgur.com/c0HQ7g1.png)

Create a `Protected` endpoint.

![image](https://i.imgur.com/Ak8kchZ.png)

If you were successful, you should see the following screen:

![image](https://i.imgur.com/IBYG3wm.png)

You'll repeat the same process for your embedding model!

> #### NOTE: PLEASE SHUTDOWN YOUR INSTANCES WHEN YOU HAVE COMPLETED THE ASSIGNMENT TO PREVENT UNESSECARY CHARGES.

### Create a Simple Chat Application leveraging the new endpoint!

First, we [fine-tune](https://colab.research.google.com/drive/1TX-N9E7lESNkxIrFEC6sn0rMMfYRCmKg#scrollTo=iRGG0QCNwT6J) Llama 3 8B Instruct for a specific task, in this case: A translation task!

Then, we create a Docker Hugging Face space powering a Chainlit UI - code available [here](https://huggingface.co/spaces/ai-maker-space/GenZAI/tree/main)

### Terminating Your Resources

Please go to each endpoint's settings and select `Delete Endpoint`. To delete the resources, you will need to type the endpoint's name.
