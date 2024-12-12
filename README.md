# MilkDropLM Lite

*Notebook Version: 1.1b - Gradio added*

## Purpose
This repo contains notebooks to run [MilkDropLM](https://huggingface.co/InferenceIllusionist/MilkDropLM-7b-v0.3) on a Google Colab instance, by using the GPUs available on the cloud.
This will allow you to create MilkDrop presets inside colab, with an intuitive Gradio interface. Just like with the original model, you will get output text that can then be copied and pasted into a `.milk` file

## Usage
1) Copy the notebook in this repo to your personal Google Colab
2) Make sure that you have selected a GPU runtime from the GPU options. Hit `Runtime -> Change Runtime -> T4 GPU` from the top colab menu While CPU inference is technically possible, the exeuction times are far longer. For now, only GPU accelerated inferencing is supported

![image](https://github.com/user-attachments/assets/81825ff9-836c-4a9b-bda4-c62a5e7236ae)

![image](https://github.com/user-attachments/assets/72ed01eb-7a07-43d6-a26c-e403f084bdd6)

3) Again from the Runtime menu, hit `Run All` and the required packages will be installed
4) The code will execute. At the very bottom of the colab window you will see a Gradio UI that you can use to generate. A temporary link is also created which will enable you to access the Gradio link from anywhere for up to 72 hours.
5) Please bear in mind that generation will be slower than local inferencing. If you do have a GPU in your local machine, even 8GB VRAM would be enough for the [GGUF version of this model](https://huggingface.co/Quant-Cartel/MilkDropLM-7b-v0.3-GGUF)

## Acknowledgements
* Thank you to Gradio for providing the front-end UI capabilities for this experience
* Gratitude for Google for providing the compute for this to enable folks to be able to try LLMs without the hardware requirements too
