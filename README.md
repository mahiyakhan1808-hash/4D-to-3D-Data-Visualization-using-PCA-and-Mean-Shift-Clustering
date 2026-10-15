4D to 3D Data Visualization using PCA and Mean Shift Clustering
Project Overview
This project demonstrates how to reduce four-dimensional numerical data to three dimensions using Principal Component Analysis (PCA) and visualize the results in a 3D scatter plot. It also applies Mean Shift clustering to the original four-dimensional data and displays the predicted cluster labels in a second 3D plot.
Dataset
The project uses the built-in Iris dataset from scikit-learn. It contains 150 samples and four numerical features:
- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)
Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
Workflow
1. Load the Iris dataset using load_iris().
2. Convert the feature data into a Pandas DataFrame.
3. Select all four features as the input data (X).
4. Apply PCA(n_components=3) to transform the data into three dimensions.
5. Plot the transformed data in a 3D scatter plot.
6. Fit a MeanShift clustering model to the original four-dimensional data.
7. Visualize the PCA-transformed points again, colored by their predicted cluster labels.
Installation
Install the required packages:
pip install numpy pandas matplotlib seaborn scikit-learn
How to Run
1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Run:
python 14_oct_3d.py
The script displays two 3D scatter plots. You can also run the code in a notebook environment such as Google Colab.
Output
- 3D PCA visualization: A scatter plot of the Iris dataset after dimensionality reduction.
- 3D cluster visualization: A scatter plot of the same transformed points, colored according to Mean Shift cluster predictions.
Note: PCA is used for visualization, while Mean Shift clustering is fitted on the original four-dimensional features. The first plot does not assign a color variable to its points; the second uses predicted cluster labels.

Future Improvements
- Add axis labels and plot titles.
- Display the number of clusters identified by Mean Shift.
- Report PCA explained variance ratios.
- Save the visualizations as image files.
Project File
- 14_oct_3d.py — Python source code for PCA, clustering, and 3D plotting.



