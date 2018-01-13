# CLMandDlibEasyTool in C++
Easy to use CLM or Dlib 

Hi all
This is a Face landmark sdk include CLM and Dlib.

# Start Compiling CLMandDlib C++ example programs

1. Clone this project

2. Open CLMandDlib.sln

3.Set as start up prject to Sample project

4.change solution Configurations to "Release"

5.Run

# Change Dlib to CLM face landmark

Change code CreateFaceLandmark(LandmarkType::Dlib) to CreateFaceLandmark(LandmarkType::CLM) in SampleProject.cpp

# Get Face landmark Api

FaceLandmarkAPI Temp;                             // new FaceLandmarkAPI
Temp.CreateFaceLandmark(LandmarkType::CLM);       // 1.Set Face landmark type
Temp.initializationDataSet(strModel, 0);          // 1.Set 3rdparty Data path, 2.Set Camera ID
Temp.Run(vPoint3dLandmarkData, matImage, true);   // 1.Get Face landmark point, 2.Get Image, 3.Show resoult

# Code architecture

# Conclusion

Merge CLM ans Dlib face landmark SDK，use virtual interface class to design API.
