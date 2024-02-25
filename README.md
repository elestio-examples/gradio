# Gradio CI/CD pipeline

<a href="https://dash.elest.io/deploy?source=cicd&social=dockerCompose&url=https://github.com/elestio-examples/stable-diffusion"><img src="deploy-on-elestio.png" alt="Deploy on Elest.io" width="180px" /></a>

Deploy Gradio with CI/CD on Elestio

<img src="stable-diffusion.png" style='width: 100%;'/>
<br/>
<br/>

# Once deployed ...

You can open Gradio here:

    URL: https://[CI_CD_DOMAIN]
    login: root
    password: [ADMIN_PASSWORD]

# Pulling a Model

To effortlessly pull a model into your project, adhere to the following steps:

## Using Elestio Dashboard

Navigate to the Elestio dashboard and click on Open terminal.

In the terminal, input the following command to access the appropriate directory:

    cd ./storage/models/Stable-diffusion

## Obtaining the Model

Copy the download URL for your desired model. Ensure that the URL adheres to the following format:

    https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/resolve/main/sd_xl_base_1.0.safetensors

In the terminal, use the wget command to pull the model. Replace <your-model> and <your-url> with the appropriate names:

    wget -O <your-model>.safetensors <your-url>

For instance:

    wget -O sd_xl.safetensors https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/resolve/main/sd_xl_base_1.0.safetensors

## Applying Changes

Once the download is complete, return to the Gradio UI.

Click on the Refresh button located at the top left of the UI.

Select your newly downloaded model from the refreshed list.

Your model is now successfully pulled and ready for use.
