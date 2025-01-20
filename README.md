# SpheroidPicker  

This repository designed to reproduce the SpheroidPicker system, providing tools and resources for both hardware handling and image analysis. 

### Schematics  

<img src="./images/schematics.png" alt="Schematics" width="600"> 

<br><br>

The system includes a stereo microscope, syringe, stage, and manipulator controller. The automatic screening function results in brightfield images of the spheroids. The segmentation and feature extraction steps are based on a deep learning model. After the selection of the spheroids, the spheroid picker automatically transfers the spheroids into the target plate.

## Repository Structure  

1. **`AutomaticSpheroidPickerSoftware`**  
   Contains C++ software for interfacing with and managing the specific hardware components used in the SpheroidPicker system.  

2. **`SpheroidPicker-Image-analysis`**  
   Includes a Docker environment to train and reproduce the results presented in the publication.  

## System Overview  

### SpheroidPicker system
<img src="./images/Realillustration-02.png" alt="Real Illustration" width="600">  


### 3D Printed Parts  

Download the 3D printed part designs here:  
[https://doi.org/10.5281/zenodo.14679243](https://doi.org/10.5281/zenodo.14679243)  

#### Printer Recommendation  
We recommend using a **Prusa i3 MK3** for printing, but any filament-based printer supporting **PET-G** and having a minimum build size of **200 × 200 × 100 mm** can be used.  

#### Printing Guidelines  

- **Nozzle**: Use a **0.4 mm brass nozzle**.  
- **Plate Holders**:  
  - Material: PLA  
  - Bed Temperature: 60 °C  
  - Hotend Temperature: 210 °C  

- **Manipulator Parts**:  
  - Material: PET-G  
  - Bed Temperature: 90 °C  
  - Hotend Temperature: 245 °C  

- **General Settings**:  
  - Nozzle: Brass, 0.4 mm hole diameter  
  - Layer Height: 0.15 mm  

#### Design and Slicing  
- The models were designed in **Autodesk Inventor**.  
- Slicing was performed using **PrusaSlicer**. 

## Citation  

If you use this repository, please cite the following publication:  




```bibtex
@article{grexa2021spheroidpicker,  
  title={SpheroidPicker for automated 3D cell culture manipulation using deep learning},  
  author={Grexa, I. and Diosdi, A. and Harmati, M. and others},  
  journal={Scientific Reports},  
  volume={11},  
  pages={14813},  
  year={2021},  
  publisher={Nature Publishing Group},  
  doi={10.1038/s41598-021-94217-1}  
}
```
```bibtex
@phdthesis{grexa2024development,
  title={Development of intelligent microscopy systems},
  author={Grexa, Istv{\'a}n}
}
```