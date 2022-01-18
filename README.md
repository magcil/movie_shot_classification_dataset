# movie_shot_classification_dataset
A dataset with classified film shots.

## Dataset classes
The dataset contains the following 10 classes that where extracted from movies
| Shot type           | instances |
|---------------------|-----------|
| Static              | 985       |
| Handled             | 273       |
| Panoramic           | 207       |
| Travelling_in       | 55        |
| Vertical_movements  | 52        |
| Zoom in             | 51        |
| Aerial              | 51        |
| Travelling_out      | 46        |
| Panoramic_lateral   | 46        |
| Tilt                | 37        |
| **Total**           | 1803      |

## Dataset files

After extracting a sequence of 5 frames/sec for all shots, three kinds of pre-computed features are available in a npy format for the dataset: 

1. **sequential_vgg_features** directory contains, for each shot, a sequence of features that are extracted using the first linear layer of the VGG16 network
2. **sequential_features** directory contains, for each shot, a sequence of features that are extracted using the visual analysis from [multimodal_movie_analysis](https://github.com/tyiannak/multimodal_movie_analysis) library.
3. **aggregated_features** directory contains, for each shot, 6 statistics (mean, std, median by std ratio, top-10 percentile, mean of the delta features and std of the delta features) for the non-object features and the mean values of the object features that are calculated based on a sequence of features that are extracted using the visual analysis from [multimodal_movie_analysis](https://github.com/tyiannak/multimodal_movie_analysis) library.

## Cite

To be filled 
