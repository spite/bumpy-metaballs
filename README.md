# Bumpy metaballs

Isosurface created with Marching Cubes, and bump added with normal mapping.

The metaballs don't have generated UV coordinates, and tangents can't be
calculated with the usual method because it relies on texture coordinates.

Following the triplanar mapping explained in this GPU Gems 3 article is possible
to generate the Tangent Space Basis in the fragment shader.

Shading is the same MatCap as Spherical Environment Mapping.

Code by Jaume Sánchez @thespite using three.js.
