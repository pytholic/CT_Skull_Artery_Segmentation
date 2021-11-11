# CT Skull Artery Segmentation
Segmentation of arteries in CT skull scans. We will use the `Deep Learning-based` approach.

## Steps
* Collecting data
* Preprocessing
* Groundtruth Masks
* Training and Validation
* Testing

### Data collection
Skull CT scans of 49 patients are collected.

### Preprocessing

### Labeling the Dataset
The next main and crucial step is to generate ground-truth masks. We can do this *manually* or in a *semi-automated* way using some image processing tools like **3D Slicer**, **VTK**, **OpenCV**, etc.

#### Main issue
There are two main issues with generating `ground-truth masks` for arteries in CT data.

* Need of a **medical expert**. For medical image data, we always need an expert from that field who can help us label the data correctly. It is very crucial for the good performance of the deep learning models, especially for the medical domain. However, currently, I am struggling with this since we do not have access to any medical personnel. Therefore, I am trying to figure it out myself. It is difficult to find a way, especially for skull arteries. In addition, arteries are not quite visible in my dataset.
* Secondly, the intensity values of arteries overlap with other segments of the brain like bones and even background. So it is really hard to threshold them at the moment.
