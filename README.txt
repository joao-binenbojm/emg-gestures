This repository is used to investigate various classical EMG gesture classification approaches on the EMG Gestures dataset available from the UCI repository. I've primarily focused on using simple window-based classification approaches with time-domain features from the work of Englehart and Hudgins (2003), including a PCA/LDA analysis and LDA-based classification. When training on a single subject and single trial, the performance on the same's subject second trial was poor (~30-40% accuracy). When training classifier on a training set containing data across trials/subjects, as well as when training on a subset of subjects (and testing on held-out subjects), performance was reasonable given task complexity (~65-75% accuracy). All in all, it would've been good to investigate the effects of inter-trial variability with more trials of data available.=


Below is information of the README from the original data.



EMG Pattern Database

For recording patterns, we used a MYO Thalmic bracelet worn on a user’s forearm, and a PC with a Bluetooth receiver. The bracelet is equipped with eight sensors equally spaced around the forearm that simultaneously acquire myographic signals. The signals are sent through a Bluetooth interface to a PC. 
We present raw EMG data for 36 subjects while they performed series of static hand gestures.The subject performs two series, each of which consists of six (seven) basic gestures. Each gesture was performed for 3 seconds with a pause of 3 seconds between gestures.


Description of raw_data _*** file
Each file consist of 10 columns:
1) Time - time in ms;
2-9) Channel - eightEMG channels of MYO Thalmic bracelet;
10) Class  –thelabel of gestures: 
0 - unmarked data,
1 - hand at rest, 
2 - hand clenched in a fist, 
3 - wrist flexion,
4 – wrist extension,
5 – radial deviations,
6 - ulnar deviations,
7 - extended palm (the gesture was not performed by all subjects).




Relevant Paper:
Lobov S., Krilova N., Kastalskiy I., Kazantsev V., Makarov V.A. Latent Factors Limiting the Performance of sEMG-Interfaces. Sensors. 2018;18(4):1122. doi: 10.3390/s18041122


Supported by the Ministry of Education and Science of the Russian Federation in the framework of megagrant allocation in accordance with the decree of the government of the Russian Federation №220, project № 14.Y26.31.0022 
