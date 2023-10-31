# R scripts for forecasting in Learning Dashboard

R script files including a set of forecasting methods. These scripts act as wrappers of some state of the art forecasting methods, implemented in packages like the well-known **forecast**. Apart from that, they also implement some other useful aspects, like wrapping the **mongolite** package to allow easy metrics, factors, and strategic indicators gathering from a MongoDB database. The scripts also implement saving and reusing the fitted forecasting models, in order to save time and computation resources.

The scripts are intended to be used along with the [LD-forecast](https://github.com/Learning-Dashboard/LD-forecast) library, but are prepared to be used alone as well.


# Available forecasting methods

The available methods and the corresponding R package implementing them are as follow:

| Method Name | R Package |
| -------------------- | --------------------------------|
| Arima | forecast |
| Arima (force seasonality) | forecast |
| Theta | forecast, forecastHybrid |
| ETS | forecast |
| ETS (force damped) | forecast |
| Bagged ETS | forecast |
| STL | forecast |
| Neural Network (nnetar)| forecast |
| Hybrid | forecastHybrid |
| Prophet | prohpet |


## Dependencies

The scripts depend on the following packages:

 - forecast
 - devtools
 - mongolite
 - forecastHybrid
 - prophet

These required packages should be installed beforehand using the following commands:

     install.packages("devtools")
     library(devtools)
     install_version("forecast", version="8.21")
     install_version("prophet", version="1.0")
     install_version("Rserve", version="1.8-11")
     install_version("mongolite", version="2.7.2")
     install_version("forecastHybrid", version="5.0.19")
     install_version("curl", version="5.0.0")
    
## Licensing
Software licensed under GNU Lesser General Public License v3.0. Permissions of this copyleft license are conditioned on making available complete source code of licensed works and modifications under the same license or the GNU GPLv3. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. However, a larger work using the licensed work through interfaces provided by the licensed work may be distributed under different terms and without source code for the larger work.
    
