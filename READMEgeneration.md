[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/SyuA65Jv)
## DL module coursework 1



# Build a generative model that creates X-ray images of hands

<img src="https://drive.google.com/uc?id=1LubLuuyiJwyDNRd2Wj0vaA0Ek2AtAFxH" width="500"/>


Relase date: 14:00h Thursday 7th December 2023

Submission deadline: 18:00h Friday 8th December 2023

**At 18:00h on Friday I will clone the repositories, so make sure to have everything commited by then.**

<br>

## **Task**:
Create a generative model, either a VAE or a GANs, train it, and use it to generate 300 new samples (new images) of X-ray images of hands. <br>

Justify your choice (there is a dedicated text cell in the 'clean' notebook. There is no right or wrong here, but the quality of the justification will be assessed.

[**IMPORTANT: Choose a single generative model (VAE or GAN), and submit the generated samples from your model of choice, you won't get any extra marks for implementing one VAE and one GAN.**].

## **Dataset**:
You have 8000 samples available in the repository under the folder `real_hands` that you can use to train your VAE or your GAN.

## **Deliverables**:
1. `VAE_hands` or `GAN_hands` — folder containting the 300 samples generated with your model. The format should be `jpeg`. Save your generated hands in the corresponding folder provided in the repository: `VAE_hands` or `GAN_hands`. Name the samples in the folder as `yourusername_001.jpeg`, `yourusername_002.jpeg`, ..., `yourusername_300.jpeg`. You only have to populate one of the folders (depending on the model you have chosen, VAE or GAN). The sizes of the generated images should be the same as the ones in the training set. <br>
[**If you implement both generative models and populate the two folders, keep in mind that I will only use one of them for the marks.**]. 

2. `yourusername_DLcw1_clean.ipynb` — 'clean' notebook containing the code and supporting explanatory text for:
	- Data preparation
	- Design and implementation of your network of choice (VAE or GAN)
	- Implementation of training loops and any other utility functions you see fit
	- Executed cells for network training with accompanying loss evolution plots (using livelossplot or any other visualisation tool you like). Here use the best hyperparameters you have found. **Important: you will have to train your network from scratch**, so no pre-trained networks allowed (unless you pretrain them yourself and show it in the notebook).
	- Generation of 300 samples by using the trained model (and the code you need to save the generated images in your drive or local machine that you will upload in the repo). The uploading does not need to be automated from the notebook directly, you can save the images any way you want and then put them in the repository by copy-pasting them from your local machine or your Google Drive.


3. `yourusername_DLcw1_hypertune.ipynb` — An 'auxiliary' notebook containting any hyperparameter exploration you have done to decide what are the best hyperparameters to use for your final training. You will include your final training with your choice of hyperparameters in the 'clean' notebook described in point 2.). 

4. `references.md` — List of your references used in the template references.md (see Referencing section below).

[**IMPORTANT: when you save your notebooks, make sure that all the cells are executed so that when you upload the .ipynb file in the repo the outputs of the code cells are visible**].

### Instructions to prepare the deliverables:
- **Use the empty notebook templates provided only**, they contain some structure that you have to follow but are otherwise pretty flexible. If you want to use any other notebooks for testing or validating ideas, do not include them in the repository. You will be assessed on the quality of the generated samples and the two notebooks described above only.
- Please make sure to add **text cells and comments in the code to explain what you are doing and why you are doing it**. Do not write unnecessarily-long paragraphs about every step, but provide a sentence or two to justify your choices and your decision-making process.
- If you want to package some functionalities (that you want to use in the delivered notebooks) in modules, please do so, but create **only one** dedicated folder called `utils` in the repo and put it there.



## Tips and tricks

- You have a day and a half. Organise your time well, and think about all the tasks you will need to do to complete the assessment before starting. Then build a list of tasks, prioritise it and allocate time to each task in the list, including breaks and appropriate time to rest overnight (you can leave your networks training while you sleep, but be careful not to burn all your compute-unit budget!).
- Set up your development environment carefully: do not connect to a GPU that burn credits while you are writing code or doing other tasks that do not require serious compute power (like data preparation).
- Checkpoint your models during training to avoid having to retrain from epoch 0 every time you disconnect your runtime environment.
- Test your submission strategy early, in particular:
	- make sure you can save images generated by your model, and upload them in the repository well before the deadline to avoid unpleasant last minute surprises.
	- make sure that when you download your notebook from Colab (or your local machine) with all the executed cells, these executed cells containing the output you want to have there are visible in the repository. If not, check that you have saved and uploaded the right notebook.

## Referencing
	
This is an open book assessment, you are encouraged to use resources online. Populate the markdown file in the repository called references.md with links to sites you used, papers you have read, links to your chatGPT prompts and answers, and any other resource you used to help you design your generative model.

