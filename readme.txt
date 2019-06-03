1.wsta-project.ipynb
(1)Do the job of indexing of wiki-pages-text files and searching for wiki docs and sentences for model to use as refined input data;
(2)Deal with the selected (wiki name,sentence id, sentence content) in (1) and format it into what the first BERT model needs, and feed it to BERT which is used in colab notebook(wsta-train-model.ipynb).
(3)Mark evidence sentence for test, and deal with the output from colab notebook and format it into what the second BERT needs, and feed it to BERT.
(4)Mark all labels of test set, and get the output file "testoutput.json".
(5)P.S.1 The parts of code with explicit markdown are the alternative method using dev dataset as test for final result.
(6)P.S.2 All output and input files for this file should be under the same directory of wsta-project.ipynb. Those output files from wsta-train-model.ipynb which are not from local should be downloaded to this directory.

2.wsta-train-model.ipynb(using TPU hence containing some Colab code)
This notebook trains with BERT model with our data, makes a prediction and classification using TPU, hence should be run on Colab. You may see some processed data in this notebook is directly downloaded from Google Drive, it is because Colab cannot directly get local file. The input data sets are all the same as the output from the wsta-project.ipynb, and should be under the same directory of wsta-project.ipynb and the file names should be the same. The output data of Colab are stored in Google Cloud Storage.
