# SimilarBrain
Code to use a KNN to find patients with similar brain tumours
Takes MRI scans, consider then as slices, train a CAE over the slices.
Use the middle layer (bottleneck) of the CAE to induce a vector space, within which every image is represented
To use it, input a query MRI - i.e. "Find an MRI like this one"
Decomposes the input MRI into a set of slices and use a Nearest Neighbour approaches to find similar slices
Aggregate over patients (i.e. choose the patients who have the highest number of similar slices) and chose the 5 most common "similar" patients.
