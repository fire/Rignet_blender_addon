# Rignet_blender_addon
Adopting https://github.com/zhan-xu/RigNet neural network we created an addon in blender for an intuitive and easy rigging of their existing template characters 
We strongly advise to use the latest version of blender available in order to use the addons

1)Setup of Anaconda that emulates our environment on windows 64x
--------
Install anaconda.

open anaconda navigator interface/program

go into environments

create a new environment with python 3.7

press the play button next to the created environment, open terminal

pip install numpy==1.20.2

pip install scipy==1.7.0

pip install matplotlib==3.4.2

pip install tensorboard==2.5.0

pip install open3d==0.9.0

pip install opencv-python==4.5.2.54

pip install rtree==0.9.7

pip install trimesh[easy]

conda install pytorch==1.8.1 torchvision==0.7.0 cudatoolkit=10.1 -c pytorch

pip install torch-scatter==2.0.7 -f https://pytorch-geometric.com/whl/torch-1.8.1+cu101.html

pip install torch-sparse==0.6.9 -f https://pytorch-geometric.com/whl/torch-1.8.1+cu101.html

pip install torch-spline-conv==1.2.1 -f https://pytorch-geometric.com/whl/torch-1.8.1+cu101.html

pip install torch-cluster==1.5.9 -f https://pytorch-geometric.com/whl/torch-1.8.1+cu101.html

pip install torch-geometric==1.7.2

Download from https://www.lfd.uci.edu/~gohlke/pythonlibs/#rtree the file named "Rtree‑0.9.7‑cp37‑cp37‑win_amd64.whl" then run on the console: pip install Rtree‑0.9.7‑cp37‑cp37‑win_amd64.whl

If any of the above ends up in an error it is possible to browse the created environment directly in anaconda navigator and install the above mentioned packages



2)https://github.com/zhan-xu/RigNet network setup
--------
Download the code of https://github.com/zhan-xu/RigNet and unzip it

Download the folder "checkpoints" form https://umass.box.com/s/l7dxfayrubf5qzxcyg7can715xnislwm and paste it within the folder "RigNet-master"

Download quick_start1.py from our github and paste it inside the folder RigNet-master (there is no need to delete the original quick_start.py within the folder)


3)Blender setup
--------
Once you downloaded the latest version of Blender, open the anaconda environment terminal again

Change folder path with "cd C:\Program Files\Blender Foundation\Blender 2.93"

Run "blender"

Blender should open on it own, from here go to "edit", "preferences", "addons", install

Browse your folder till you find the zipped folder "Addon_rignet" downloaded from our github

Select it. After a short delay it should appear next to a box which turns on the addon


4)Using the addon
--------
Press "N" to open the addon panel

Select the path where "RigNet-Master" is within your computer

Select from the list of object the one you choose to add inside blender

Run. The process may take a while depending on the complexity of the the object chose for the rigging

After a while the object will appear at the center of the world centered in the cursor. If you don't see it it's because the object is very small, just zoom in until you see it

5)Expandind the addon with new objects to rig
--------
In theory, https://github.com/zhan-xu/RigNet explains that it is possible to create new objects for the RigNet to work on. For any consideration related to the topic we advice the reader to check https://github.com/zhan-xu/RigNet because we don't know how to do it yet :p
