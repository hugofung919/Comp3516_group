# Comp3516_group08 Floor Pressure sensing
## Team members:  
Hui Lam, POON, 3035801415, u3580141@connect.hku.hk  
Ho Yin, LAI, 3035801570, hoyinleo@connect.hku.hk  
King Hung, FUNG, 3035695153, hugofung@hku.hk  

# Problem complication:
## Project 
HK is a 3D city. However, it is non-trivial to know which floor one is even with the help of GPS (GPS is relatively poor in determining the altitude compared with longitude and latitude). Modern phones are equipped with various sensors, including barometers that can detect altitude changes at a reasonable accuracy. Can you design a solution for locating which floor a user is (through barometers, perhaps with the help of other available sensors)?

### Indroduction of Indoor positionion

### Limitations of GPS
Global positioning systems (GPS) have become indispensable technology in modern society. GPS is a radio wave receiver used to provide coordinates that give the exact position of an element in a certain space. (https://www.sciencedirect.com/topics/biochemistry-genetics-and-molecular-biology/global-positioning-system) However, it is not suitable for indoor positioning. The radio wave of GPS can be easily blocked by different obstacles such as roofs, walls, etc. No line-of-sight to the satellite

## Workflow:  
### 1) Data Collection & data set  
- Collect Barometer data from the "phyphox" app.
- 

# Technical solution
## 2) Data coll








Data Collection: 

Data Pre-processing: Eliminate any outliers or erroneous data points from the collected
barometer data.

Altitude Calculation: Use the collected barometer data to compute the altitude of the user's
current location.

Floor Level Estimation: Define a range of altitudes for each floor of a building and assign a
floor number to the altitude range.. Estimate the user's floor level by determining which
altitude range the calculated altitude falls within.
Longitude and latitude calculation: Install multiple wireless access points as references
points located at different spots of the building. Use the collected Wi-Fi signal data to
compute the estimated location of the user by measuring the signal strength of the nearest
eight access point.

Validation and Refinement: Validate the estimation algorithm by comparing it with actual
location using floor maps or other sources. Refine the algorithm based on the validation
results. This can involve adjusting the altitude ranges for each floor, using additional sensors
to improve accuracy, or implementing machine learning techniques to optimize the
algorithm.
