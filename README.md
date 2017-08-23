# SPARE-Corpus
This repository holds the Birmingham-Tufts Spatial Referring Expression Corpus.

## Organization
- `corpus/` contains `data.csv` which has four columns: 
  - Description: an RE collected during our experiment.
  - image_id: the image shown to the participant during the experiment.
  - scene_id: the scene configuration used to generate that image.
  - Object Type: the type for the target referent.
- `img/` contains a set of .png files named with corresponding image_ids.
- `metadata/` contains `scenes.json`, which contains a list of image metadata entries. Each entry maps an imageid to a scene description, which contains:
  - pixel:  a list of entries that are either: 
    - WIDTH: the width of the image
    - HEIGHT: the height of the image
    - or an object name mapped to its bounding box within the scene
  - object: the name of the object bounded within the scene
  - scene_id: the scene_id for this configuration.
  
## License
   This corpus is released under a Creative Commons Attribution-ShareAlike 4.0 International license. 
   [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)

   If you use this data, please cite "Spatial Referring Expression Generation for HRI: Algorithms and Evaluation Framework" by Lars Kunze, Tom Williams, Nick Hawes, and Matthias Scheutz, as appeared in the proceedings of the 2017 AAAI Fall Symposium on Artificial Intelligence for Human-Robot Interaction (AR-HRI).

   ```@InProceedings{kunze2017arhri,
           author = {Lars Kunze and Tom Williams and Nick Hawes and Matthias Scheutz},
           title = {Spatial Referring Expression Generation for HRI: Algorithms and Evaluation Framework},
           booktitle = {{AAAI} Fall Symposium on Artificial Intelligence for Human-Robot Interaction ({AR-HRI})},
           year = {2017},
           address = {Arlington, VA, US}
           }```

Note that that paper used a subset of this corpus corresponding to data collected from participants that faithfully completed the entire experiment.

   

 