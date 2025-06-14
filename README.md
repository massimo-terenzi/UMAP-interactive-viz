# UMAP Interactive Visualization Tool

An interactive web tool for exploring UMAP (Uniform Manifold Approximation and Projection) results with advanced clustering and data analysis features.

The tool is available here: [https://massimo-terenzi.github.io/UMAP-interactive-viz](https://massimo-terenzi.github.io/UMAP-interactive-viz/)

## ✨ Key Features

### 📊 Interactive Visualization
- **UMAP scatter plot** with color-coded cluster points
- **Smooth zoom and pan** with mouse wheel and dedicated controls
- **Zoom selection** - Draw a rectangle to zoom into specific areas
- **Reset view** to return to full dataset view

### 🎯 Cluster Filtering
- **Click on cluster colors** in legend to isolate/show specific groups
- **Visual feedback** with points becoming transparent
- **Dynamic statistics** that update based on active filters

### 🖼️ Detailed Preview
- **Click on points** to view detailed information
- **Image loading** from Google Drive with loading animations
- **Associated text** and descriptions for each data point
- **Direct link** to original image

### 📁 Data Loading
- **Simple CSV upload** with drag & drop support
- **Robust parsing** handles complex CSV files
- **Data validation** with clear error messages
- **Progress bar** during loading process

## 🎮 How to Use

### 1. Load Your Data
- Click "📁 Load CSV File"
- Select your UMAP file (format specified below)
- Wait for loading and automatic chart generation

### 2. Explore the Visualization
- **↔ Pan Mode**: Move and zoom normally
- **⬚ Zoom Selection**: Drag to create a zoom rectangle
- **Mouse wheel**: Quick zoom
- **+ / -**: Incremental zoom
- **⌂**: Reset to full view

### 3. Filter by Cluster
- **Click on colors** in the legend to isolate specific clusters
- **Click again** to show all points
- Statistics update automatically

### 4. Analyze Details
- **Click on points** to see image preview and metadata
- **View original image** by clicking the link

## 📋 Required CSV Format

Your CSV file must contain these columns:

```csv
cluster,UMAP1,UMAP2,file_name,file_url,post_text,description
1,2.34,-1.56,image1.jpg,https://drive.google.com/file/d/ID/view,Sample text,Detailed description
2,0.12,3.45,image2.jpg,https://drive.google.com/file/d/ID/view,Another text,Another description
```
- `filename` *(optional)*: name of the image file  
- `file_url`: full URL to the image file (e.g., Google Drive link)  
- `post_text`: original text associated with the post  
- `description`: detailed or connotative description of the image
