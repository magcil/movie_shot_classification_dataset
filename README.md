# movie_shot_classification_dataset
A dataset with classified film shots.

## Dataset classes
The dataset contain the following 9 classes that where extracted from movies
| Shot type                     | instances |
|-------------------------------|-----------|
| Static (985 shots)            | 985       |
| Handled (273 shots)           | 273       |
| Panoramic (207 shots)         | 207       |
| Travelling_in (55 shots)      | 55        |
| Travelling_out (46 shots)     | 46        |
| Vertical_movements (52 shots) | 52        |
| Zoom in (51 shots)            | 51        |
| Aerial (51 shots)             | 51        |
| Panoramic_lateral (46 shots)  | 46        |
| **Total**                     | 1766      |

## Dataset files

After extracting a sequence of 2 frames/sec for all shots, three kinds of pre-computed features are available in a npy format for the dataset: 

1. **sequentail_vgg_features** directory contains, for each shot, a sequence of features that are extracted using the first linear layer of the VGG16 network
2. **sequentail_features** directory contains, for each shot, a sequence of features that are extracted using the visual analysis from [multimodal_movie_analysis](https://github.com/tyiannak/multimodal_movie_analysis) library.
3. **aggregated_features** directory contains, for each shot, 4 statistics (std ratio, top-10 percentile, mean of the delta features and std of the delta features) that are calculated based on a sequence of features that are extracted using the visual analysis from [multimodal_movie_analysis](https://github.com/tyiannak/multimodal_movie_analysis) library.

## Cite

To be filled 
