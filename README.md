# 🖼️ Image Compression With K-Means

## 📌 Introduction

This project demonstrates **K-Means based image compression**, a powerful unsupervised machine learning technique to reduce image file size while maintaining visual quality. By clustering similar colors in an image and replacing them with their cluster centers, we can significantly compress images with minimal perceptual loss.

## 🔧 How It Works

The project follows these key steps:

- **📂 Load Image**: Import an image file using PIL (Python Imaging Library)
- **🔄 Reshape Data**: Convert the 2D image into a 1D array of pixel values (flattening the image dimensions)
- **🎯 Apply K-Means Clustering**: Group similar colors into K clusters, where K is the number of colors to retain
- **🖌️ Reconstruct Image**: Replace each pixel with its nearest cluster center color
- **📊 Visualize Results**: Display side-by-side comparison of original vs. compressed images

## 📋 Requirements

This project requires the following dependencies:

- **numpy** - Numerical computing and array operations
- **matplotlib** - Data visualization and plotting
- **PIL (Pillow)** - Image loading and manipulation
- **scikit-learn** - Machine learning library for K-Means algorithm

### Installation

```bash
pip install numpy matplotlib pillow scikit-learn
```

## 🚀 Usage Instructions

Follow these steps to run the code:

1. **Open Jupyter Notebook**
   ```bash
   jupyter notebook Image_Compression_With_K_Means.ipynb
   ```

2. **Prepare Your Image**
   - Place your image file in the working directory
   - Update the image path in the notebook code

3. **Set K Value (Number of Colors)**
   - Modify the `n_clusters` parameter (default: 16)
   - Lower K values = higher compression, lower quality
   - Higher K values = better quality, lower compression
   - Example: `K = 8, 16, 32, 64, 128`

4. **Run All Cells**
   - Execute the notebook cells sequentially
   - The code will process the image and display results

## 📊 Output

The notebook produces:

- **Original Image**: The uncompressed source image with original file size
- **Compressed Image**: The K-Means compressed version with reduced file size
- **Comparison View**: Side-by-side visualization showing:
  - Original colors (millions of possible colors)
  - Compressed colors (limited to K clusters)
  - Compression ratio and quality metrics

### Compression Benefits

✅ Reduces file size by 50-90% depending on K value
✅ Maintains reasonable visual quality
✅ Useful for web optimization and storage
✅ Demonstrates practical ML applications

## 👤 Credits

- **Author**: [Nakshatra1729yuvi](https://github.com/Nakshatra1729yuvi)
- **Project**: K-Means Image Compression
- **Repository**: [GitHub Link](https://github.com/Nakshatra1729yuvi/K-Means)

---

**Happy Compressing!** 🎉
