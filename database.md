# The data

Luckily enough, there is an [amazing website](https://opendata.paris.fr/ "Paris | Data") in which are stored all kinds of data regarding the city of Paris. For my project, I will mainly use two datasets:

## 1. [Arrondissement dataset](https://opendata.paris.fr/explore/dataset/arrondissements/table/)
In this dataset are stored the coordinates of the 20 parisien *arrondissements*, which will be the first step to filter our search domain.
Each of the 20 entries is provided, among other things, with its coordinates, shape, extension, official name and postal code.
Of these information, the main ones to be used are the coordinates and the geometrical shapes, in order to produce a map that points out the different arrondissements.

## 2. [Administrative quarters](https://opendata.paris.fr/explore/dataset/quartier_paris/table/)
Each *arrondissement* is composed of several administrative quarters; in this second dataset we will exploit their coordinates and geometry to add details to our search.
The format is similar to the previous table, with the addition of the arrondissement to which the neighbor belongs to.

## 3. [Four Square API](https://developer.foursquare.com/)
FourSquare data will be our main filter to determine which zones are in line with our needs. We will use it to retrieve interesting venues around the potential neighborhoods that we will find! 
