# Drawing Participation: Reblocking a Million Neighborhoods
### — A generative AI and collaboration tool for the common good, addressing urban migration

## Reference Repository

### About the Project
Drawing Participation: Reblocking allows global mapping and characterization of informal settlements and provides a scalable tool to develop cadastral maps for these communities as they plan for future growth and urbanisation.

It addresses the current scarcity of municipal planning data and seeks to empower literacy and collaboration in the vernacular building process. This builds a foundation for land-tenure, municipal recognition, and essential infrastructure planning, such as energy, freshwater, and sanitation.

The approach automates a wide range of tasks, scaling and supporting on-site work currently manually performed on-site by surveyors and NGOs.

### 
The project was made possible by the Prototype Fund and was funded through the Federal Ministry of Education and Research from March 2024 until August 2024. Read more on the Prototype Fund's [Demo Week 15 Website](https://prototypefund.de/project/million-neighborhoods-re-blocking/) (in German).

If you are interested in supporting or joining the project or simply want to find out more, please reach out via [mail(at)drawing-participation.org](mailto:mail@drawing-participation.org]). We're looking forward to hearing from you!

### Broader Scope
Our software architecture has three main components: 
1. We provide a Generative Ensemble Model (GEM) to produce plausible baseline parcel maps based on satellite imagery of existing building structures, 
2. An online multi-user design interface for residents of informal neighborhoods to modify baseline parcel maps and to crowdsource parcel maps,
3. A version control system to record and synthesize competing resident proposals to arrive at common-ground neighborhood parcel maps.

### Current specific Scope
We have so far developed the first component, the Generative Ensemble Model. 

It has has five different steps:
(1) gathering openly accessible GIS data on building footprints and parcel outlines, 
(2) generate training data with that data on top of satellite imagery, 
(3) train multiple image-to-image translation models (based on a pix2pix architecture), 
(4) use a quantitative and qualitative model evaluation approach,
and lastly,
(5) provide a model that can synthesize the output of different models to adapt to the specific contextual characteristics of a given neighborhood

### Python Libraries
The python libraries below allow you to perform data acquisition, model training, and model synthesis.
In addition, you can find a set of pretrained models on [Hugging Face](https://huggingface.co/scalable-design-participation-lab/building-to-parcel/tree/main), available for download and use for users with less background knowledge or computing resources.

With these tools, any user can develop vector datasets based on existing building structure information.

#### Repositories
- [building2parcel-trainingdata](https://github.com/scalable-design-participation-lab/building2parcel-trainingdata)  
- [building2parcel-pix2pix](https://github.com/scalable-design-participation-lab/building2parcel-pix2pix)  
- [building2parcel-ensemble](https://github.com/scalable-design-participation-lab/building2parcel-ensemble)

### License
Unless otherwise described, the code in this repository and its sub-repositories is licensed under GNU AGPLv3. Please note that some modules, extensions, fonts or code herein might be licensed otherwise. If you have any questions, don't hesitate to get in touch via [email](mailto:mail@drawing-participation.org).
