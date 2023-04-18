# VHTO Girls Day Workshop at LVNL
This repository contains all the material that is needed to repeat the workshop given to a Dutch High School class for the VHTO Girls Day (https://www.vhto.nl/aanbod/girls-day/) at Luchtverkeersleiding Nederland. In this workshop, students were tasked with designing an air route over the Netherlands minimising both the length of this route and the noise disturbance that it would cost. This workshop was chosen as a good way to illustrate technical concepts such as a trade-off without overwhelming the students with math (which is all in this package).

## Preparatory steps
First, make sure [the requirements](requirements.txt) are fulfilled. Next, a dataframe from the CBS must be downloaded and a parameter of this needs to be chosen [as laid out](1%20-%20Source%20Data%20and%20Processing/Convert_Source_File.ipynb). This will result in a Shapefile that can be loaded into QGIS with a value per each block that the file is made up of. Extra maps [can be created as needed](2%20-%20Extra%20Maps/Convert_Extra_Maps.ipynb). In this repository a way of creating extra maps for the defined start and end points of the air route is defined, as well as a way of turning the Schiphol TMA into a polygon that can be used in QGIS as well. These maps can all be loaded into QGIS and turned into printable PDFs as needed for the workshop. Example prints are included [as well](3%20-%20GIS%20and%20Printing%20Map/girlsday_A2_ingezoomd.pdf).

## Running the workshop
For the workshop, the students were divided in groups of 5. After designing a route, the points indicated on the print were looked up in QGIS and the coordinates were entered into [the evaluation script](4%20-%20Running%20the%20Workshop\Design%20evaluator.ipynb). After running the 3 cells that analyzed a design the scores were returned to them, and they got the chance to design another route.

Scoring was performed based on a normalization of the distance and noise score, but any combination worked. It was also seen that, at least with this set-up, the distance flown did not have a big impact on the outcome, so a minimisation for pure noise may also be a good metric on its own.

## Author
[![Linkedin](https://img.shields.io/badge/Linkedin-0072b1?logo=linkedin&logoColor=white&style=for-the-badge)](https://www.linkedin.com/in/jnp-post/)