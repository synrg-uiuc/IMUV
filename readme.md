# IMUV Dataset

IMUV project aims to decode speech signal from earphone IMUs, which has the advantage of being insensitive to environmental noise.


<br />

IMUV dataset composes of speech data recorded using (1) IMU placed near the ear, (2) IMU placed near the neck, (3) contact microphone placed near the neck, and (4) normal microphone.

<br />
We recruited four volunteers, and each volunteer is asked to speak (1) a list of 39 normal words, (2) a list of voice assistant wake words (Alexa, Google, Siri, Bixby)


## Directory Structure
    .
    ├── Volunteer1                         
      ├── general_aud.mat               # data collected when users speak normal words
      ├── wake_aud.mat                  # data collected when users speak wake words, 
    ├── Volunteer2                   
      ├── general_aud.mat     
      ├── wake_aud.mat
    ├── Volunteer3                   
      ├── general_aud.mat     
      ├── wake_aud.mat
    ├── Volunteer4                   
      ├── general_aud.mat     
      ├── wake_aud.mat
   
## Mat file Structure
Each row is a one-second speech/IMU clip<br />
col. 1: clean mic data (44.1kHz)<br />
col. 2: contact mic data (44.1kHz)<br />
col. 3: IMU data near the ear (~475Hz, microsecond timestamp in first column)<br />
col. 4: IMU data near the neck(~475Hz, microsecond timestamp in first column)<br />
col. 5 and 6: unused data at this moment<br />
