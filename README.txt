SETUP:

Anomalib can be found on github.com/openvinotoolkit/anomalib and installed using the description provided.

The config-files need to be copied into the folders of the models, e.g. anomalib/models/padim/
Unfortunately, the references are absolute and need to be changed to the image-folder before use.

The ProjectSeminar.zip contains the images and folder structure that is needed.
This is our final progress and also includes some colored images that did not deliver any meaningful results. 
The folder can directly be added to the datasets folder, it also contains the augmented images.

For the input data without augmentation see the two .zip-files in the Pictures folder on the Sharepoint.
Photos.zip contains our sample images that we took of the provided samples.
Input_Data.zip contains the images cut to 1024x1024 pixels and the folder structure needed for training.


TRAINING:

To train a model use this command:
python tools/train.py --config anomalib/models/padim/config.yaml

Make sure to reference the right config-file as an alternative is to use the files in the config folder using a different command.

The results can be found in the results folder with the standard settings.