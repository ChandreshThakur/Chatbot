# Chatbot for IIT Bombay Information

This repository provides a complete guide on implementing a chatbot that has been trained to provide information related to IIT Bombay, covering three key domains: **Courses**, **Faculty**, and **Events**.

### Features:
- Natural Language Processing (NLP) and Natural Language Understanding (NLU) powered chatbot
- Provides relevant information about courses, faculty, and events at IIT Bombay
- Built using the Rasa Framework with custom actions and domain configuration

---

## Setup and Installation

### Prerequisites:
- Install **Anaconda** (Ensure you check the option to add Conda to your system PATH during installation).
- Download and set up the required dependencies as outlined below.

### Step-by-Step Instructions:

1. **Create Project Folder**:
   - Create a new folder named `chatbot`.
   - Open a command prompt inside the `chatbot` folder.

2. **Create and Activate Conda Environment**:
   Run the following commands in sequence to set up the necessary environment:
   ```bash
   conda create --name rasa python==3.8
   conda activate rasa
   ```

3. **Install TensorFlow**:
   TensorFlow is required for model training and optimization:
   ```bash
   conda install tensorflow
   pip install --upgrade tensorflow
   ```

4. **Install Rasa Framework**:
   Use `pip` to install Rasa, the main framework used for chatbot development:
   ```bash
   pip install rasa
   ```
   During installation, you may be prompted to specify a directory. **Ensure you provide the path to your `chatbot` folder** to correctly set up the working directory.

5. **Download and Organize Files**:
   - Navigate to the `chatbot` folder and create a subdirectory named `botdata`.
   - Download all the files from this repository and paste them into the `botdata` folder.
   - **Important:** When pasting, ensure you **replace any existing files or folders** rather than copying them separately.

6. **Train the Model**:
   To train the chatbot model, run the following command in the command prompt (ensure you are inside the `chatbot` folder):
   ```bash
   rasa train
   ```

7. **Run Custom Actions**:
   Open a new command prompt tab, activate the Rasa environment, and run the custom actions server:
   ```bash
   conda activate rasa
   rasa run actions
   ```

8. **Interact with the Chatbot**:
   In the original command prompt tab (where you trained the model), you can now interact with the chatbot by typing:
   ```bash
   rasa shell
   ```

---

## Additional Training and Debugging

If you'd like to further train or fine-tune the chatbot's performance interactively, Rasa offers an interactive training mode. Simply run:
```bash
rasa interactive
```
This command allows you to test and correct the bot's predictions and behavior on the fly, ensuring optimal performance and accuracy.

---

### Notes:
- Make sure to replace any old files with the ones provided in this repository when setting up your environment.
- The `rasa train` command will create the necessary model files for your chatbot to operate.


