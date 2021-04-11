# automated_hybrid_IDH  

This code tests one sample at a time using Jupyter-Notebook. 
If you want to test multiple cases at once (from DICOM to IDH status) check my [IDHpredict](https://github.com/ihrapsa/IDHpredict) repo  
**Note!**
* This fork also includes the skullstripping part.
* You need to convert DICOM files to NIFTI format before feeding the input to the pipeline. I used [MRIcroGL](https://github.com/rordenlab/MRIcroGL12) that is a DICOM/NIFTI viewer as well as convertor based on [dcm2niix](https://github.com/rordenlab/MRIcroGL12)
____________________________________
![alt_text](/workflow.png)
___________________________________

This is public repository for "Fully Automated Hybrid Network to Predict IDH Mutation Status of Glioma via Deep Learning and Radiomics" by Choi et al.
 The automated hybrid model consists of UNet-based Model1 for tumor segmentation, ResNet-based Model 2 for IDH status prediction, and automated processing pipeline inbetween. Model 2 integrates 2D MR images, radiomic features of 3D tumor shape & loci, and age in one CNN. The code to test a sample is avaialble as a jupyter notebook in 'Model_testing.ipynb'.
 
