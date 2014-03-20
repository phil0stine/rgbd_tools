rgbd_tools
==========

rgbd processing scripts to accomodate various datasets

add_pointclouds_to_bagfile.py is a fork of the version provided by TUM, that can be found at http://vision.in.tum.de/data/datasets/rgbd-dataset

The script takes bagfiles with calibrated color and depth image streams as input, and outputs the same bag with added pointcloud messages.

The script originally assumed square pixels (fx=fy), but for the case of calibrated cameras, both fx and fy should be used for projection and re-projection.

The updated version uses both fx and fy to create the PointCloud messages.

