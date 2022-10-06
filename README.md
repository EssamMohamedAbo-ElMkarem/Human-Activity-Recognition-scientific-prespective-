# Human Activity Recognition

Human activity recognition, or HAR for short, is a broad field of study concerned with identifying the specific movement or action of a person based on sensor data. 

Movements are often typical activities performed indoors, such as walking, talking, standing, and sitting. They may also be more focused activities such as those types of activities performed in a kitchen or on a factory floor.

The sensor data may be remotely recorded, such as video, radar, or other wireless methods. Alternately, data may be recorded directly on the subject such as by carrying custom hardware or smart phones that have accelerometers and gyroscopes.

<img src= https://repository-images.githubusercontent.com/284708744/60f0a800-ec73-11ea-9c98-1061b5545d29 width=600 align='center'/>

## Word about used sensors

* <b>Accelerometers</b>  is a device that measures the vibration, or acceleration of motion of a structure. The force caused by vibration or a change in motion (acceleration) causes the mass to "squeeze" the piezoelectric material which produces an electrical charge that is proportional to the force exerted upon it. Since the charge is proportional to the force, and the mass is a constant, then the charge is also proportional to the acceleration. These sensors are used in a variety of ways from space stations to handheld devices, and there's a good chance you already own a device with an accelerometer in it. For example, almost all smartphones today house an accelerometer. They help the phone know whether it undergoes acceleration in any direction, and it’s the reason why your phone’s display switches on when you flip it. In an industry setting, accelerometers help engineers understand a machine's stability and enable them to monitor for any unwanted forces/vibrations. 

* <b>Gyroscope</b> is a device containing a rapidly spinning wheel or circulating beam of light that is used to detect the deviation of an object from its desired orientation. Gyroscopes are used in compasses and automatic pilots on ships and aircraft, in the steering mechanisms of torpedoes, and in the inertial guidance systems installed in space launch vehicles, ballistic missiles, and orbiting satellites. Gyroscopes can be very perplexing objects because they move in peculiar ways and even seem to defy gravity. These special properties make ­gyroscopes extremely important in everything from your bicycle to the advanced navigation system on the space shuttle. A typical airplane uses about a dozen gyroscopes in everything from its compass to its autopilot. The Russian Mir space station used 11 gyroscopes to keep its orientation to the sun, and the Hubble Space Telescope has a batch of navigational gyros as well. Gyroscopic effects are also central to things like yo-yos and Frisbees!

# Word about the dataset

The Human Activity Recognition database was built from the recordings of 30 study participants performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors. The objective is to classify activities into one of the six activities performed.

<img src = https://storage.googleapis.com/kaggle-datasets-images/226/478/11ff0be5a773e73886c3da626349e8f0/dataset-cover.jpeg width=600/>

<a href='https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones?select=train.csv'> Link to Dataset <a/>

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKINGUPSTAIRS, WALKINGDOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.



---


## Attribute Information:

For each record in the dataset it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope.
- A 561-feature vector with time and frequency domain variables.
- Its activity label.
- An identifier of the subject who carried out the experiment.


### The set of variables that were estimated from these signals are: 

* mean(): Mean value
* std(): Standard deviation
* mad(): Median absolute deviation 
* max(): Largest value in array
* min(): Smallest value in array
* sma(): Signal magnitude area
* energy(): Energy measure. Sum of the squares divided by the number of values. 
* iqr(): Interquartile range 
* entropy(): Signal entropy
* arCoeff(): Autorregresion coefficients with Burg order equal to 4
* correlation(): correlation coefficient between two signals
* maxInds(): index of the frequency component with largest magnitude
* meanFreq(): Weighted average of the frequency components to obtain a mean frequency
* skewness(): skewness of the frequency domain signal 
* kurtosis(): kurtosis of the frequency domain signal 
* bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
* angle(): Angle between to vectors.

## The data set is balanced as the plot indicates

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/2.png />

## Distribution of stationary and moving activities

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/1.png />

## T-SNE visualization of dataset

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/3.png  />


## Models fighting

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/4.png />

## The model used as a benchmark for dataset versions (SVC Linear)

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/6.png  />

## Different dataset versions performance

<img src=https://github.com/EssamMohamedAbo-ElMkarem/Human-Activity-Recognition-scientific-prespective-/blob/main/imgs/5.png />
