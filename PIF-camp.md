# PIFCAMP 2024 : Modulating Time

As part of the annual [PIFcamp festival](https://pif.camp/sl/) in Soča Valley, Slovenia, live-coders [Alex McLean](https://slab.org/) and [Lizzie Wilson](https://lwlsn.github.io/) and designer/educator in the fields of e-Textiles, Interaction Design and Physical Computing [Mika Satomi](https://www.nerding.at/cv/) came together to continue some work they had begun as part of the ["Patterns InBetween Intelligences" project](https://www.stnds.de/aktuelles/link_ki). 


## Connecting Sensors & Live Coding 

In a previous iteration of the work, we made a sensor suit that was to be worn by performers as part of a 4-hour durational piece ['Pattern Parade'](https://www.nerding.at/mos-aick-pattern-parade/) shown on March 29, at Transmediale Studio/Silent Green, Berlin. This sensor suit was designed with (flex sensor? which?) connected to a remote Bela Mini board. The Machine Learning library [mllib](https://spark.apache.org/mllib/) was used to classify a range of gestures made by the sensor suits the performers were wearing. 

[Image - Sensor suits from performance March 2023 - assets/image02.jpeg]

The learnt data was used in various formats. The objective was to look for repeating patterns of movement from the performers sensed through the e-textile. Where movements were repeated, we wanted to use these to control the performance itself, as a way of gathering a sense of the collective movements of the performers, moving towards rhythmic and repetitive 'flow' states of music.  

[Image - System-Flow - assets/performance-outline.drawio.png ]

Firstly data (what data was this??) from the performers was collected and the repetitions were used directly in the music. This used the cyclical nature of the Tidal-Cycles live coding mini-language, where patterns built up over the TidalCycles unit of time 'the cycle' would become stronger when consistently repeated. This cycle was divided up into n-events, and each 1/n cycle would contribute to the pattern repetitions. These could then be directly turned into sound events in TidalCycles and thus the performers movements would drive the musical pattern being played in the performance. 

[Add image of circle visualisation]

Secondly, autocorrelation (McLaughlin and Raviv, 1968) was used as an algorithm for pattern recognition of the signals. The trained data was sent through the zero-mq library (Hintjens, 2013) - an open-source universal messaging library - to allow lossless messaging across a network. 

## Modulating Time 

For this iteration of the project, we worked further on the concept of 'modulating time', where in this iteration, instead of the data coming from sensors on performers, we wanted to work with the audience as the catalysts of the performance. 


## 








### References 

McLaughlin, J.A. and Raviv, J., 1968. Nth-order autocorrelations in pattern recognition. Information and Control, 12(2), pp.121-142.


Hintjens, Pieter. 2013. ZeroMQ: Messaging for Many Applications. "O’Reilly Media, Inc."