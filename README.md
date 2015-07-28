# DLCA

A C++ implementation of the **diffusion-limited cluster-cluster aggregation** (DLCA), an algorithm to generate aerogel structures.

# Usage

1. Parameters

    - ```[D]``` Dimension of the grid.

    - ```[L]``` Size of the grid. E.g. ```L``` x ```L``` for ```D``` = 2.

    - ```[N]``` Number of particles in the grid.

    - ```[F]``` The output file name, without ```.txt``` suffix. E.g. ```output/D2.L10.N10```.

    - ```[P]``` The period for snapshots.

    - ```[I]``` The number of iterations.
    
    - ```[M]``` The marker size of plots.

2. Windows

    - Single run

        - 32-bit

            ```bat
            exe\win32\DLCA.exe [D] [L] [N] [F]
            ```

        - 64-bit

            ```bat
            exe\win64\DLCA.exe [D] [L] [N] [F]
            ```

    - Visualizing single run
    
        ```
        python visualize.py [D] [L] [INPUT] [OUTPUT] [M]
        ```
            
    - Creating GIF ([Python](https://www.python.org/), [matplotlib](http://matplotlib.org/), and [ImageMagick](http://www.imagemagick.org/) required)

        ```bat
        create_demo.bat [D] [L] [N] [P] [M]
        ```

3. Linux

    - Build (C++11 support required)

        ```sh
        make
        ```

    - Single run

        ```sh
        bin/dlca [D] [L] [N] [F]
        ```
        
    - Visualizing single run
    
        ```
        python visualize.py [D] [L] [INPUT] [OUTPUT] [M]
        ```
        
    - Creating GIF ([Python](https://www.python.org/), [matplotlib](http://matplotlib.org/), and [ImageMagick](http://www.imagemagick.org/) required)

        ```sh
        create_demo.sh [D] [L] [N] [P] [M]
        ```

# Benchmark



# GIF demo

- [D2.L128.N2000](https://github.com/zhangns/DLCA/tree/master/demo/D2.L128.N2000)

    ![D2.L128.N2000](https://raw.githubusercontent.com/zhangns/DLCA/master/demo/D2.L128.N2000/animation.gif)

- [D2.L1024.N50000](https://github.com/zhangns/DLCA/tree/master/demo/D2.L1024.N50000)

    ![D2.L1024.N50000](https://raw.githubusercontent.com/zhangns/DLCA/master/demo/D2.L1024.N50000/animation.gif)

# Related info

- [Computer Simulations of Cluster-Cluster Aggregation](http://dx.doi.org/10.1039/DC9878300125)

- [Formation of Fractal Clusters and Networks by Irreversible Diffusion-Limited Aggregation](http://dx.doi.org/10.1103/PhysRevLett.51.1119)

- [Mechanical structure-property relationship of aerogels](http://dx.doi.org/10.1016/S0022-3093(00)00288-X)

- [Scaling of Kinetically Growing Clusters](http://dx.doi.org/10.1103/PhysRevLett.51.1123)

# License

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
