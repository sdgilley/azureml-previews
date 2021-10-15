# Quickstart: Deploy the model (preview)

Now that you've trained a model, it's time to deploy it to predict scores for new data. Completing this quickstart incurs a small cost of approximately 10 USD cents in your Azure account.

In this quickstart, you'll use the job creation wizard to submit a training job.  You'll learn how to:

* Register a model
* Deploy the model to a managed inference
* Try out the model with some new sample data

## Prerequisites

Complete either one of these quickstarts:

* [Quickstart: Try it out with a sample model (preview)](quickstart-train-model-sample.md)
* [Quickstart: Train your own model with the job creation wizard (preview)](quickstart-train-model.md)
 

## Download model

To start, you'll download a model that you've already trained.

1. Start by signing into Azure Machine Learning [studio](https://ml.azure.com)
1. Access the private preview
1. On the left, select **Experiments**.
1. Select the experiment that contains the model (for example, sklearn-iris-example for the model created from [Quickstart: Try it out with a sample model (preview)](quickstart-train-model-sample.md)).
1. Select the link on the display name for the run.
1. Select the **Output + logs** tab.
1. Select **Download all** in the tools above the tabs.

    ![ Screenshot: Download output from training run. ](../media/quickstart-deploy-model/download-all.png)

1. Locate the downloaded folder and extract all contents if it is a zipped file.

1. Name the model **iris-classification**
1. For the **Model framework**, select **scikitlearn**.
1. For the **Framework version** enter **0.24.1**
1. for the **Model file or folder**, select **Upload folder**
1. Select **Browse**, and select the *model* folder inside your downloaded output folder.
1. Select **Upload** on the prompt to confirm the upload of four files.
1. Select **Register**.

## Deploy the model

1. Select **Home** to return to the studio homepage
1. Select **Deploy your model**.

    ![ Screenshot: Deploy your model wizard on the homepage. ](../media/quickstart-deploy-model/deploy-your-model.png)

Fill out the **Create deployment (preview)** wizard as shown in the following sections.

### Endpoint

1. For **Endpoint name**, enter **iris-endpoint**
1. Leave the rest of this page with default values.
1. Select **Next**

### Model

 1. Select **+ Register model**
1. Name the model **iris-classification**
1. For the **Model framework**, select **scikitlearn**.
1. For the **Framework version** enter **0.24.1**
1. for the **Model file or folder**, select **Upload folder**
1. Select **Browse**, and select the *model* folder inside your downloaded output folder.
1. Select **Upload** on the prompt to confirm the upload of four files.
1. Select **Register**.
1. Select the model **iris-classification** in the list.
1. Select **Next**.
