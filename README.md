# Pokemon-CompVision-Fill-In

A computer vision project designed to generate in-between animation frames from a set of key frames. Given a start frame, an end frame (and optionally intermediate key frames), the model interpolates the missing frames in between reducing the manual labor required of animators and lowering production costs for studios.

## Required Packages
These are the required Python packages to run the scripts:

- Matplotlib
- NumPy
- tqdm
- Torch

##### pip Installation

```
!pip install opencv-python-headless
```

##### Data
Training data was sourced from three Pokémon animated films
- Pokémon: The First Movie — Mewtwo Strikes Back
- Pokémon: The Movie 2000 — The Power of One
- Pokémon 3: The Movie — Spell of the Unown

```
https://archive.org/details/pokemon-kanto-movie-collection/1.+Pok%C3%A9mon+The+First+Movie+-+Mewtwo+Strikes+Back.mkv 
```

## Repo Contents:
 - `Image_to_Video_Project.ipynb` main script to extract clips, model training, and producing predictions 
 - `Prediction Videos` Folder containing prediction gifs versus the actual clips
 - `Clips_metaData` meta data for the training clips produced by the script

## Missing Content   
 - `Movies` to large to render into repo
 - The training clips produced by the script as they were to large to put in the 

## Limitations
- Currently trained on a single animation studio's visual style; generalization to other studios may vary
- Long-range motion (fast action sequences) may produce artifacts
- The 9-frame extended clips dataset is small (30 clips) and may limit sequence generation quality
