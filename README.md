# 3D-printing the Cosmic Microwave Background Radiation temperature anisotropy

This repository contains code and artifacts for a 3-D printable sphere with bumps
and valleys corresponding to the high and low temperatures of the Cosmic Microwave
Background Radiation (CMBR). We map 0.0004 K (valley-to-peak) out of 2.73 K (0.015%)
to 20% of the radius (valley-to-peak). That's an amplification factor of ~1365×.

## Contents

```
├── README.md
├── binary_artifacts
│   ├── cmbr.stl: the raw output of cmbr_mesh.ipynb, a whole spiky sphere
│   ├── cmbr_bottom.stl: the bottom half of a cut-in-half sphere with a channel for a dowel
│   ├── cmbr_hollow_split.f3d: the Fusion 360 file containing all history of importing and repairing the mesh, turning it into a solid, then slicing in half and making suitable for a dowel
│   ├── cmbr_top.stl: the top half of a cut-in-half sphere with a channel for a dowel
│   ├── dowel.stl: the keyed dowel to connect _top and _bottom
│   └── ornament
│     ├── cmbr_ornament_bottom.stl: bottom half of solid sphere with a ring added for hanging (no dowel needed)
│     └── cmbr_ornament_top.stl: top half of solid sphere with a ring added for hanging (no dowel needed)
├── cmbr_mesh.ipynb: Jupyter notebook containing the executable Rust code to read Planck data, downsample, map, and output to an STL file
└── cmbr_mesh.pdf: Print to PDF of the Jupyter notebook
```

## Requirements

See the Jupyter notebook [cmbr_mesh.pdf](cmbr_mesh.pdf) for details.

## License

This work is licensed under CC BY 4.0. ![CC](https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1) ![BY](https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1)
