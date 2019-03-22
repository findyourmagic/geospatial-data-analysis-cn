# Scipy 2018 教程 - Python地理信息数据分析介绍

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/geopandas/scipy2018-geospatial-data/master)

### 导师

- [Levi John Wolf](https://ljwolf.org) - [University of Bristol](http://www.bristol.ac.uk/geography/levi-j-wolf/overview.html)
- Sergio Rey - [Center for Geospatial Sciences, University of California, Riverside](http://spatial.ucr.edu/peopleRey.html)
- [Dani Arribas-Bel](http://darribas.org/) -  University of Liverpool
- [Joris Van den Bossche](https://jorisvandenbossche.github.io/) - Université Paris-Saclay Center for Data Science 

本教程是关于使用Python分析地理信息数据的介绍, 主要聚焦于表格矢量数据. 它首先着重于介绍用于处理地理信息数据的各种包，也会涵盖地理数据的解析处理及其探索其在空间内的关系. 包括导入各种格式数据 (e.g. shapefile, GeoJSON), 可视化, 为了分析进行数据合并和数据清理, 还会学习使用这些包 `pandas`, `geopandas`, `shapely`, `PySAL`, 或 `rasterio`. 第二步会基于这个基础上聚焦于更加高级的地理数据科学和统计学方法洞察数据. 对于这些 Python 包的使用经验不是必须的, 但是了解基本的地理数据概念 (shapefiles, vector vs raster data) 以及了解 pandas 会帮助理解.

## 目录

[Python地理信息向量数据处理介绍](./01-introduction-geospatial-data.ipynb)


## 日程

- 7:50 - 8:20: **安装 & 配置**

- 8:20 - 9:00: **处理地理信息数据**

  <!-- synthesize `01,04,05` -->

- 9:00-10:00: **地理信息关系和连接**

  <!-- synthesize `02,03`, plus a very small bit of `99` -->

- 10:00 - 10:10: **休息**

- 10:10 - 11:00: **探索性地理数据分析**

  <!-- notebook `03,08` for profiles of clusters -->

- 11:00 - 12:00: **使用空间模型**

  <!-- notebook `07`, basic feature engineering, kernel regression, & endog regression -->

## 安装提示

本教程需要用到以下软件和包:

- Python >= 3.5 (it will probably work on python 2.7 as well, but I didn't test it specifically)
- pandas
- geopandas >= 0.3.0
- matplotlib
- rtree
- PySAL
- scikit-learn
- mgwr
- cartopy
- geoplot
- [Jupyter Notebook](http://jupyter.org)

如果你还没装这些软件和包，我们推荐 [conda](http://conda.pydata.org/docs/intro.html) 包管理工具 
(可以安装 [miniconda](http://conda.pydata.org/miniconda.html) 或者 (体积更大) Anaconda https://www.anaconda.com/download/).

装好 miniconda/anaconda 以后, 使用下面的命令安装所有依赖生成 Python 环境:

```
conda env create -f environment.yml
```

当然其他发行版 (e.g. Enthought Canopy) 或者 ``pip`` 也行 (依赖文件也已提供), 只要你装好上面这些软件和包.


## 下载教程素材

推荐通过克隆教程仓库下载素材:

    git clone https://github.com/geopandas/scipy2018-geospatial-data


## 测试教程环境

为了确保所有安装都能正常运行, 打开命令行, 并且切换到教程文件目录下，然后运行以下命令:

```sh
python check_environment.py
```

确保命令行打印出以下字样 "All good. Enjoy the tutorial!"

