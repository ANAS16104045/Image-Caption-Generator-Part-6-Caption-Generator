# Image-Caption-Generator-Part-6-Caption-Generator

 let’s generate a description for a new photograph.
 
 We will generate a description for it using our model.

Download the photograph and save it to your local directory with the filename “example.jpg“.

First, we must load the Tokenizer from tokenizer.pkl and define the maximum length of the sequence to generate, needed for padding inputs.

Next, we must load the photo we which to describe and extract the features.

We could do this by re-defining the model and adding the VGG-16 model to it, or we can use the VGG model to predict the features and use them as inputs to our existing model. We will do the latter and use a modified version of the extract_features() function used during data preparation, but adapted to work on a single photo.

We can then generate a description using the generate_desc() function defined when evaluating the model.

