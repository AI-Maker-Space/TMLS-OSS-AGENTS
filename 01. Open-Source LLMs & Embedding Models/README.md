## Build 🏗️

### Build Task 1: Deploy LLM and Embedding Model to SageMaker Endpoint Through Hugging Face Inference Endpoints

#### LLM Endpoint

Select "Inference Endpoint" from the "Solutions" button in Hugging Face:

![image](https://i.imgur.com/6KC9TCD.png)

Create a "+ New Endpoint" from the Inference Endpoints dashboard.

![image](https://i.imgur.com/G6Bq9KC.png)

Select the `NousResearch/Hermes-2-Pro-Llama-3-8B` model repository and name your endpoint. Select N. Virginia as your region (`us-east-1`). Give your endpoint an appropriate name. Make sure to select *at least* a L4 GPU. 

![image](https://i.imgur.com/X3YlUbh.png)

Select the following settings for your `Advanced Configuration`.

![image](https://i.imgur.com/c0HQ7g1.png)

Create a `Protected` endpoint.

![image](https://i.imgur.com/Ak8kchZ.png)

If you were successful, you should see the following screen:

![image](https://i.imgur.com/IBYG3wm.png)

#### Embedding Model Endpoint
We'll be using `Snowflake/snowflake-arctic-embed-m` for our embedding model today.

The process is the same as the LLM - but we'll make a few specific tweaks:

Let's make sure our set-up reflects the following screenshots:

![image](https://i.imgur.com/IHh8FnC.png)

After which, make sure the advanced configuration is set like so:

![image](https://i.imgur.com/bbcrhUj.png)

> #### NOTE: PLEASE SHUTDOWN YOUR INSTANCES WHEN YOU HAVE COMPLETED THE ASSIGNMENT TO PREVENT UNESSECARY CHARGES.

### Build Task 2: Access the Endpoints With the Notebook!

Follow the [notebook](https://colab.research.google.com/drive/1OHvE-myskVE2NQZ5EQhN8sb47VGYEmby?usp=sharing) to learn how to access the Hugging Face Inference Endpoint API like a developer!

> #### NOTE: PLEASE SHUTDOWN YOUR INSTANCES WHEN YOU HAVE COMPLETED THE ASSIGNMENT TO PREVENT UNESSECARY CHARGES.