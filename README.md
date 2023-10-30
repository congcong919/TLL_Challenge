# TLL_Challenge<br>

***Dataset***<br>
The dataset provided is a subset of the Totally-Looks-Like (TLL) dataset. Each image pair has been
split into a “left” and “right” image, and the dataset has been further split into 2000 training pairs and
2000 test pairs. The ground truth matches for the training set are provided in the file train.csv. <br><br>
In the test set, each “left” image is paired with 20 possible “right” images. The set of candidates includes the ground truth “right” image for this “left” image and 19 foils which have been chosen
at random from the test set. Your algorithm should evaluate each of these 20 possible matches and
attempt to predict which one is the true “right” image for the given “left” image. The candidates are
given in the file test candidates.csv. <br><br>

***Taining hint***<br>
In this project, use pre-trained model for feature extraction, and construct Siamese Neural Network based on existing CNN.<br> 
Instead, you can train your own model, by setting up a similar task using the training dataset: for each training
“left” image you could select a set of 20 candidates which includes the ground truth “right” image
and 19 random foils. However, this is not the only way to train your model. You could instead train
your model to select the correct “right” image from the entire training dataset (though this is likely
to be a more difficult task, and slower, than choosing from only 20 candidates). Or you could select
foils non-randomly; for example, intentionally including “difficult” foils that your model is likely to
mistake for the ground truth match, to force it to learn a better representation.<br><br>

The images were scraped from the website and automatically resized/cropped to 200 × 245 pixels;
some images may have borders, overlaid text, or other artefacts. Images are not guaranteed to be
unique – a “left” image could appear multiple times in the dataset with different “right” matches, or
vice versa. Because the images were collected from the internet, they may contain inappropriate or
offensive content.<br><br>


Dataset link: https://drive.google.com/drive/folders/1ltlWnv5GAa8Ms-cEjOMJwwJBKs7-npJN?usp=drive_link 

