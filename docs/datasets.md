# Datasets

## Listado de datasets disponibles en Librerías de Python

A continuación te presento un listado de los principales datasets incluidos o fácilmente accesibles desde librerías de Python utilizadas en Data Science. Se incluye el enlace a la documentación oficial donde pueden consultarse todos los datasets disponibles.

| Librería	| Función para acceder	| Algunos datasets disponibles	| Documentación oficial|
| --- | ---| ---| ---| 
| scikit-learn| 	sklearn.datasets	| iris, wine, diabetes, breast_cancer, digits, linnerud, california_housing, olivetti_faces, covtype, kddcup99, 20newsgroups, openml| 	https://scikit-learn.org/stable/datasets.html| 
| seaborn| 	sns.load_dataset()	| anscombe, attention, brain_networks, car_crashes, diamonds, dots, exercise, flights, fmri, geyser, iris, mpg, penguins, planets, seaice, taxis, tips, titanic| 	https://github.com/mwaskom/seaborn-data
| Plotly Express| 	plotly.express.data| 	iris, tips, gapminder, medals_long, medals_wide, stocks, elections, experiment, carshare, wind, election_geojson| 	https://plotly.com/python-api-reference/generated/plotly.express.data.html| 
| Statsmodels| 	statsmodels.datasets| 	macrodata, co2, longley, sunspots, nile, heart, modechoice, spector, randhie, grunfeld, elnino| 	https://www.statsmodels.org/stable/datasets/index.html| 
| SciPy	| scipy.datasets| 	ascent, face, electrocardiogram	| https://docs.scipy.org/doc/scipy/reference/datasets.html| 
| TensorFlow Datasets| 	tensorflow_datasets	| Más de 1.000 datasets (MNIST, CIFAR-10, IMDB Reviews, Fashion-MNIST, Oxford Flowers, etc.)| 	https://www.tensorflow.org/datasets| 
| TorchVision| 	torchvision.datasets	| MNIST, FashionMNIST, CIFAR10, CIFAR100, ImageNet, STL10, CelebA, EMNIST, KMNIST, VOCDetection| 	https://pytorch.org/vision/stable/datasets.html| 
| OpenML| 	fetch_openml() (scikit-learn)	| Miles de datasets de Machine Learning (Titanic, Adult, Boston, etc.)| 	https://www.openml.org| 
| Hugging Face|  Datasets	datasets.load_dataset()	| Más de 200.000 datasets para NLP, visión e IA generativa| 	https://huggingface.co/datasets| 
| Bokeh|  Sample Data	bokeh.sampledata	| autompg, iris, unemployment, us_states, stocks, airports, world_cities| 	https://docs.bokeh.org/en/latest/docs/reference/sampledata.html| 
| Altair / Vega Datasets| 	vega_datasets| 	cars, iris, wheat, stocks, flights, barley, seattle_weather| 	https://github.com/vega/vega-datasets| 
| GeoPandas| 	geopandas.datasets (algunas versiones antiguas)	| naturalearth_lowres, naturalearth_cities, nybb| 	https://geopandas.org| 

## Ejemplos de uso

Datasets más utilizados en cursos de Data Science

### scikit-learn
```jupyter
from sklearn.datasets import load_iris

iris = load_iris(as_frame=True)
iris.frame.head()
```
Los más utilizados son:
* Iris
* Wine
* Breast Cancer Wisconsin
* Diabetes
* Digits
* California Housing
* Olivetti Faces


### seaborn
```jupyter
import seaborn as sns

sns.get_dataset_names()
```
Algunos de los más utilizados:
* Diamonds
* Flights
* Car Crashes
* Planets
* Taxis
* Tips
* Titanic
* iris
* titanic
* penguins
* mpg


### Plotly Express
```jupyter
import plotly.express as px

px.data.iris()
px.data.tips()
px.data.gapminder()
px.data.stocks()
```

### Statsmodels
```jupyter
import statsmodels.api as sm

sm.datasets.macrodata.load_pandas().data.head()
```

### SciPy
```jupyter
from scipy import datasets

ecg = datasets.electrocardiogram()
```
