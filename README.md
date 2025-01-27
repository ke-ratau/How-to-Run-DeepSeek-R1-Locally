# How-to-Run-DeepSeek-R1-Locally
1. Using LM Studio
Download and install LM Studio : Just go to the LM Studio website and download the version for your system.

Download the DeepSeek R1 model : In LM Studio, go to the Discover tab, search for "DeepSeek R1," and select the version most compatible with your system. If you're using a MacBook with Apple processors, keep the MLX option selected next to the search bar (these versions are optimized for Apple hardware). For Windows or Linux, choose the GGUF option.

Load the model : After downloading, go to Local Models , select DeepSeek R1, and click Load .

Start the local server : In the Developer tab, enable Start Server . It will start running the model at http://localhost:1234.

Proceed to step 4 Integrating with VSCode !

2. Using Ollama
Install Ollama : Download it from the Ollama website and install it.
Download the model : In the terminal, run*:
   ollama pull deepseek-r1  
*This is the main model; if you want smaller models, go to https://ollama.com/library/deepseek-r1 and see which command to run in the terminal.

Start the server : In the terminal, run:
   ollama serve  
The command will start running the model at http://localhost:11434.

Proceed to step 4 Integrating with VSCode !
3. Using Jan
Download and install Jan : Choose the version for your system on the Jan website.

Download the model : I couldn't find DeepSeek R1 directly in Jan. So, I went to the Hugging Face website and manually searched for "unsloth gguf deepseek r1." I found the desired version, clicked the "Use this model" button, and selected Jan as the option. The model automatically opened in Jan, and I then downloaded it.

Load the model : After downloading, select the model and click Load .

Start the server : Jan automatically starts the server, usually at http://localhost:1337.

Proceed to step 4 Integrating with VSCode !

4. Integrating with VSCode
Install the extension : In VSCode, open the Extensions tab and install Cline or Roo Code.
Configure the extension for Jan or LM Studio : The configuration for both Cline and Roo Code is practically identical. Follow the steps below:

Click on the extension and access "Settings" .
In API Provider , select "LM Studio" .
In the Base URL field, enter the URL configured in Jan or LM Studio.
The Model ID field will be automatically filled if you only have one model available. Otherwise, manually select the DeepSeek model you downloaded.
Finish by clicking "Done" .
Configure the extension for Ollama :

Click on the extension and access "Settings" .
In API Provider , select "Ollama" .
In the Base URL field, enter the URL configured in Ollama.
The Model ID field will be automatically filled if you only have one model available. Otherwise, manually select the DeepSeek model you downloaded.
Finish by clicking "Done" .
Integration complete, now just enjoy the functionalities of Cline or Roo Code.

Conclusion
DeepSeek R1 is a lifesaver for those who want a powerful AI without spending anything. With LM Studio , Ollama , or Jan , you can run it locally and integrate it directly into Visual Studio Code . Choose the model that fits your PC and start using it today!
