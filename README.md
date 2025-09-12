# ELM-Binary-Classifier

Is is a feed-forward neural network known as Extreme Learning Machine (ELM) Binary classifier, adtaped for use from GitHub [popcornell, 2018](https://github.com/popcornell/tfelm/blob/pop_new/ELM_class_example.ipynb)

The main changes found are: 

- Importing Dataset from locally saved storage form an external source.
- Adding the epoch count to watch the progress of the training
- Adding a system to allow users to directly upload an image to test it on the trained model. 
- Added [Huuging Face's Gradio](https://huggingface.co/gradio) to allow the use of comparision is a web UI, providing the Colab session is active! 

To try yourself simply start a new project in Google Colab and add the selected blocks of code in order of: 

- ELM-Main
- Image-Prediction
- Gradio-UI

Datasets that are downloaded go into Colab's "Content" folder, however, It should also be worth noting (if you’re new to TensorFlow/Colab) that datasets don’t store permanently, you’ll find after an extended period of time or new day you’ll have to re-upload the dataset and re-train the model before being able to use it again. They can also be called in locally from a google-drive if you link it. One of the main datasets I used was [CIFAKE from Kaggle](https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images), as well as a handful of others.

Gradio's UI will run, so long as the session is active in Colab, unless externally hosted elsewhere. When the session ends the web UI will time out. 

Colab's inbuilt AI was used to help troubleshoot errors (I'm no expert)

Feel free to use how wanted, the licene is under MIT for any personal use, so long as I (LordChristoff, 2024) and (Popcornell, 2018) are credited either in the code or project description. 

Or find a breif post about it on [medium.com](https://lordchristoff.medium.com/elm-image-classifier-using-tensorflow-f92564bc5efd)

## Background

In the intrests of cyber forensics and transparency this project was undertaken at Univreisty to determine if the use of Exreme Learning Machine, that provides an unbiased approach to its learning, with its hidden layers. Can provide a solution to determining what is and what isn't fake from online sources. Although the model did work in some cases, it also failed in others. A lot of this was arrtibuted to the ever evolving landscape and sophistication of the data it was trying to determine was real or fake against the dated datasets that were being used. Overfitting and lack of backpropogation was also deemed to not aid the process. 

However, further avenues of research into this method such as QELM or QGANs was determined to be the next step in such research. 

----

Project was done merely for academic purposes and no finanical gain was made from it. 

The project has now been adapted/added to Huggingface spaces https://huggingface.co/spaces/SirChristoff/ELM-Binary-Classifier
