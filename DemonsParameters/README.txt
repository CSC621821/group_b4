To run (DeformableRegistion2.cxx):

./Demons fixedImageFile movingImageFile outputImageFile[outputDisplacementFieldFile] numberOfHistogramLevels numberOfMatchPoints numberOfIterations standardDeviation

*NOTE: default parameter values are:

numberOfHistogramLevels: 1024
numberOfMatchPoints: 7
numberOfIterations: 50
standardDeviation: 1.0

------------------------------------------------------

To run (DeformableRegistion17.cxx):

./Demons fixedImage movingImage registeredImage deformationField numberOfHistogramLevels numberOfMatchPoints standarDeviation numberOfLevels

*NOTE: default parameter values are:

numberOfHistogramLevels: 1024
numberOfMatchPoints: 7
standardDeviation: 1.0
numberOfLevels: 4
