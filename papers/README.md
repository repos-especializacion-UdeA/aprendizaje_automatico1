# Apuntes papers

## Articulos

## A quantitative taxonomy of human hand grasps

* **Link**: https://pmc.ncbi.nlm.nih.gov/articles/PMC6377750/

* **Palabras clave**: Hierarchical trees, Electromyography, Kinematics, Hand Grasps Taxonomy, Hand Movements, Robotics


The taxonomy is based on electromyography and kinematic data recorded from 40 healthy subjects performing 20 unique hand grasps. F

hierarchical trees are computed for several signal features

The general taxonomy merges the kinematic and muscular description into a comprehensive hierarchical structure. According to the results, hand movements can be divided into five movement categories defined based on the overall grasp shape, finger positioning and muscular activation

GRASP taxonomy: This taxonomy is organized in a matrix, with the grasps divided into several
columns and in two rows according to four main parameters including power type, opposition type, position of
the thumb and virtual finger assignments


A quantitative taxonomy of hand movements can therefore reduce ambiguity in the field, but it requires the
measurement of specific biomedical data. Several parameters can be used to quantitatively characterize hand
grasps, such as posture, muscular activity and force. 

Kinematic data are usually measured with two main techniques: visual or wearable systems. Visual systems can
be affected by visual occlusion in the recording of hand
grasps and the procedure to place the visual markers can
be time consuming. Data gloves are a common alternative that is sufficiently precise [21] and extremely easy
to record. Thus, they are suitable for studies involving
many subjects. The joint angles were previously used
as features in order to compare model estimations with
real position measurements [22, 23]


In the comparison of movements, synthesis functions are often applied
to represent the entire motion with fewer data. For
instance, Finger Aperture Indexes (FAIs) were used to
represent long finger opening starting from joint angles
collected by a Motion Capture (MoCap) system composed of nine infrared cameras and 17 retro-reflective
hemispheric markers

Muscular data can be measured with Surface Electromyography (sEMG). The sEMG signal can be modeled
as a superimposition of the Motor Unit Action Potentials (MUAPs) of the active Motor Units (MUs)

This paper presents the first quantitative taxonomy
of hand movements. The relative variations between
joint bending angles (measured with a data glove) allow
a quantitative characterization of the hand movement
kinematics. 

We analyze the movements performed by
40 intact subjects to extract the common underlying patterns that characterize each grasp. We create hierarchical
trees for each subject individually and subsequently merge
them into supertrees to obtain a generalized taxonomy.

The data analysis procedure can be summarized:
* Data acquisition:
  * second Ninapro dataset (DB2) (https://www.nature.com/articles/sdata201453)
  * Acquisition setup:
    * Hand kinematics were measured using a 22-sensor CyberGlove II: providing data proportional to joint angles, sampled at slightly less than 25 Hz 
    * Delsys Trigno Wireless system: Muscular activity --> The sEMG electrodes are double-differential and measure the myoelectric signals at 2 kHz with a baseline noise of less than 750 nV RMS.
  * Each subject performed 6 repetitions of 49 movements plus rest. Each movement repetition lasted 5 s, alternated with 3 s of rest. 
* signal feature extraction: pre-processing and feature extraction
  * EMG data preprocessing: 
    1. Filtering and synchronization (Que es esto ultimo?):
       *  Filtering: Hampel filter at 50 Hz.
       *  Synchronization: all the modalities were up-sampled at the sampling frequency of the fastest device (2 kHz) using linear-interpolation.
    3. Extracting a set of signal features using a moving window technique. 
       *  Signal feature extraction was performed applying the method described by Englehart:
          *  Each movement repetition was windowed using a 200 ms window, with 100 ms of overlap
          *  In order to make the taxonomy robust to differences between features.
             *  Five time domain signal features:
                *  Root Mean Square (RMS)
                *  Mean Absolute Value (MAV)
                *  Integrated Absolute Value (IAV)
                *  Time Domain Statistics (TD) [44] and 
                *  Waveform Length (WL) [43, 47–52]. 
              * The Time Domain Statistics (TD): 
                *  Mean Absolute Value (MAV)
                *  Mean Absolute Value Slope (MAVS)
                *  Zero Crossings (ZC)
                *  Slope Sign Changes (SSC)
                *  Waveform Length (WL)
    4. The signal features were used as input data to compute the hand movement taxonomies.
  * CyberGlove data: window based time series analysis and in particular from the literature in EMG data analysis.
  
* creation of the hierarchical trees
* fusion of the trees into super-trees (“Computation of the muscular, kinematic and general quantitative taxonomies: hierarchical super-trees” subsection), 




### Vocabulario

* human grasping = agarrar con la mano
* Taxonomies of hand grasps = Taxonomias de hagarres de manos.





## Otros

* https://www.nature.com/articles/sdata2018101
* https://www.cs.cmu.edu/~ynakamur/papers/TaxonomyEverydayGrasps.pdf
* https://www.csc.kth.se/grasp/taxonomyGRASP.pdf
* 