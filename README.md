# TerrainDecorator
![terrain decorator cover](https://user-images.githubusercontent.com/62556242/183722147-92a19c3e-9275-497b-9900-febe5d1e768e.jpg)


TerrainDecoration is Rule-based terrain texturing tool for Unity3D.

I am publishing it as it is because I believe that I can no longer find time and correct my mistakes due to a difficult work schedule :(  It would be nice if someone could fix it.
It contains filters such as slope, height, noise, image mask and blend modes that can be used in combination. It consists of 2 scripts. You can put the "MiniTerrainDecorator" script on the terrain and start entering the rules.

tutorial: https://youtu.be/veQOj4AJxZI

![Screenshot 2022-08-07 194304](https://user-images.githubusercontent.com/62556242/183722260-cc1ea8f1-0b80-4bd1-8238-507fbaa0708f.png)
![Screenshot 2022-08-09 203346](https://user-images.githubusercontent.com/62556242/183722269-1c4a4241-1109-403e-8102-59b21a2b7cdc.png)


TODO & BUGS

- If adding, removing or changing layers or trees while minidecorator is present, terrainDecorator may crash very badly. It would be more appropriate to add miniDecorator after this process is finished.

- There is a big bug with weight calculation. unexpected behavior occurs when there are too many rules. please someone solve

- It should be optimized, it gets very slow at 4096x4096 resolution, especially if there are image filters.

- "show progress" is very problematic. That's why I said it was experimental. It looks very stylish in videos, but if there is an error, it is very difficult to fix. And It's running very slow. Only, It can be used for demonstration purposes.

- perlin noise in is very difficult to control. luckily, i give nice noise images instead. Better noise patterns can be achieved using ImageFilter.

- A tile parameter can be added for the image filter.

- Since I work in hdrp, I did not add grass/details textures/models. they can be added the parameters in the tree insertion part are very experimental


