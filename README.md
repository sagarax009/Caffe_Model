# Caffe for Medical Image Segmentation

Hi This is subject to new ones from my experience with caffe and medical image segmentation hope it will be helpful too

1 In medical Images data is often 4 D ,(x,y,z,t) ,4th axis is time at which data is available (0 or 1) ,just squeeze the array to get 3D volume. I will give example code soon.
2 Label: If you see normal caffe the label file is often .txt containing imagenumber, class name (n12345,Robin) ,do not live in this world when it comes to medical image segmentation ,I have spent 15 days what is mean by label for medical data.It is nothing but the 3-D volume -binary mask.Use 3D slicer or MITK to generate it ,its painful work but no way.
3 Now by somehow you have data (3-D image) and (3-D label) which format to use ,as you see there are lmdb,hdf5 great,but when you use MITK then I recommend save those files (image and label) in .nrrd format. Trust me ,it pays off
4 Next is which caffe model to choose ,if it is segmentation then U-Net,V-Net are good to go . I am working with V-Net
5 Remaining experinces I will put soon 

