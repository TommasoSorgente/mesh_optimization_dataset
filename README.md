# mesh_optimization_dataset
Datasets used for "Mesh Optimization for the Virtual Element Method: How Small Can an Agglomerated Mesh Become?" by T. Sorgente, F. Vicini, S. Berrone, S. Biasotti, G. Manzini and M. Spagnuolo. 

The repository contains two **polygonal datasets**:

<p align="center"><img src="tet_datasets.png" width="500"></p>

two **polyhedral datasets**:

<p align="center"><img src="hex_datasets.png" width="500"></p>

and one **cad mesh**:

<p align="center"><img src="voro_datasets.png" width="500"></p>

## Content

Each .zip file contains a dataset made of five meshes with decreasing mesh size; dataset "tet" is divided in two parts due to the file size limitations of GitHub.

Each mesh is saved in the _OVM_ format, which consists in a file containing informations on 
- the vertices: _x-coord____y-coord____z-coord_
- the edges: _vertex0-id____vertex1-id_
- the faces: _#verts___vertex-id-list_ (only for polyhedral meshes)
- the elements: _#faces___faces-id-list_ (_verts-id-list_ for polygonal meshes)

Together with the original meshes, there are their optimized versions presented in the paper.
For each optimized mesh, we provide the OVM mesh file and a _mesh_hierarchy_ file containing the relationship between the original and the optimized mesh.

...

## Citing us
If you use one or more datasets in your academic projects, please consider citing the original paper using the following BibTeX entry:

```
@article{sorgente2024mesh,
  title={Mesh Optimization for the Virtual Element Method: How Small Can an Agglomerated Mesh Become?},
  author={Sorgente, Tommaso and Berrone, Stefano and Biasotti, Silvia and Manzini, Gianmarco and Spagnuolo, Michela and Vicini, Fabio},
  journal={arXiv preprint arXiv:2404.11484},
  year={2024}
}
```

## Acknowldegment
Funded by the European Union - NextGenerationEU and by the Ministry of University and Research (MUR), National Recovery and Resilience Plan (NRRP), Mission 4, Component 2, Investment 1.5, project “RAISE - Robotics and AI for Socio-economic Empowerment” (ECS00000035).
However, the views and opinions expressed are those of the authors alone and do not necessarily reflect those of the European Union or the European Commission. 
Neither the European Union nor the European Commission can be held responsible for them.
S. Biasotti, G. Manzini, T. Sorgente, and M. Spagnuolo are part of the RAISE Innovation Ecosystem.
F. Vicini, S. Berrone, and G. Manzini are members of the Gruppo Nazionale Calcolo Scientifico-Istituto Nazionale di Alta Matematica (GNCS-INdAM); this work has been partially supported by INdAM-GNCS Project CUP: E53C23001670001, by the MUR PRIN project 20204LN5N5\_003, and by the European Union through the project Next Generation EU, PRIN 2022 PNRR project P2022BH5CB\_001 CUP:E53D23017950001.
