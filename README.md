# HealthCare: COVID19 Detection From X-Ray Images
Automatic detection of COVID-19 from X-ray images of lungs using Keras and Tensorflow in Deep Learning.

## Directory Structure

<pre>
.
├── Dataset_Collection.ipynb
├── Evaluate_COVID19.ipynb
├── README.md
├── architecture.json
├── dataset
│   ├── covid
│   │   ├── 01E392EE-69F9-4E33-BFCE-E5C968654078.jpeg
│   │   ├── 03BF7561-A9BA-4C3C-B8A0-D3E585F73F3C.jpeg
│   │   ├── 1-s2.0-S0140673620303706-fx1_lrg.jpg
│   │   ├── 1-s2.0-S0929664620300449-gr2_lrg-a.jpg
...     ...
│   │   ├── ryct.2020200034.fig2.jpeg
│   │   ├── ryct.2020200034.fig5-day0.jpeg
│   │   ├── ryct.2020200034.fig5-day4.jpeg
│   │   └── ryct.2020200034.fig5-day7.jpeg
│   └── normal
│       ├── IM-0028-0001.jpeg
│       ├── IM-0033-0001-0001.jpeg
│       ├── IM-0240-0001.jpeg
│       ├── IM-0450-0001.jpeg
...     ...
│       ├── person925_virus_1582.jpeg
│       ├── person934_virus_1595.jpeg
│       ├── person939_bacteria_2864.jpeg
│       └── person989_virus_1667.jpeg
├── history.pkl
├── metadata.csv
├── model_plot.png
└── train_COVID19.ipynb
</pre>

## File Details

### [Dataset_Collection.ipynb](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/Dataset_Collection.ipynb)

Jupyter notebook for collecting training and testing dataset of lung images. Uses publicly available data for storing  **COVID-19**
positive and negative images.

### [Evaluate_COVID19.ipynb](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/Evaluate_COVID19.ipynb)

Notebook for evaluating trained model on test images and measure different parameters of usefulness. Uses architecture.json and weights.h5 files which are given as output from training the model.

### [architecture.json](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/architecture.json)

JSON file which stores complete architecture of trained detection model.

### [dataset](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/tree/master/dataset)

Dataset folder consists of normal and covid images which are used for training the model. There are 70 normal and 70 COVID19 positive lung images collected from publicly available data sources.

### [history.pkl](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/history.pkl)

Pickle file for storing different parameters related to history of model training process, like 'loss', 'accuracy', etc.

### [metadata.csv](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/metadata.csv)

CSV file which has metadata related to publicly available dataset for COVID-19 lung X-Ray images. Used during dataset collection and preparation.

### [model_plot.png](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/model_plot.png)

Layer-wise detailed model image which was used for training and testing.

### [train_COVID19.ipynb](https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/train_COVID19.ipynb)

Jupyter notebook containing code for training detection model which uses Keras and Tensorflow for training and validation.

## Results

<img src="https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/result-graph.png">

### Classification Report

<img src="https://github.com/prateekguptaiiitk/HealthCare-COVID19-Detection/blob/master/ConfusionMatrix.png">

<pre>
	Accuracy: 96.43%
	Sensitivity: 1.0000
	Specificity: 0.9286
</pre>

## Usage

Use following command in terminal:
<pre>
 $python usage.py --image /Path/To/Image/
</pre>

## Author

<table>
<tr>
<td>
     
     Prateek Gupta

<p align="center">
<a href = "https://github.com/prateekguptaiiitk"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
</p>
</td>
<td>
     
     Gourav Sharma

<p align="center">
<a href = "https://github.com/gourav2698"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
</p>
</td>
</tr> 
  </table>
