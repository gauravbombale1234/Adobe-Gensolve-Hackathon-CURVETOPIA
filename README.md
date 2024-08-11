## README: Curvetopia - A Journey into the World of Curves

### Overview
Welcome to **Curvetopia**! This project is dedicated to the exploration, identification, regularization, and beautification of 2D curves. Our focus is on working with various types of curves, starting with simple closed shapes and gradually moving towards more complex formations. The journey includes discovering symmetry in these curves and developing techniques to complete any incomplete curves.

### Objectives
- **Identify Curves**: Recognize various regular shapes within a set of curves such as straight lines, circles, ellipses, rectangles, polygons, and star shapes.
- **Regularize Curves**: Transform irregular shapes into more regular and aesthetically pleasing forms.
- **Symmetry Detection**: Identify and analyze symmetry within closed curves, such as reflection symmetry, where a curve can be divided into mirrored halves.
- **Curve Completion**: Fill in gaps or incomplete sections of curves to produce a smooth and continuous shape.

### Problem Description
The primary challenge is to take a polyline representation of line art and convert it into a set of connected cubic Bézier curves. We aim to regularize these curves, identify any symmetry present, and complete any incomplete shapes. The final output should be a set of well-defined and smooth curves in SVG format, ready for visualization.

### Key Features
1. **Regularize Curves**:
   - Recognize and regularize simple geometric shapes from a set of curves.
   - Handle various shapes like straight lines, circles, ellipses, rectangles, polygons, and stars.

2. **Explore Symmetry**:
   - Detect symmetry in closed curves, particularly reflection symmetry.
   - Identify symmetry using point-based transformations and fit Bézier curves to symmetric points.

3. **Complete Curves**:
   - Develop algorithms to naturally complete curves with gaps caused by occlusions or incomplete drawings.
   - Handle different levels of shape occlusion, from fully contained shapes to disconnected curves.

### Input & Output
- **Input**: The input is a set of paths represented as polylines in CSV format. Each path is a sequence of points in 2D space.
- **Output**: The output is a set of curves, ideally represented as cubic Bézier curves, visualized in SVG format.

### Expected Results
- **Regularization & Symmetry**: The output should feature well-regularized shapes with detected symmetry where applicable.
- **Curve Completion**: The algorithm should successfully complete incomplete curves, resulting in smooth, continuous shapes.

### Evaluation Criteria
- **Regularization**: Number of regular geometric shapes identified and successfully regularized.
- **Symmetry**: Accuracy in detecting symmetry and fitting Bézier curves to symmetric points.
- **Curve Completion**: Effectiveness of the curve completion process, evaluated through rasterization and visual comparison.

### How to Run the Code
1. **Reading CSV Files**: Use the provided `read_csv()` function to load polyline data from CSV files.
2. **Visualizing Curves**: Use the `plot()` function to visualize the loaded curves.
3. **Generating SVG Output**: Use `polylines2svg()` to convert the processed curves into SVG format for visualization.

### Example Files
- **Isolated Shapes**: `examples/isolated.csv`
- **Fragmented Shapes**: `examples/frag0.csv`, `examples/frag1.csv`
- **Occluded Shapes**: `examples/occlusion1.csv`, `examples/occlusion2.csv`

### Conclusion
Curvetopia provides a structured approach to working with 2D curves, offering tools for regularization, symmetry detection, and completion. The project aims to transform simple line art into beautiful and regularized curves, ready for use in various applications.

Enjoy your journey into the world of curves with Curvetopia!
