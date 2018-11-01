+++
title = "Logiciels gratuits pour le calcul scientifique"
date = "2018-11-01T08:47:59+01:00"
draft = false
layout = "docs"

# Does the project detail page use math formatting?
math = false

# Does the project detail page use source code highlighting?
highlight = true

[menu.tmp]
  name = "Software for scientific computing"
  weight = 1

+++


<!-- 
   - Free software for scientific computing
   - ======================================
   - 
   - Written by Antoine Le Hyaric [[http://www.ljll.math.upmc.fr/lehyaric]]
   - 
   - _references_ [[3D-Studio]] [[ADMesh]] [[ARPACK]] [[Atlas]] [[Automake]] [[Ayam]] [[BLAS]] [[Blender]] [[Blitz++]] [[Boost]] [[C++]]
   -              [[CAD]] [[CUDA]] [[Cilk]] [[Code_Aster]] [[Code_Saturne]] [[DDD]] [[Doxygen]] [[EMAP]] [[Elmer]] [[Emacs]] [[FAQ]] [[FEMM]]
   -              [[FElt]] [[FEniCS]] [[FFTW]] [[FLAME]] [[Fortran]] [[FreeFEM++-cs]] [[FreeFem++]] [[GDB]] [[GETM]] [[GRUMMP]] [[Geomview]]
   -              [[GetDP]] [[Getfem++]] [[Gmsh]] [[Gnuplot]] [[HDF]] [[Hypre]] [[IGES]] [[IML++]] [[ISAAC]] [[ITPACK]] [[Impact]] [[LAPACK]]
   -              [[LaTeX]] [[Libtool]] [[METIS]] [[MUMPS]] [[Matlab]] [[Maxima]] [[MayaVi]] [[Mercurial]] [[Meshing]] [[Méfisto]] [[Mélina]]
   -              [[NAPACK]] [[NCO]] [[NSC2KE]] [[Netgen]] [[OFELI]] [[OFF]] [[OOFEM]] [[Octave]] [[OpenMP]] [[OpenSees]] [[PARI/GP]]
   -              [[PBLAS]] [[PETSc]] [[PLAPACK]] [[POOMA]] [[PRIMME]] [[PRISM]] [[ParaView]] [[Perl]] [[Plotmtv]] [[Povray]] [[Python]]
   -              [[Questions/Réponses]] [[Radia]] [[Rheolef]] [[SLEPc]] [[SLFCFD]] [[SLFFEA]] [[SPARSE]] [[SPOOLES]] [[STEP]] [[Sage]]
   -              [[Salomé]] [[ScaLAPACK]] [[Scilab]] [[SparseLib++]] [[SuperLU]] [[TYPHON]] [[TetGen]] [[Triangle]] [[UMFPACK]] [[VRML]]
   -              [[VTK]] [[VisIt]] [[Visualisation]] [[XEmacs]] [[Y12M]] [[Yorick]] [[Z88]] [[autres_informations_utiles]] [[bamg]]
   -              [[bidirectional_reflectance_codes]] [[bilum]] [[blacs]] [[brl-cad]] [[bsp]] [[c]] [[cadna]] [[calcul]] [[calculix]]
   -              [[cast3m]] [[channelflow]] [[deal.II]] [[dolfyn]] [[featflow]] [[gotm]] [[history]] [[industrialisation]] [[jCAE]]
   -              [[libMesh]] [[liens]] [[modeles_physiques]] [[mpi]] [[ngsolve]] [[nohup]] [[opendx]] [[openfem]] [[openfoam]] [[pARMS]]
   -              [[pthreads]] [[questions_reponses_langages_compiles]] [[questions_reponses_sur_freefem]] [[reutilisation]] [[rlabplus]]
   -              [[screen]] [[trilinos]] [[uBLAS]] [[xd3d]]
   - _TODO_ [[file:::3447]] [[file:::3990]]
   - 
   - [[elisp:(alh-set-keywords)]] [[file:~/.emacs::alh-set-keywords]] [[file:~/alh/bin/headeralh]]
   - emacs-keywords brief="Free software for scientific computing" markdown nofaces start=19/10/18 top=\n written
   -->

<!--
    template       [[https://raw.githubusercontent.com/Bertbk/infomath/master/content/tools/vscode.md]]
    syntax         [[https://sourcethemes.com/academic/docs/writing-markdown-latex/]]
                   [[https://daringfireball.net/projects/markdown/syntax]]
                   [[info:m4]]
    compile
    - dev          [[elisp:(compile "make freesoft.htm")]]
                   [[file:Makefile::freesoft.htm]]
                   [[file:freesoft.htm]]
                   [[elisp:(startup-persistent-process "browseralh freesoft.htm")]]
                   [[man:pandoc]]
    - infomath     [[elisp:(compile "m4 -DINFOMATH=1 freesoft.m4 > ~/infomath/content/tmp/free_software_for_scientific_computing.md")]]
                   [[file:~/infomath/content/tmp/free_software_for_scientific_computing.md]]
    Nombre de ##   [[shell:grep '^## ' freesoft.md|wc -l]]
-->



L'objectif de cette page est de mettre en valeur les interactions possibles entre les logiciels numériques gratuits disponibles sur
internet. Ceci afin de les connecter entre eux dans la chaîne de développement informatique. La description de chaque logiciel est succincte
(voyez les [liens vers d'autres listes de logiciels](#liens) pour des descriptions plus détaillées) mais une attention spéciale a été
réservée aux formats de données qui peuvent servir d'interface. Un format de données est cité s'ils est décrit par la documentation du
logiciel et suffisamment standard pour servir d'interface avec d'autres outils.

Cette page est produite au [Laboratoire Jacques-Louis Lions](http://www.ljll.math.upmc.fr) de [Sorbonne
Université](http://www.sorbonne-universite.fr), mais beaucoup de logiciels cités ne sont ni développés ni maintenus au Laboratoire. La seule
référence officielle est la documentation de chaque logiciel. Merci de prévenir [Antoine Le Hyaric](http://www.ljll.math.upmc.fr/lehyaric)
si vous notez une imprécision.

## Categories

* [CAD Design](#CAD)
* [Mesh generation](#Meshing)
* [Modèles Physiques](#modeles_physiques) 
* [Calcul](#calcul) 
* [Visualisation](#visualisation)
* [Industrialisation](#industrialisation)
* [Réutilisation](#reutilisation)
* [Autres Informations](#autres_informations_utiles)
* [Liens vers d'autres listes de logiciels](#liens)

<p>&nbsp;</p>

<!-- <<<CAD>>> -->
## <a name="CAD"></a> CAD Design

> [Ayam](#ayam), [Blender](#blender), [BRL-CAD](#brl_cad), [Gmsh](#gmsh), [jCAE](#jcae), [Méfisto](#maofisto),
> [Salomé](#salome), [Wings 3D](#wings_3d)

<p>&nbsp;</p>

<!-- <<<Meshing>>> -->
## <a name="Meshing"></a> Mesh generation

*  Construire un maillage 2D : [Bamg](#bamg), [GRUMMP](#grummp), [Triangle](#triangle)
*  Construire un maillage 3D (surfaces &amp; volumes) : [Gmsh](#gmsh), [GNU Triangulated Surface Library](#gnu_triangulated_surface_library), [GRUMMP](#grummp), [jCAE](#jcae), [Méfisto](#maofisto), [Netgen](#netgen), [Salomé](#salome), [TetGen](#tetgen)
*  [Trouver un maillage gratuit](#free_meshes)
*  Réparation de maillage : [ADMesh](#admesh)
*  Partitionnement de maillage : [METIS](#metis)

<p>&nbsp;</p>

<!-- <<<modeles_physiques>>> -->
## <a name="modeles_physiques"></a> Modélisation de Phénomènes Physiques

*  Multi-physiques : [Elmer](#elmer), [FElt](#felt), [Méfisto](#maofisto), [NGSolve](#ngsolve), [OOFEM](#oofem), [OpenFOAM](#openfoam), [TYPHON](#typhon)
*  Dynamique des fluides : [Channelflow](#channelflow), [Code_Saturne](#code_saturne), [dolfyn](#dolfyn), [FEATFLOW](#featflow), [Gerris Flow Solver](#gerris_flow_solver), [ISAAC](#isaac), [NSC2KE](#nsc2ke), [SLFCFD](#slfcfd)
*  Electromagnétisme : [Bidirectional Reflectance Codes](#bidirectional_reflectance_codes), [EMAP](#emap), [FEMM](#femm), [GetDP](#getdp), [Radia](#radia)
*  Mécanique des structures : [CalculiX](#calculix), [Cast3M](#cast3m), [Code_Aster](#code_aster), [FEniCS](#fenics), [Impact](#impact), [SLFFEA](#slffea), [Z88](#z88)
*  Dynamique des solides rigides : [Open Dynamics Engine](#open_dynamics_engine)
*  Géophysique : [GETM](#getm), [GOTM](#gotm), [OpenSees](#opensees)

<p>&nbsp;</p>

<!-- <<<calcul>>> -->
## <a name="calcul"></a> Logiciels et Bibliothèques de Calcul Numérique

*  Méthode des éléments finis : [deal.II](#deal_ii), [Feel++](#feel), [FEniCS](#fenics), [FreeFEM++](#freefem), [FreeFEM++-cs](#freefem_cs),
   [Getfem++](#getfem), [libMesh](#libmesh), [Mélina](#maolina), [OFELI](#ofeli), [OpenFEM](#openfem), [Rheolef](#rheolef)
*  Eléments finis discontinus : [FreeFEM++](#freefem), [Sledge++](#sledge)
*  Langages mathématiques : [Maxima](#maxima), [Octave](#octave), [PARI/GP](#pari_gp), [rlabplus](#rlabplus), [Sage](#sage), [Scilab](#scilab), [Yorick](#yorick)
*  Bibliothèques scientifiques tous usages : [Boost](#boost), [GNU Scientific Library](#gnu_scientific_library),
   [NumPy](https://www.projet-plume.org/fiche/numpy), [POOMA](#pooma), [SciPy](http://www.scipy.org), [Trilinos](#trilinos)
*  Solveurs linéaires : [BILUM](#bilum), [Hypre](#hypre), [IML++](#iml), [ITPACK](#itpack), [LAPACK](#lapack), [MUMPS](#mumps),
   [NAPACK](#napack), [pARMS](#parms), [PETSc](#petsc), [PLAPACK](#plapack), [ScaLAPACK](#scalapack), [SPARSE](#sparse),
   [SuperLU](#superlu), [SPOOLES](#spooles), [UMFPACK](#umfpack), [Y12M](#y12m)
*  Valeurs et vecteurs propres : [ARPACK](#arpack), [NAPACK](#napack), [PRIMME](#primme), [PRISM](#prism), [SLEPc](#slepc)
*  Algèbre linéaire : [Atlas](#atlas), [BLAS](#blas), [Blitz++](#blitz), [FLAME](#flame), [NIST Sparse BLAS](#nist_sparse_blas),
   [OpenBLAS](http://xianyi.github.io/OpenBLAS), [PBLAS](#pblas), [SparseLib++](#sparselib), [uBLAS](#ublas)
*  Transformées de Fourier : [FFTW](#fftw)
*  Problèmes d&#039;arrondi arithmétique : [CADNA](#cadna), [GNU Multiple Precision Arithmetic Library](http://gmplib.org/)
*  Modèles de programmation parallèle : [BLACS](#blacs), [BSP](#bsp), [Cilk](#cilk), [MPI](#mpi), [OpenMP](#openmp), [Pthreads](#pthreads)

<p>&nbsp;</p>

<!-- <<<industrialisation>>> -->
## <a name="industrialisation"></a> Industrialisation et Génie Logiciel

* Gestion des versions : [Mercurial](#mercurial), [Git](http://fr.wikipedia.org/wiki/Git)
* Configuration : [Automake](#automake), [GNU Make](#gnu_make), [Libtool](#libtool)
* Documentation : [Doxygen](#doxygen), HTML, [LaTeX](#latex) 
* [Licences pour logiciels libres](#licences_pour_logiciels_libres)
* De l'importance de la robustesse d'un code : [Working with the Chaos Monkey](http://www.codinghorror.com/blog/2011/04/working-with-the-chaos-#monkeyl)

<p>&nbsp;</p>

<!-- <<<autres_informations_utiles>>> -->
## <a name="autres_informations_utiles"></a> Autres Outils Utiles pour la Programmation

*  Langages compilés : [C](#c), [C++](#cxx), [Fortran](#fortran) 
*  Langages interprétés : [Perl](#perl), [Python](#python)
*  Debugging : [DDD](#ddd), [GDB](#gdb)

<p>&nbsp;</p>

<!-- <<<liens>>> -->
## <a name="liens"></a> Liens vers d'autres listes de logiciels

* [Finite element analysis - Wikipedia, the free encyclopedia](http://en.wikipedia.org/wiki/Finite_element_analysis)
* [Matrix Market : A visual repository of test data for use in comparative studies of algorithms for numerical linear algebra, featuring nearly 500 sparse matrices from a variety of applications, as well as matrix generation tools and services](http://math.nist.gov/MatrixMarket/)
* [Free Mechanical Engineering Software](http://www.freebyte.com/cad/)
* [Netlib Repository](http://www.netlib.org/)
* [Jack Dongarra's survey : Freely available software for linear algebra on the web](http://www.netlib.org/utk/people/JackDongarra/la-#swl)
* [polymorphe.org: Ce site regroupe de nombreuses archives portant sur divers domaines de l'informatique, les cours que vous pourrez trouver ici sont sous divers formats : doc, html, pdf, ps mais d'autres sont egalement compresses au format rar](http://www.polymorphe.org/)
* [Convert: Bridging the Scientific Data Format Chasm](http://www.adass.org/adass/proceedings/adass94/#jenningsdl) (1995)
* [website dedicated to numerical analysis by Jean-Pierre Moreau](http://perso.wanadoo.fr/jean-pierre.moreau)
* [Overview of Iterative Linear System Solver Packages, Victor Eijkhout, 15 August, 1997](http://www.netlib.org/utk/papers/iterative-survey/)
* [Solutions informatiques sur Internet - Page maintenue par : Alex ZAÏMI](http://zaimi.free.fr/informatique/#indexl) (2005)

<p>&nbsp;</p>

---

<p>&nbsp;</p>

<!-- <<<3D-Studio>>> -->
## <a name="3D-Studio"></a> 3D-Studio

> "*This document describes the file format of the 3ds files generated by 3d-studio by Autodesk.*"

### Web

[http://www.dcs.ed.ac.uk/home/mxr/gfx/3d/3DS.spec](http://www.dcs.ed.ac.uk/home/mxr/gfx/3d/3DS.spec)

<p>&nbsp;</p>

<!-- <<<ADMesh>>> -->
## <a name="ADMesh"></a> ADMesh

> "*ADMesh is a program for processing triangulated solid meshes. Currently, ADMesh only reads the [STL file format](#stl_file_format)
> that is used for rapid prototyping applications, although it can write [STL](#stl_file_format), [VRML](#vrml), [OFF](#off), and
> [DXF (voir AutoCAD)](#autocad_dxf) files.*"

### Features

* Read and write binary and **ASCII** [STL](#stl_file_format) files
* Check [STL](#stl_file_format) files for flaws (i.e. unconnected facets, bad normals)
* Repair facets by connecting nearby facets that are within a given tolerance
* Fill holes in the mesh by adding facets.
* Repair normal directions (i.e. facets should be CCW)
* Repair normal values (i.e. should be perpendicular to facet with length=1)
* Remove degenerate facets (i.e. facets with 2 or more vertices equal)
* Translate in x, y, and z directions
* Rotate about the x, y, and z axes
* Mirror about the xy, yz, and xz planes
* Scale the part by a factor
* Merge 2 [STL](#stl_file_format) files into one
* Write an [OFF](#off) file
* Write a [VRML](#vrml) file
* Write a [DXF (voir AutoCAD)](#autocad_dxf) file
* Calculate the volume of a part

### Web

[http://www.varlog.com](http://www.varlog.com)

### Licence

[GPL](#licences_pour_logiciels_libres)

### Format de données standard lus

[STL file format](#stl_file_format)

### Format de données standard écrits

[STL file format](#stl_file_format), [VRML](#vrml), [OFF](#off), [DXF](#autocad_dxf)

<p>&nbsp;</p>

<!-- <<<ARPACK>>> -->
## <A NAME="ARPACK"></A> ARPACK

> "*ARPACK++ is an object-oriented version of the ARPACK package. ARPACK is a well known collection of [Fortran](#fortran) subroutines
> designed to compute a few eigenvalues and eigenvectors of large scale sparse matrices and pencils. It implements a variant of the Arnoldi
> process for finding eigenvalues called Implicit restarted Arnoldi method (IRAM) and is capable of solving a great variety of problems from
> single precision positive definite symmetric problems to double precision complex non-Hermitian generalized problems.*

> *ARPACK++ is a collection of classes that offers [C++](#c) programmers an interface to ARPACK. It preserves the full capability,
> performance, accuracy and low memory requirements of the [Fortran](#fortran) package, but takes advantage of the [C++](#c)
> object-oriented programming environment.*
	    
> *ARPACK is a collection of [Fortran](#fortran) 77 subroutines designed to solve large scale eigenvalue problems.*

> *The package is designed to compute a few eigenvalues and corresponding eigenvectors of a general n by n matrix A. It is most appropriate
> for large sparse or structured matrices A where structured means that a matrix-vector product w ← Av requires order n rather than the
> usual order n2 floating point operations. This software is based upon an algorithmic variant of the Arnoldi process called the Implicitly
> Restarted Arnoldi Method (IRAM). When the matrix A is symmetric it reduces to a variant of the Lanczos process called the Implicitly
> Restarted Lanczos Method (IRLM). These variants may be viewed as a synthesis of the Arnoldi/Lanczos process with the Implicitly Shifted QR
> technique that is suitable for large scale problems. For many standard problems, a matrix factorization is not required. Only the action
> of the matrix on a vector is needed.*

> *ARPACK software is capable of solving large scale symmetric, nonsymmetric, and generalized eigenproblems from significant application
> areas. The software is designed to compute a few (k) eigenvalues with user specified features such as those of largest real part or
> largest magnitude. Storage requirements are on the order of n.k locations. No auxiliary storage is required. A set of Schur basis vectors
> for the desired k-dimensional eigen-space is computed which is numerically orthogonal to working precision. Numerically accurate
> eigenvectors are available on request.*

> *PARPACK (Parallel ARPACK) is an extension of the ARPACK software package used for solving large scale eigenvalue problems on distributed
> memory parallel architectures.  The message passing layers currently supported are [BLACS](#blacs) and [MPI](#mpi).*"
	    
[https://en.wikipedia.org/wiki/ARPACK](https://en.wikipedia.org/wiki/ARPACK)

<p>&nbsp;</p>

<!-- <<<Atlas>>> -->
## <a name="Atlas"></a> Atlas

> "*The ATLAS (Automatically Tuned Linear Algebra Software) project is an ongoing research effort focusing on applying empirical techniques
> in order to provide portable performance. At present, it provides [C](#c) and [Fortran](#fortran) 77 interfaces to a portably
> efficient [BLAS](#blas) implementation, as well as a few routines from [LAPACK](#lapack).*"

### Web

[http://math-atlas.sourceforge.net/](http://math-atlas.sourceforge.net/)

### Documentation

**FAQ** : [http://math-atlas.sourceforge.net/#faql](http://math-atlas.sourceforge.net/#faql)

<p>&nbsp;</p>

<!-- <<<AutoCAD DXF>>> -->
## <a name="AutoCAD DXF"></a> AutoCAD DXF

(il ne s&#039;agit pas ici du logiciel commercial AutoCAD mais du format de ses fichiers car ils sont compris par beaucoup d&#039;autres
logiciels)

"*Drawing Interchange Format (DXF) files enable the interchange of drawings between AutoCAD and other programs. DXF files can be either
**ASCII** or binary formats.*"

### Documentation

[http://www.autodesk.com/techpubs/autocad/acad2000/dxf/#index](http://www.autodesk.com/techpubs/autocad/acad2000/dxf/#index)

### Logiciels capables d&#039;écrire dans ce format

[ADMesh](#admesh)

<p>&nbsp;</p>

<!-- <<<Automake>>> -->
## <a name="Automake"></a> Automake

"* Automake is a tool for automatically generating &#039;Makefile.in&#039; files compliant with the GNU Coding Standards. Automake requires
the use of GNU Autoconf.*"

### Web

[http://www.gnu.org/software/automake/](http://www.gnu.org/software/automake/)

### Documentation

[http://www.gnu.org/software/automake/manual/html_node/#indexl](http://www.gnu.org/software/automake/manual/html_node/#indexl)

<p>&nbsp;</p>

<!-- <<<Ayam>>> -->
## <a name="Ayam"></a> Ayam

"*Ayam is a free (as in free speech, [BSD-licensed](#licences_pour_logiciels_libres)) 3D modelling environment for the RenderMan
interface. Free means that neither the author nor any contributors make money out of this software. We need your (yes your!) feedback to
keep this project alive. If you use Ayam, please submit your pictures, bug reports, or feature requests.*"

"*Ayam currently runs on Unix (Linux, IRIX, FreeBSD tested), Win32 (Win95-Win2000, XP), and Mac **OS** X (Aqua and X11)*"

"*Ayam features at a glance :*"

*   RIB (RenderMan Interface Bytestream) export and import.
*   Support for NURBS curves and (trimmed) NURBS surfaces, Boxes, Quadrics (Sphere, Disk, Cylinder, Cone, Hyperboloid, Paraboloid, and
    Torus), CSG, MetaBalls, Patch Meshes, Polygonal Meshes, and Subdivision Surfaces.
*   NURBS modelling includes normal and interpolating curves as well as extrude, revolve, sweep, birail, skin and gordon objects with caps, holes, and bevels.
*   Custom objects that may freely implement their representations (using OpenGL and RIB) and even small GUIs to edit their type specific
    parameters may be written by the user and dynamically loaded at runtime.
*   Scripting interface: Tcl.
*   Misc: instancing, arbitrary number of modeling views, object clipboard, independent property clipboard, console, n-level undo.

*  Web: [http://ayam.sourceforge.net/](http://ayam.sourceforge.net/)
*  Documentation: [http://ayam.sourceforge.net/#docsl](http://ayam.sourceforge.net/#docsl)
*  Téléchargement: [http://ayam.sourceforge.net/#downloadl](http://ayam.sourceforge.net/#downloadl)
*  Exemples: [http://ayam.sourceforge.net/#galleryl](http://ayam.sourceforge.net/#galleryl)
*  Licence: "*[BSD-licensed](#licences_pour_logiciels_libres)*"

<p>&nbsp;</p>

<!-- <<<bamg>>> -->
## <a name="bamg"></a> Bamg
	  
"*Bamg est un générateur de maillages bidimensionnels isotropes ou anisotopes. Ce générateur permet, soit de construire un maillage à partir
d&#039;une géométrie, soit de construire un maillage adapté à partir d&#039;un maillage précédent et d&#039;une solution ou d&#039;une
métrique. Il permet aussi d&#039;interpoler sur le maillage créé des solutions P1 définies sur le maillage précédent.*

*Une géométrie est définie par un maillage de contours : liste de sommets, liste d&#039;arêtes, plus des informations de continuité
G1. Cette géométrie peut être construite avec EMC2 et en traduisant le fichiers de maillage avec le petit utilitaire cvmsh2 qui est
inclus.*"

*  Auteur(s): Frédéric Hecht
*  Format de données standard écrits: .am .am_fmt .amdba .nopo (Modulef, [NSC2KE](#nsc2ke), [xd3d](#xd3d)), .mesh ([FreeFEM++](#freefem))
*  Logiciels capables de lire ce format: [Rheolef](#rheolef)
    
<p>&nbsp;</p>

<!-- <<<bidirectional_reflectance_codes>>> -->
## <a name="bidirectional_reflectance_codes"></a> Bidirectional Reflectance Codes

"*This webpage provides access to two collections of [FORTRAN](#fortran) codes.*

*The first one can be used to compute the (scalar) bidirectional reflectance of a semi-infinite homogeneous slab composed of arbitrarily
shaped, randomly oriented particles based on a rigorous numerical solution of the radiative transfer equation.*

*The second one can be used to compute the Stokes reflection matrix of a rough interface separating two homogeneous half-spaces with
different refractive indices (e.g., a rough ocean surface).*"

<p>&nbsp;</p>

<!-- <<<bilum>>> -->
## <A NAME="bilum"></A> BILUM

"*BILUM is a set of programs designed for solving general sparse linear systems by using Krylov subspace methods preconditioned by some
multi-level block ILU (BILUM) preconditioning techniques. BILUM combines the benefits of generality and robustness of ILU preconditioning
techniques with those of grid-independent convergence of multigrid methods. The multi-level algorithms implemented by BILUM are based on the
block independent set ordering and multi-elimination techniques. At each level, a block independent set is found by some greedy algorithms
such that each block is decoupled with other blocks in the independent set. There is an inherited parallelism associated with this
technique. The coefficient matrix is then re-ordered according to the independent set ordering and an approximate block ILU factorization is
performed with a reduced system of smaller size. The multi-level structure is constructed by recursively applying the above idea to the
approximate Schur complement (the reduced system) until the last reduced system is small enough to be solved by a direct method or a
preconditioned iterative method.*"

### Web

[http://www.cs.uky.edu/~jzhang/#biluml](http://www.cs.uky.edu/~jzhang/#biluml)

### Téléchargement

[http://www.cs.uky.edu/~jzhang/bilum/bilum.tar.gz](http://www.cs.uky.edu/~jzhang/bilum/bilum.tar.gz)

### Licence

"*This is a preliminary examination version of BILUM. Permission is granted for using the software for the purpose of examination. Users are
not permitted to distribute the software. This software package comes with no warranty. The authors are not liable for any loss/damage or
inconvenience caused in the use of this software package or any modification thereof. You use it at your own risk.*"

### Autres indications

Written in [Fortran](#fortran).

<p>&nbsp;</p>

<!-- <<<blacs>>> -->
## <A NAME="blacs"></A> BLACS

"*The BLACS (Basic Linear Algebra Communication Subprograms) project is an ongoing investigation whose purpose is to create a linear algebra
oriented message passing interface that may be implemented efficiently and uniformly across a large range of distributed memory platforms.*

*The length of time required to implement efficient distributed memory algorithms makes it impractical to rewrite programs for every new
parallel machine. The BLACS exist in order to make linear algebra applications both easier to program and more portable. It is for this
reason that the BLACS are used as the communication layer of [ScaLAPACK](#scalapack).*"

### Web

[http://www.netlib.org/blacs/](http://www.netlib.org/blacs/)

### Documentation

[http://www.netlib.org/blacs/BLACS/QR#efl](http://www.netlib.org/blacs/BLACS/QR#efl)

### Exemples

[http://www.netlib.org/blacs/BLACS/E#xamplesl](http://www.netlib.org/blacs/BLACS/E#xamplesl)

<p>&nbsp;</p>

<!-- <<<BLAS>>> -->
## <A NAME="BLAS"></A> BLAS

"*The BLAS (Basic Linear Algebra Subprograms) are high quality “building block” routines for performing basic vector and matrix
operations. Level 1 BLAS do vector-vector operations, Level 2 BLAS do matrix-vector operations, and Level 3 BLAS do matrix-matrix
operations. Because the BLAS are efficient, portable, and widely available, they&#039;re commonly used in the development of high quality
linear algebra software, LINPACK and [LAPACK](#lapack) for example.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/blas-basic-linear-algebra-subprograms)

### Documentation

[http://www.netlib.org/blas/#faql](http://www.netlib.org/blas/#faql)

### Autres indications

The BLAS have to be optimized for each particular hardware architecture. If you do not know where to find such an optimized version the BLAS, see [Atlas](#atlas) or the [GNU Scientific Library](#gnu_scientific_library).

<p>&nbsp;</p>

<!-- <<<Blender>>> -->
## <a name="Blender"></a> Blender

"*Blender is the open source software for 3D modeling, animation, rendering, post-production, interactive creation and playback.*"

### Web

[http://blender.org](http://blender.org)

### Téléchargement

[http://www.blender.org/download/get-blender](http://www.blender.org/download/get-blender)

### Licence

"*Available for all major operating systems under the [GNU General Public License](#licences_pour_logiciels_libres).*"

<p>&nbsp;</p>

<!-- <<<Blitz++>>> -->
## <a name="Blitz++"></a> Blitz++

"*Blitz++ is a [C++](#c) class library for scientific computing which provides performance on par with [Fortran](#fortran) 77/90. It uses
template techniques to achieve high performance. The current versions provide dense arrays and vectors, random number generators, and small
vectors and matrices. Blitz++ is distributed freely under an open source license, and contributions to the library are welcomed.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/blitz)

<p>&nbsp;</p>

<!-- <<<Boost>>> -->
## <a name="Boost"></a> Boost

"*Boost provides free peer-reviewed portable [C++](#c) source libraries.*

*We emphasize libraries that work well with the C++ Standard Library. Boost libraries are intended to be widely useful, and usable across a
broad spectrum of applications. The Boost license encourages both commercial and non-commercial use.*

*We aim to establish “existing practice” and provide reference implementations so that Boost libraries are suitable for eventual
standardization. Ten Boost libraries are already included in the C++ Standards Committee&#039;s Library Technical Report (TR1) as a step
toward becoming part of a future C++ Standard. More Boost libraries are proposed for the upcoming TR2.*

*Getting started: Boost works on almost any modern operating system, including UNIX and Windows variants. Follow the Getting Started Guide
to download and install Boost. Popular Linux and Unix distributions such as Fedora, Debian, and NetBSD include pre-built Boost
packages. Boost may also already be available on your organization&#039;s internal web server.*"

### Web

[http://www.boost.org](http://www.boost.org)

### Documentation

[http://www.boost.org/more/getting_started/#indexl](http://www.boost.org/more/getting_started/#indexl),

[http://www.boost.org/libs/#libraries](http://www.boost.org/libs/#libraries)

### Téléchargement

[http://sourceforge.net/project/showfiles.php?group_id=7586](http://sourceforge.net/project/showfiles.php?group_id=7586)

### Licence

[http://www.boost.org/more/#license_infol](http://www.boost.org/more/#license_infol)

<p>&nbsp;</p>

<!-- <<<brl-cad>>> -->
## <A NAME="brl-cad"></A> BRL-CAD

"*The BRL-CAD package is a powerful Constructive Solid Geometry (CSG) solid modeling system with over 20 years development and production
use by the U.S. military. BRL-CAD includes an interactive geometry editor, parallel ray-tracing support for rendering and geometric
analysis, path-tracing for realistic image synthesis, network distributed framebuffer support, image-processing and signal-processing
tools.*"

### Web

[http://www.brlcad.org](http://www.brlcad.org)

### Documentation

[http://brlcad.org/wiki/Documentation](http://brlcad.org/wiki/Documentation)

### Téléchargement

[http://brlcad.org/d/download](http://brlcad.org/d/download)

### Licence

"*The entire package is distributed in source code form.*"

<p>&nbsp;</p>

<!-- <<<bsp>>> -->
## <A NAME="bsp"></A> BSP

"*Parallel programmers looking for a simple but efficient approach to developing scalable applications software may be interested in the
BSPlib programming library. BSPlib is an alternative to [MPI](#mpi) and PVM, and is based on the BSP model of parallel computation. It is
already being used by a rapidly growing community of software developers in universities and in industry.*

*BSPlib can be used with [C](#c), [C++](#c), or [Fortran](#fortran). It supports SPMD parallelism based on efficient one-sided
communications. The core library (excluding collective communications) consists of just 20 primitives.*"

### Web

[http://www.bsp-worldwide.org/implmnts/oxtool/](http://www.bsp-worldwide.org/implmnts/oxtool/)

### Documentation

[http://www.bsp-worldwide.org/implmnts/oxtool/man/](http://www.bsp-worldwide.org/implmnts/oxtool/man/)

### Autres indications

See also [MPI](#mpi).

<p>&nbsp;</p>

<!-- <<<cadna>>> -->
## <A NAME="cadna"></A> CADNA

"*… the CADNA library … allows to estimate the round-off error propagation on every scientific code written in FORTRAN language.*"

*  Web: [http://www.lip6.fr/cadna](http://www.lip6.fr/cadna)

<p>&nbsp;</p>

<!-- <<<calculix>>> -->
## <a name="calculix"></a> CalculiX

"*CalculiX is a package designed to solve field problems. The method used is the finite element method.*

*With CalculiX Finite Element Models can be build, calculated and post-processed. The pre- and post-processor is an interactive 3D-tool
using the OpenGL **API**. The solver is able to do linear and non-linear calculations. Static, dynamic and thermal solutions are
available. Both programs can be used independently. Because the solver makes use of the abaqus input format it is possible to use commercial
pre-processors as well. In turn the pre-processor is able to write mesh related data for nastran, abaqus, ansys, [code-aster](#code_aster)
and for the free-cfd codes duns, [ISAAC](#isaac) and [OpenFOAM](#openfoam). A vda CAD interface is available. The program is designed to run
on Unix platforms like Linux and Irix computers but also on MS-Windows.*

*The CalculiX package was developed by a team of enthusiasts in their raw spare time. They are employees of MTU Munich, an
Aero Engine manufacturer in Germany which granted the publication.*"
	    
[https://fr.wikipedia.org/wiki/Calculix](https://fr.wikipedia.org/wiki/Calculix)

<p>&nbsp;</p>

<!-- <<<cast3m>>> -->
## <a name="cast3m"></a> Cast3M

"*CASTEM 2000 est un code de calcul pour l'analyse de structures par la méthode des éléments finis. Ce code a été développé par le
Département Mécanique et Technologie (DMT) du Commissariat français à l'Energie Atomique (CEA).*

*Le développement de CASTEM 2000 entre dans le cadre d'une activité de recherche dans le domaine de la mécanique dont le but est de
définir un instrument de haut niveau, pouvant servir de support pour la conception, le dimensionnement et l'analyse de structures et de
composants, dans le domaine du nucléaire comme dans le secteur industriel classique.*

*Dans cette optique, CASTEM 2000 intègre non seulement les processus de calculs proprement dits mais également les fonctions de construction
du modèle (pré-processeur) et les fonctions de traitement des résultats (post-traitement). CASTEM 2000 est un programme que
l'utilisateur peut adapter à ses besoins pour résoudre ses propres problèmes.*"

[http://www-cast3m.cea.fr](http://www-cast3m.cea.fr)

<p>&nbsp;</p>

<!-- <<<channelflow>>> -->
## <a name="channelflow"></a> Channelflow

"*Channelflow is a software system for direct spectral simulation of incompressible Navier-Stokes flow in channel geometries, witten in
[C++](#c). Channelflow is not innovative as an algorithm. Rather, Channelflow uses relatively modern software design to improve the
usability, flexibility, and intelligibility of a well-known algorithm. The goals of Channelflow are*

* *to lower the barrier to entry to computational fluid dynamics*
* *to make CFD research codes short, readable, and easily modifiable*"

### Web

[http://www.cns.gatech.edu/channelflow/](http://www.cns.gatech.edu/channelflow/)

### Documentation

[http://www.cns.gatech.edu/channelflow/documentation/#indexl](http://www.cns.gatech.edu/channelflow/documentation/#indexl)

### Téléchargement

[http://www.cns.gatech.edu/channelflow/download](http://www.cns.gatech.edu/channelflow/download)

### Licence

"*Channelflow is free software. It is licensed under the [GNU GPL](#licences_pour_logiciels_libres) version 2 and available for download.*"

<p>&nbsp;</p>

<!-- <<<c>>> -->
## <a name="c"></a> C

C est un langage de programmation généraliste, de même que [C++](#cxx) et [Fortran](#fortran).

Référence : [Anglais](http://www.acm.uiuc.edu/webmonkeys/book/c_guide/)

[Questions/Réponses de programmation](#questions_reponses_langages_compiles)

### Questions/Réponses

#### La syntaxe de printf()

[http://www.cplusplus.com/reference/clibrary/cstdio/printf](http://www.cplusplus.com/reference/clibrary/cstdio/printf)

<p>&nbsp;</p>

<!-- <<<Cilk>>> -->
## <a name="Cilk"></a> Cilk

"*Cilk is a language for multithreaded parallel programming based on [ANSI C](#c). Cilk is designed for general-purpose parallel programming, but it is especially effective for exploiting dynamic, highly asynchronous parallelism, which can be difficult to write in data-parallel or message-passing style. Using Cilk, our group has developed three world-class chess programs, StarTech, *Socrates, and Cilkchess. Cilk provides an effective platform for programming dense and sparse numerical algorithms, such as matrix factorization and N-body simulations, and we are working on other types of applications. Unlike many other multithreaded programming systems, Cilk is algorithmic, in that the runtime system employs a scheduler that allows the performance of programs to be estimated accurately based on abstract complexity measures.*"

### Web

[http://supertech.lcs.mit.edu/cilk/](http://supertech.lcs.mit.edu/cilk/)

<p>&nbsp;</p>

<!-- <<<Code_Aster>>> -->
## <a name="Code_Aster"></a> Code_Aster

"*Code_Aster propose, bien au delà des fonctionnalités standard d'un code de calcul thermo-mécanique, toute une panoplie de méthodes d'analyse et de modélisations multiphysiques : de l'analyse sismique aux milieux poreux en passant par l'acoustique, la fatigue, la dynamique stochastique… Ses modélisations, ses algorithmes et ses solveurs ont gagné en robustesse et en complétude (1000000 lignes de codes, 200 opérateurs). Résolument ouvert, il est chaîné, couplé et encapsulé de mille façons. Bref, l'utilisateur n'a que l'embarras du choix !*"

[http://www.code-aster.org](http://www.code-aster.org)

<p>&nbsp;</p>

<!-- <<<Code_Saturne>>> -->
## <a name="Code_Saturne"></a> Code_Saturne

"*Code_Saturne® is EDF's general purpose computational fluid dynamics software. Developed since 1997 at EDF R&amp;D, it is based on a co-located Finite Volume approach that accepts meshes with any type of cell (tetrahedral, hexahedral, prismatic, pyramidal, polyhedral…) and any type of grid structure (unstructured, block structured, hybrid, conforming or with hanging nodes…).

Its basic capabilities enable the handling of either incompressible or expandable flows with or without heat transfer and turbulence (mixing length, 2-equation models, v2f, Reynolds stress models, Large Eddy Simulations…).

Dedicated modules are available for specific physics such as radiative heat transfer, combustion (gas, coal…), magneto-hydro dynamics, compressible flows, two-phase flows (Euler-Lagrange approach with two-way coupling), extensions to specific applications (e.g.  for atmospheric environment: code Mercure_Saturne).

 Code_Saturne can be coupled to EDF's thermal software Syrthes.  It can also be used jointly with EDF's structural analysis software [Code_Aster](#code_aster), in particular in the [Salomé](#salome) platform.

Parallel code coupling capabilities are provided by the FVM library (EDF's “Finite Volume Mesh” library, under [LGPL](#licences_pour_logiciels_libres) licence).*"

[Fiche PLUME](http://www.projet-plume.org/fiche/codesaturne)

### Format de données standard lus

"*De nombreux mailleurs sont compatibles avec Code_Saturne, entre autres [I-DEAS®](#i_deas_file_format), [GMSH](#gmsh), Gambit®, Simail®, [Salomé](#salome), Harpoon®, ICEM®, …*"

### Format de données standard écrits

"*Les sorties de posttraitement sont disponibles aux formats EnSight®, CGNS et [MED_fichier](#salome), avec des fonctionnalités avancées offertes par la librairie FVM (librairie « Finite Volume Mesh » développée par EDF sous licence [LGPL](#licences_pour_logiciels_libres)).  La librairie FVM offre aussi des possibilités de couplage de codes en parallèle.*"

<p>&nbsp;</p>

<!-- <<<Conversion des fichiers texte>>> -->
## <a name="Conversion des fichiers texte"></a> Conversion des fichiers texte

Les systèmes Linux, Windows et MacOS ne traitent pas les fichiers textes de la même façon :

<ul>
<li > sur Linux, chaque ligne se termine par le caractère <strong>0x0d</strong>
</li>
<li > sur Windows : <strong>0x0d 0x0a</strong>
</li>
<li > sur MacOS (et anciennement SunOS) : <strong>0x0a</strong>
</li>
</ul>

### sed

Plusieurs éditeurs (par exemple [Emacs](#emacs)) sont capables de traduire les lignes d'un système à l'autre. Mais on peut aussi utiliser
les commandes suivantes sous Linux ou MacOS :

<ul>
*  De Windows vers Linux :

</ul>
<pre >sed 's/\x0d\x0a/\x0d/g' windows.txt &gt; linux.txt</pre>
<ul>
*  De MacOS vers Linux :

</ul>
<pre >sed 's/\x0a/\x0d/g' macos.txt &gt; linux.txt</pre>

### Emacs
<pre >M-x set-buffer-file-coding-system RET undecided-unix RET C-x C-s</pre>

<p>&nbsp;</p>

<!-- <<<CUDA>>> -->
## <A NAME="CUDA"></A> CUDA

Au laboratoire, CUDA est disponible sur <strong>gpu1</strong>, <strong>gpu2</strong> et <strong>tesla</strong>. CUDA est une technologie
propriétaire développée par la société [NVidia](http://www.nvidia.fr). La technologie alternative
[OpenCL](http://fr.wikipedia.org/wiki/OpenCL) est moins dépendante d'une société mais aussi moins mature actuellement.

[Introduction à CUDA](http://tcuvelier.developpez.com/tutoriels/gpgpu/cuda/introduction)

[Description de CUDA sur Wikipedia](http://fr.wikipedia.org/wiki/Compute_Unified_Device_Architecture)

<p>&nbsp;</p>

<!-- <<<C++>>> -->
## <a name="C++"></a> C++

C++ est un langage de programmation généraliste issu d'une évolution du langage [C](#c).

<ul>
*  Introduction : [Cours de C/C++](http://casteyde.christian.free.fr/cpp/cours/#indexl) (Français), [The cplusplus.com tutorial](http://www.cplusplus.com/doc/tutorial) (English)

*  Réference : [http://www.cplusplus.com/ref](http://www.cplusplus.com/ref), [http://www.cppreference.com](http://www.cppreference.com)

*  Standard Template Library (STL) : [Tutorial](http://www.cs.brown.edu/people/jak/proglang/cpp/stltut/#tutl), [Reference](http://www.sgi.com/tech/stl), [Concepts de la programmation générique](http://www.boost.org/more/#generic_programmingl)

</ul>

[Questions/Réponses de programmation](#questions_reponses_langages_compiles)

<p>&nbsp;</p>

<!-- <<<DDD>>> -->
## <A NAME="DDD"></A> DDD

"*GNU DDD is a graphical front-end for command-line debuggers such as [GDB](#gdb), DBX, WDB, Ladebug, JDB, XDB, the Perl debugger, the bash debugger, or the Python debugger. Besides “usual” front-end features such as viewing source texts, DDD has become famous through its interactive graphical data display, where data structures are displayed as graphs.*"

<ul>
*  Web: [http://www.gnu.org/software/ddd/](http://www.gnu.org/software/ddd/)

</ul>

<p>&nbsp;</p>

<!-- <<<deal.II>>> -->
## <a name="deal.II"></a> deal.II

"* deal.II is a [C++](#c) program library targeted at adaptive finite elements and error estimation. It uses state-of-the-art programming techniques of the C++ programming language to offer you a modern interface to the complex data structures and algorithms required for adaptivity and enables you to use a variety of finite elements in one, two, and three space dimensions, as well as time-dependent problems.

The main aim of deal.II is to enable development of modern finite element algorithms, using among other aspects sophisticated error estimators and adaptive meshes. Writing such programs is a non-trivial task, and successful programs tend to become very large and complex. We therefore believe that this is best done using a program library that frees the application programmer from aspects like grid handling and refinement, handling of degrees of freedom, input of meshes and output of results in graphics formats, and the like. Also, support for several space dimensions at once is included in a way such that programs can be written independent of the space dimension without unreasonable penalties on run-time and memory consumption.*"

### Web

[http://www.dealii.org/](http://www.dealii.org/)

### Documentation

[README](http://www.dealii.org/#readmel),

[Full documentation](http://www.dealii.org/developer/#indexl)

### Téléchargement

[http://www.dealii.org/download/#indexl](http://www.dealii.org/download/#indexl)

<p>&nbsp;</p>

<!-- <<<dolfyn>>> -->
## <a name="dolfyn"></a> dolfyn

"*The Open Source CFD code dolfyn is an initiative in Noord-Brabant, a Dutch province in the south of the Netherlands, particularly in the region around Eindhoven. The Eindhoven Region presents itself as Leading in technology and ranks in the top three most technological districts in Europe. The goal of dolfyn is to promote, introduce and teach the use of modern numerical simulation techniques in general and the use of Computational Fluid Dynamics (CFD) in particular.*"

### Web

[http://www.dolfyn.net/#index_enl](http://www.dolfyn.net/#index_enl)

### Documentation

[http://www.dolfyn.net/dolfyn/#installatie_enl](http://www.dolfyn.net/dolfyn/#installatie_enl),

[http://www.dolfyn.net/dolfyn/#faq_enl](http://www.dolfyn.net/dolfyn/#faq_enl)

### Téléchargement

[http://www.dolfyn.net/dolfyn/#downloads_enl](http://www.dolfyn.net/dolfyn/#downloads_enl)

### Exemples

[http://www.dolfyn.net/dolfyn/#voorbeelden_enl](http://www.dolfyn.net/dolfyn/#voorbeelden_enl)

### Autres indications

Part of the documentation is in dutch. There is also a graphical user interface for dolfyn, at

[http://www.dolfyn.net/dolfyn/#orka_enl](http://www.dolfyn.net/dolfyn/#orka_enl).

<p>&nbsp;</p>

<!-- <<<Doxygen>>> -->
## <a name="Doxygen"></a> Doxygen

"*Doxygen is a documentation system for [C++](#cxx), [C](#c), Java, IDL (Corba and Microsoft flavors) and to some extent Objective-C, PHP, C# and D.*

*It can help you in three ways:*

* *It can generate an on-line documentation browser (in HTML) and/or an off-line reference manual (in [LaTeX](#latex)) from a set of
  documented source files. There is also support for generating output in RTF (MS-Word), PostScript, hyperlinked PDF, compressed HTML, and
  Unix man pages. The documentation is extracted directly from the sources, which makes it much easier to keep the documentation consistent
  with the source code.*

* *You can configure doxygen to extract the code structure from undocumented source files. This is very useful to quickly find your way in
  large source distributions. You can also visualize the relations between the various elements by means of include dependency graphs,
  inheritance diagrams, and collaboration diagrams, which are all generated automatically.*

* *You can even 'abuse' doxygen for creating normal documentation (as I did for this manual).*

*Doxygen is developed under Linux, but is set-up to be highly portable. As a result, it runs on most other Unix flavors as
well. Furthermore, executables for Windows 9x/NT and Mac **OS** X are available.*"

### Web

[http://www.stack.nl/~dimitri/doxygen/](http://www.stack.nl/~dimitri/doxygen/)

### Documentation

[Manual](http://www.stack.nl/~dimitri/doxygen/#manuall),

[FAQ](http://www.stack.nl/~dimitri/doxygen/#faql)

### Licence

"*Permission to use, copy, modify, and distribute this software and its documentation under the terms of the [GNU General Public License](#licences_pour_logiciels_libres) is hereby granted. No representations are made about the suitability of this software for any purpose. It is provided “as is” without express or implied warranty. See the [GNU General Public License](#licences_pour_logiciels_libres) for more details. Documents produced by doxygen are derivative works derived from the input used in their production; they are not affected by this license.*"

<p>&nbsp;</p>

<!-- <<<Elmer>>> -->
## <a name="Elmer"></a> Elmer

"*Elmer is an open-source computational tool for multi-physics problems. It has been developed in collaboration with Finnish universities,
research laboratories and industry.*

- *Elmer includes physical models of fluid dynamics, structural mechanics, electromagnetics and heat transfer. These are described by
  partial differential equations which Elmer solves by the Finite Element Method (FEM).*

- *Elmer comprises of several different parts: The geometry, boundary conditions and physical models are defined in ElmerFront. The
  resulting problem definition is solved by ElmerSolver. Finally the results are visualized by ElmerPost. Additionally a utility ElmerGrid
  may be used for simple mesh manipulation.*

- *The different parts of Elmer software may also be used independently. The strongest of the components is ElmerSolver which includes many
  sophisticated features. For pre- and postprosessing the users may find also other alternatives.*"

*Web:* [http://www.csc.fi/elmer/](http://www.csc.fi/elmer/)

<p>&nbsp;</p>

<!-- <<<Emacs>>> -->
## <a name="Emacs"></a> Emacs

"*To quote the Emacs Manual:*

*Emacs is the extensible, customizable, self-documenting real-time display editor.*

*If this seems to be a bit of a mouthful, an easier explanation is Emacs is a text editor and more. At its core is an interpreter for Emacs
Lisp ('elisp', for short), a dialect of the Lisp programming language with extensions to support text editing. Some of the features of GNU
Emacs include:*

* *Content sensitive major modes for a wide variety of file types, from plain text to source code to **HTML** files.*
* *Complete online documentation, including a tutorial for new users.*
* *Highly extensible through the Emacs Lisp language.*
* *Support for many languages and their scripts, including all the European “Latin” scripts, Russian, Greek, Japanese, Chinese, Korean,
  Thai, Vietnamese, Lao, Ethiopian, and some Indian scripts. (Sorry, Mayan hieroglyphs are not supported.)*
* *A large number of extensions which add other functionality. The GNU Emacs distribution includes many extensions; many others are
  available separately–even a web browser*"

[Fiche PLUME](http://www.projet-plume.org/fiche/emacs)

### Documentation

Initiation : [Emacs Beginner's HOWTO](http://jeremy.zawodny.com/emacs/#emacsl), [Tutorial pour Emacs, pour le programmeur](http://www.linux-france.org/article/appli/emacs/tut/)

**FAQ** : [générale](http://www.gnu.org/software/emacs/emacs-faq.text), [Microsoft Windows](http://www.gnu.org/software/emacs/windows/#ntemacsl)

Manuel : [http://www.gnu.org/software/emacs/manual](http://www.gnu.org/software/emacs/manual)

GNU Emacs Lisp Reference Manual : [http://www.gnu.org/software/emacs/manual/#elispl](http://www.gnu.org/software/emacs/manual/#elispl)

<p>&nbsp;</p>

<!-- <<<EMAP>>> -->
## <A NAME="EMAP"></A> EMAP

"*EMAP (ElectroMagnetic Analysis Program) is a family of three-dimensional finite element modeling codes that can be used to analyze simple
3-dimensional geometries. The EMAP codes are relatively easy to learn to use and are distributed in source code form.*

*The EMAP codes are not intended to compete with commercial finite element modeling codes. They do not have a sophisticated mesh generator,
graphical output, or unlimited technical support. Their primary strengths are ease-of-use, modest resource requirements, and accurate
modeling of simple three-dimensional configurations over a wide range of frequencies.*"

### Web

[http://www.cvel.clemson.edu/modeling/EMAG/EMAP](http://www.cvel.clemson.edu/modeling/EMAG/EMAP)

<p>&nbsp;</p>

<!-- <<<featflow>>> -->
## <a name="featflow"></a> FEATFLOW
    
"*The progam package FEATFLOW is both a user oriented as well as a general purpose subroutine system for the numerical solution of the
incompressible Navier-Stokes equations in two and three space dimensions. It is based on the packages FEAT2D and FEAT3D.*

*FEATFLOW is designed for the following three classes of applications:*
	    
* *Education of students*
* *Scientific research*
* *Industrial applications*"
    
<p>&nbsp;</p>

<!-- <<<Feel++ : Finite Element Embedded Library in C++>>> -->
## <a name="Feel++ : Finite Element Embedded Library in C++"></a> Feel++ : Finite Element Embedded Library in C++

"*FEEL++ est une bibliothèque C++ pour la résolution des EDP par des méthodes de Galerkin généralisées telles que les méthodes des éléments finis simples et étendues (FEM et hp-FEM) et les méthodes spectrales.*"

[Fiche PLUME](http://www.projet-plume.org/relier/feel)

<p>&nbsp;</p>

<!-- <<<FElt>>> -->
## <a name="FElt"></a> FElt

"*The current version of FElt knows how to solve linear static and dynamic structural and thermal analysis problems; it can also do modal
and spectral analysis for dynamic problems. FElt's element library currently contains fourteen elements. The **FAQ** contains some
additional information about what what kinds of problems FElt can solve as well as some information about expandability if you think you'd
like to hack on FElt for your own purposes. A user can access FElt's capabilities through several different interfaces. The three most
important are felt, the basic command-line application for solving FE problems given a standard FElt input file, burlap, our powerful,
interactive, scripting environment that combines the flexibility of [Matlab](#matlab)-like programs with FElt's finite element know-how and
velvet, the full-featured CAD like pre- and post-processor that uses the X Window System for a graphical environment. All three applications
use an intuitive, **ASCII** based syntax for problem definition. This powerful syntax allows you to substitute analytic functions in place
of numeric values (sin(60) instead of 0.866025) and even more importantly allows for time-dependent forcing and boundary conditions to be
specified as analytic functions of time or in the more traditional fashion as a series of discrete time, magnitude pairs. This feature makes
it quite easy to specify a wide range of functions.*"

### Web

[http://felt.sourceforge.net/](http://felt.sourceforge.net/)

### Documentation

[http://felt.sourceforge.net/#other_docsl](http://felt.sourceforge.net/#other_docsl)

### Téléchargement

[http://sourceforge.net/project/showfiles.php?group_id=2883](http://sourceforge.net/project/showfiles.php?group_id=2883)

### Exemples

[http://felt.sourceforge.net/#examplesl](http://felt.sourceforge.net/#examplesl)

<p>&nbsp;</p>

<!-- <<<FEMM>>> -->
## <A NAME="FEMM"></A> FEMM

"*A Windows finite element solver for 2D and axisymmetric magnetic and electrostatic problems with graphical pre- and post-processors.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/femm)

<p>&nbsp;</p>

<!-- <<<FEniCS>>> -->
## <a name="FEniCS"></a> FEniCS

"*The vision of FEniCS is to set a new standard in Computational Mathematical Modeling (CMM), which is the Automation of CMM (ACMM), towards
the goals of generality, efficiency, and simplicity, concerning mathematical methodology, implementation, and application.*

*The basic ingredients for the Automation of CMM are*

* *automation of discretization of differential/integral equations,*
* *automation of discrete solution,*
* *automation of error control,*
* *automation of modeling,*
* *automation of optimization.*"

* Web: [http://www.fenicsproject.org](http://www.fenicsproject.org)
* Documentation: [http://www.fenicsproject.org/documentation](http://www.fenicsproject.org/documentation)
* Téléchargement: [http://www.fenicsproject.org/download](http://www.fenicsproject.org/download)

<p>&nbsp;</p>

<!-- <<<FFTW>>> -->
## <A NAME="FFTW"></A> FFTW

"*FFTW is a C subroutine library for computing the discrete Fourier transform (DFT) in one or more dimensions, of arbitrary input size, and
of both real and complex data (as well as of even/odd data, i.e. the discrete cosine/sine transforms or DCT/DST). We believe that FFTW,
which is free software, should become the FFT library of choice for most applications.*

*Our benchmarks, performed on on a variety of platforms, show that FFTW's performance is typically superior to that of other publicly
available FFT software, and is even competitive with vendor-tuned codes. In contrast to vendor-tuned codes, however, FFTW's performance is
portable: the same program will perform well on most architectures without modification. Hence the name, “FFTW,” which stands for the
somewhat whimsical title of “Fastest Fourier Transform in the West.”*"

[Fiche PLUME](http://www.projet-plume.org/fiche/fftw)

<p>&nbsp;</p>

<!-- <<<FLAME>>> -->
## <A NAME="FLAME"></A> FLAME

Quote from [http://www.cs.utexas.edu/users/flame/overview/#node1l](http://www.cs.utexas.edu/users/flame/overview/#node1l) : "*When
considering the unmanageable complexity of computer systems, Dijkstra recently made the following observations 3:*

* *(i) When exhaustive testing is impossible -i.e., almost always- our trust can only be based on proof (be it mechanized or not).*
* *(ii) A program for which it is not clear why we should trust it, is of dubious value.*
* *(iii) A program should be structured in such a way that the argument for its correctness is feasible and not unnecessarily laborious.*
* *(iv) Given the proof, deriving a program justified by it, is much easier than, given the program, constructing a proof justifying it.*

*The core curriculum of any first-rate undergraduate Computer Science department includes at least one course that focuses on the formal
derivation and verification of algorithms 4. Many of us in scientific computing may have, at some point in time, hastily dismissed this
approach, arguing that this is all very nice for small, simple algorithms, but an academic exercise hardly applicable in “our world.” Since
it is often the case that our work involves libraries comprised of hundreds of thousands or even millions of lines of code, the knee-jerk
reaction that this approach is much too cumbersome to take seriously is understandable and the momentum of established practices and
“traditional wisdom” do little if anything to dissuade one from this line of reasoning. Yet, as the result of our search for superior
methods for designing and constructing high-performance parallel linear algebra libraries, we have come to the conclusion that it is only
through the systematic approach offered by formal methods that we will be able to deliver reliable, maintainable, flexible, yet highly
efficient matrix libraries even in the relatively well-understood area of (sequential and parallel) dense linear algebra. In this paper we
attempt to make this case.*

*While some would immediately draw the conclusion that a change to a more modern programming language like [C++](#cxx) is at least highly
desirable, if not a necessary precursor to writing elegant code, the fact is that most applications that call packages like
[LAPACK](#lapack) 1 and [ScaLAPACK](#scalapack) 2 are still written in [Fortran](#fortran) and/or [C](#c). Interfacing such an application
with a library written in [C++](#cxx) presents certain complications. However, during the mid-nineties, the Message-Passing Interface
([MPI](#mpi)) introduced to the scientific computing community a programming model, object-based programming, that possesses many of the
advantages typically associated with the intelligent use of an object-oriented language 6. Using objects (e.g. communicators in [MPI](#mpi))
to encapsulate data structures and hide complexity, a much cleaner approach to coding can be achieved. Our own work on the Parallel Linear
Algebra Package ([PLAPACK](#plapack)) borrowed from this approach in order to hide details of data distribution and data mapping in the
realm of parallel linear algebra libraries 7. The primary concept also germane to this paper is that [PLAPACK](#plapack) raises the level of
abstraction at which one programs so that indexing is essentially removed from the code, allowing the routine to reflect the algorithm as it
is naturally presented in a classroom setting. Since our initial work on [PLAPACK](#plapack), we have experimented with similar interfaces
in such seemingly disparate contexts as (parallel) out-of-core linear algebra packages and a low-level implementation of the sequential
[BLAS](#blas) 5.*

*FLAME is the latest step in the evolution of these systems. It facilitates the use of a programming style that is equally applicable to
everything from out-of-core, parallel systems to single-processor systems where cache-management is of paramount concern.*

*Over the last seven or eight years it has become apparent that what makes our task of library development more manageable is this
systematic approach to deriving algorithms coupled with the abstractions we use to make our code reflect the algorithms thus
produced. Further, it is from these experiences that we can confidently state that this approach to programming greatly reduces the
complexity of the resultant code and does not sacrifice high performance in order to do so.*

*Indeed, it is exactly the formal techniques that we may have at one time dismissed as merely academic or impractical which make this
possible, as FLAME illustrates.*"

### Web

[http://www.cs.utexas.edu/users/flame](http://www.cs.utexas.edu/users/flame)

### Exemples

[http://www.cs.utexas.edu/users/flame/code/#indexl](http://www.cs.utexas.edu/users/flame/code/#indexl)

### Autres indications

FLAME has interfaces with [C](#c), [Fortran](#fortran), [Matlab](#matlab), [MPI](#mpi), [Octave](#octave), [PLAPACK](#plapack)

<p>&nbsp;</p>

<!-- <<<Fortran>>> -->
## <a name="Fortran"></a> Fortran

Fortran is a powerful general-purpose programming language. Other general-purpose programming languages include [C](#c) and [C++](#cxx).

Documentation:

* Initiation : [Fortran 77](http://www.chem.ox.ac.uk/fortran/#fortran1l)
* Référence : [Fortran 77](http://www.obliquity.com/computer/fortran/)

[Questions/Réponses de programmation](#questions_reponses_langages_compiles)

### Questions/Réponses

#### Comment exécuter un programme Fortran?

Depuis un terminal Linux :

<pre >gfortran programme.f -o programme
./programme</pre>

#### Legacy Fortran programs

Fortran 77 programs may not run as expected with recent fortran compilers, because variables are not initialized to zero by default anymore. In the case of [gfortran](http://gcc.gnu.org/wiki/GFortran), the old behaviour is obtained by adding  <strong>-finit-local-zero</strong> to the compiling command.

#### Tektronix terminals

Graphical programs that rely on [Textronix terminal](http://en.wikipedia.org/wiki/Tektronix_4010)-type commands to draw pictures can use <strong>xterm -t</strong> to run under Linux.

#### Quel environnement de programmation intégré pour Fortran 95 sous Linux?

[Eclipse](http://www.eclipse.org) et [Photran](http://www.eclipse.org/photran) ont été testés avec succès sous Linux. <em >Attention:* l'installation de Photran nécessite une configuration manuelle des téléchargements d'extensions pour eclipse.

#### Quelle est la correspondance entre la directive Fortran &quot;selected_real_kind&quot; les types C++ float et double?

La définition de cette directive est ici: [http://gcc.gnu.org/onlinedocs/gcc-4.7.1/gfortran/SELECTED_005fREAL_005fKIND.html](http://gcc.gnu.org/onlinedocs/gcc-4.7.1/gfortran/SELECTED_005fREAL_005fKIND.html)

La relation avec les autres langages: [http://stackoverflow.com/questions/838310/fortran-90-kind-parameter](http://stackoverflow.com/questions/838310/fortran-90-kind-parameter)

<p>&nbsp;</p>

<!-- <<<FreeFEM++-cs>>> -->
## <a name="FreeFEM++-cs"></a> FreeFEM++-cs

"*FreeFem++-cs is an integrated development environment for [FreeFem++](#freefem) that aims to provide a user-friendly interface which
resembles other popular windowed applications. It follows a client/server design : the client deals with user interaction, the server runs
FreeFem++ (hence its name : “cs” as in “Client and Server”).*

*FreeFem++-cs adds the following extra features to FreeFem++ :*

* *an integrated interface aimed at making users comfortable,*
* *a color-coded editor,*
* *FreeFem++ errors are linked back to the EDP source code,*
* *an integrated graphics area with a zooming tool.*"

Auteur : Antoine Le Hyaric ([http://www.ljll.math.upmc.fr/lehyaric](http://www.ljll.math.upmc.fr/lehyaric))

[Exemples](http://www.ljll.math.upmc.fr/lehyaric/ffcs/#screenshots)

[Questions/Réponses Sur FreeFem++](#questions_reponses_sur_freefem)

### Questions/Réponses

#### Comment ouvrir un script EDP sous MacOS

FreeFem++-cs pour MacOS utilise l'interface X11 comme Linux mais dispose d'une icône supplémentaire (dans la barre des tâches) qui ouvre
automatiquement dans FreeFem++-cs tout script EDP qui est glissé/déposé sur cette icône.

#### Si FreeFem++-cs ne fonctionne plus après un changement de version d'Ubuntu

Il faut télécharger la version de FreeFem++-cs qui correspond à chaque nouvelle version d'Ubuntu à [http://www.ljll.math.upmc.fr/lehyaric/ffcs/#install](http://www.ljll.math.upmc.fr/lehyaric/ffcs/#install).

<p>&nbsp;</p>

<!-- <<<FreeFem++>>> -->
## <a name="FreeFem++"></a> FreeFem++

"*FreeFem++ is an implementation of a language dedicated to the finite element method. It provides you a way to solve Partial Differential
Equations (PDE) simply.  Problems involving partial differential equations (pde) of several branches of physics such as fluid-structure
interactions require interpolations of data on several meshes and their manipulation within one program.*"

* [Fiche PLUME](http://www.projet-plume.org/fiche/freefem)
* Documentation: [http://www.um.es/freefemv3/ff++/pmwiki.php](http://www.um.es/freefemv3/ff++/pmwiki.php)
* [FreeFem++-cs](#freefem_cs) est une interface graphique pour FreeFem++.

[Questions/Réponses Sur FreeFem++](#questions_reponses_sur_freefem)

<p>&nbsp;</p>

<!-- <<<Free Meshes>>> -->
## <a name="Free Meshes"></a> Free Meshes

Free pre-built meshes available from the web.

* [http://www-static.cc.gatech.edu/projects/large_models/](http://www-static.cc.gatech.edu/projects/large_models/) Large Geometric Models Archive at Georgia Tech
* [http://www.ocnus.com/models/](http://www.ocnus.com/models/) VRML Models from ORC Incorporated

<p>&nbsp;</p>

<!-- <<<GDB>>> -->
## <A NAME="GDB"></A> GDB

"*GDB, the GNU Project debugger, allows you to see what is going on 'inside' another program while it executes – or what another program was
doing at the moment it crashed.*

*GDB can do four main kinds of things (plus other things in support of these) to help you catch bugs in the act:*

* *Start your program, specifying anything that might affect its behavior.*
* *Make your program stop on specified conditions.*
* *Examine what has happened, when your program has stopped.*
* *Change things in your program, so you can experiment with correcting the effects of one bug and go on to learn about another.*

*The program being debugged can be written in C, C++, Pascal, Objective-C (and many other languages). Those programs might be executing on the same machine as GDB (native) or on another machine (remote). GDB can run on most popular UNIX and Microsoft Windows variants.*"

* Web: [http://www.gnu.org/software/gdb/#gdbl](http://www.gnu.org/software/gdb/#gdbl)

* Documentation: [reference card](http://sources.redhat.com/gdb/current/onlinedocs/refcard.ps.gz)

<p>&nbsp;</p>

<!-- <<<Geomview>>> -->
## <a name="Geomview"></a> Geomview

"*Geomview is an interactive 3D viewing program for Unix. It lets you view and manipulate 3D objects: you use the mouse to rotate,
translate, zoom in and out, etc. It can be used as a standalone viewer for static objects or as a display engine for other programs which
produce dynamically changing geometry. It can display objects described in a variety of file formats. It comes with a wide selection of
example objects, and you can create your own objects too.*"

### Web

[http://www.geomview.org/](http://www.geomview.org/)

### Documentation

[http://www.geomview.org/docs/](http://www.geomview.org/docs/)

OOGL tutorial : [http://www.geomview.org/docs/#oogltourl](http://www.geomview.org/docs/#oogltourl)

### Licence

[GNU Lesser General Public License (LGPL)](#licences_pour_logiciels_libres)

### Format de données standard lus

OOGL, [OFF](#off)

### Logiciels capables d'écrire dans ce format

[Rheolef](#rheolef)

<p>&nbsp;</p>

<!-- <<<Gerris Flow Solver>>> -->
## <a name="Gerris Flow Solver"></a> Gerris Flow Solver

"*Gerris is an Open Source Free Software library for the solution of the partial differential equations describing fluid flow. The source
code is available free of charge under the [Free Software GPL license](#licences_pour_logiciels_libres).*

*Gerris is supported by NIWA (National Institute of Water and Atmospheric research) and by the Marsden Fund of the Royal Society of New Zealand.*

*The code is written entirely in [C](#c) and uses both the GLib Library and the [GTS Library](#gnu_triangulated_surface_library) for
geometrical functions and object-oriented programming.*

*A brief summary of its main (current) features:*

* *The same code base is compiled with 2D and 3D support.*
* *Quadtree-based (Octree in 3D) spatial discretisation with automatic and dynamic local refinement.*
* *Multigrid Poisson solver.*
* *Second-order Godunov type advection scheme.*
* *Solves the time-dependent incompressible variable-density Euler, Stokes or Navier-Stokes equations or the 2D shallow-water and 3D
  hydrostatic oceanic equations.*
* *Support for complex solid boundaries (automatic locally-refined mesh generation).*
* *Semi-implicit multigrid diffusion solver with support for complex boundaries and associated boundary conditions in 2D and 3D.*
* *Semi-implicit multigrid barotropic solver for the oceanic equations.*
* *Adaptive mesh refinement: the resolution is adapted dynamically to the features of the flow.*
* *Flexible and powerful specifications of parameters.*
* *Flexible object-oriented custom specification of initial and boundary conditions, source terms, outputs etc…*
* *Portable parallel support using the [MPI](#mpi) library.*
* *Volume of Fluid advection scheme for interfacial flows.*

*The code is being actively worked on. Future developments include:*

* *Extension of the shallow-water equations model to atmospheric flows.*
* *Non-hydrostatic oceanic and anelastic atmospheric flows support.*"

### Web

[http://gfs.sourceforge.net/wiki/index.php/Main_Page](http://gfs.sourceforge.net/wiki/index.php/Main_Page)

### Documentation

[Tutorial](http://gfs.sourceforge.net/tutorial/tutorial/#tutorial1l)

[FAQ](http://gfs.sourceforge.net/faq/faq/#indexl)

### Exemples

[Gerris in action](http://gfs.sourceforge.net/#galleryl)

[Examples](http://gfs.sourceforge.net/examples/examples/#indexl)

### Licence

"*The source code is available free of charge under the [Free Software GPL license](#licences_pour_logiciels_libres).*"

<p>&nbsp;</p>

<!-- <<<GetDP>>> -->
## <a name="GetDP"></a> GetDP

"*GetDP is a general finite element solver using mixed elements to discretize de Rham-type complexes in one, two and three dimensions. The
main feature of GetDP is the closeness between the input data defining discrete problems (written by the user in **ASCII** data files) and
the symbolic mathematical expressions of these problems.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/getdp)

### Documentation

[Which problems can GetDP actually solve?](http://www.geuz.org/getdp/doc/texinfo/#getdp_3l%23SEC12)

<p>&nbsp;</p>

<!-- <<<Getfem++>>> -->
## <a name="Getfem++"></a> Getfem++

"*The Getfem++ project focuses on the development of a generic and efficient [C++](#cxx) library for finite element methods elementary
computations. The goal is to provide a library allowing the computation of any elementary matrix (even for mixed finite element methods) on
the largest class of methods and elements, and for arbitrary dimension (i.e. not only 2D and 3D problems).*

*It offers a complete separation between integration methods (exact or approximated), geometric transformations (linear or not) and finite
element methods of arbitrary degrees. It can really relieve a more integrated finite element code of technical difficulties of elementary
computations.*

*Examples of available finite element method are : Pk on simplices in arbitrary degrees and dimensions, Qk on parallelepipeds, P1, P2 with
bubble functions, Hermite elements, elements with hierarchic basis (for multigrid methods for instance), discontinuous Pk or Qk, XFem, …*

*The addition of a new finite element method is straightforward. Its description on the reference element must be provided (in most of the
cases, this is the description of the basis functions, and nothing more). Extensions are provided for Hermite elements, piecewise
polynomial, non-polynomial and vectorial elements, XFem.*

*The library also includes the usual tools for finite elements such as assembly procedures for classical PDEs, interpolation methods,
computation of norms, mesh operations, boundary conditions, post-processing tools such as extraction of slices from a mesh …*

*Getfem++ can be used to build very general finite elements codes, where the finite elements, integration methods, dimension of the meshes,
are just some parameters that can be changed very easily, thus allowing a large spectrum of experimentations. Examples are provided (see the
screenshot section).*

*Getfem++ has no meshing capabilities (apart regular meshes), hence it is necessary to import meshes. Imports formats currently known by
getfem are GiD , [Gmsh](#gmsh) and >EMC2 mesh files.*

*A particular method allows to interpolate a finite element method on an arbitrary mesh allowing any assembly procedure to work with two
different meshes. This is usefull for some mixed finite element methods and for mortar methods with non-matching meshes.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/getfem)

* Format de données standard lus: [Gmsh](#gmsh), EMC2
* Autres indications: [Matlab](#matlab) interface available.

<p>&nbsp;</p>

<!-- <<<GETM>>> -->
## <A NAME="GETM"></A> GETM

"*GETM is a 3D numerical model simulating the most important hydrodynamic and thermodynamic processes in natural waters. The model is
general in the sense that it can be applied to various systems, scales and specifications. The model includes for example flooding and
drying of tidal flats, flexible vertical and horizontal coordinate systems, different turbulence models integrated from [GOTM](#gotm), and
is a Public Domain model published under [GNU Public Licence](#licences_pour_logiciels_libres).*"

### Web

[http://www.getm.eu](http://www.getm.eu)

<p>&nbsp;</p>

<!-- <<<Gmsh>>> -->
## <a name="Gmsh"></a> Gmsh

"*Gmsh is an automatic 3D finite element mesh generator (primarily Delaunay) with build-in CAD and post-processing facilities. Its primal
design goal is to provide a simple meshing tool for academic test cases with parametric input and up to date visualization capabilities. One
of its strengths is the ability to respect a characteristic length field for the generation of adapted meshes on lines, surfaces and
volumes, and to mix these meshes with simple structured grids.*

*Gmsh is built around four modules: geometry, mesh, solver and post-processing. The specification of any input to these modules is done
either interactively using the graphical user interface or in **ASCII** text files using Gmsh's own scripting language.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/gmsh)

### Documentation

[http://www.geuz.org/gmsh/doc/texinfo/#gmshl](http://www.geuz.org/gmsh/doc/texinfo/#gmshl)

### Logiciels capables de lire ce format

[Code_Aster](#code_aster), [Salomé](#salome)

<p>&nbsp;</p>

<!-- <<<GNU Make>>> -->
## <a name="GNU Make"></a> GNU Make

"*Make is a tool which controls the generation of executables and other non-source files of a program from the program's source files.*

*Make gets its knowledge of how to build your program from a file called the makefile, which lists each of the non-source files and how to
compute it from other files. When you write a program, you should write a makefile for it, so that it is possible to use Make to build and
install the program.*"

* Web: [http://www.gnu.org/software/make/](http://www.gnu.org/software/make/)
* Documentation:[http://www.gnu.org/software/make/manual/](http://www.gnu.org/software/make/manual/)

### Questions/Réponses

#### How to give a value to a make macro when calling make from the command line?

If MACRO is used inside a makefile, one can give it a value from the command line with

<pre >make MACRO=value</pre>

<p>&nbsp;</p>

<!-- <<<Gnuplot>>> -->
## <a name="Gnuplot"></a> Gnuplot

"*gnuplot is a command-driven interactive function plotting program. It can be used to plot functions and data points in both two- and
three-dimensional plots in many different formats, and will accommodate many of the needs of today's scientists for graphic data
representation. gnuplot is copyrighted, but freely distributable; you don't have to pay for it.*"

* [Fiche PLUME](http://www.projet-plume.org/fiche/gnuplot)
* Tutorial : [http://www.duke.edu/~hpgavin/#gnuplotl](http://www.duke.edu/~hpgavin/#gnuplotl)
* Manual : [http://theochem.ki.ku.dk/on_line_docs/gnuplot/#gnuplot_tocl](http://theochem.ki.ku.dk/on_line_docs/gnuplot/#gnuplot_tocl)
* **FAQ** : [http://www.gnuplot.info/faq/](http://www.gnuplot.info/faq/)
</li>
</ul>

### Questions/Réponses

#### Comment dessiner une courbe avec comme X et Y les deux colonnes d'un fichier
<pre >&gt; gnuplot

	G N U P L O T
	Version 4.4 patchlevel 0
	last modified March 2010
	System: Linux 2.6.39-2-686-pae

	Copyright (C) 1986-1993, 1998, 2004, 2007-2010
	Thomas Williams, Colin Kelley and many others

	gnuplot home:     http://www.gnuplot.info
	faq, bugs, etc:   type &quot;help seeking-assistance&quot;
	immediate help:   type &quot;help&quot;
	plot window:      hit 'h'

Terminal type set to 'wxt'
gnuplot&gt; plot 'resultats.dat' using 1:2 title 'Résultats' with lines
gnuplot&gt; quit</pre>

#### Comment dessiner deux courbes sur le même graphe, la première avec les colonnes 1 et 2 du fichier, la deuxième avec les colonnes 1 et 3?
<pre >&gt; gnuplot

	G N U P L O T
	Version 4.4 patchlevel 0
	last modified March 2010
	System: Linux 2.6.39-2-686-pae

	Copyright (C) 1986-1993, 1998, 2004, 2007-2010
	Thomas Williams, Colin Kelley and many others

	gnuplot home:     http://www.gnuplot.info
	faq, bugs, etc:   type &quot;help seeking-assistance&quot;
	immediate help:   type &quot;help&quot;
	plot window:      hit 'h'

Terminal type set to 'wxt'
gnuplot&gt; plot 'resultats.dat' using 1:2 title 'Courbe 1' with lines,'resultats.dat' using 1:3 title 'Courbe 2' with lines
gnuplot&gt; quit</pre>

#### Comment tracer une droite passant par des points expérimentaux?
<pre >f1(x)=a*x+b
a=10;b=10;
fit f1(x) 'data.dat' using 1:2 via a,b

plot &quot;data.dat&quot; using 1:2,a*x+b title 'fit'

pause -1</pre>

<p>&nbsp;</p>

<!-- <<<GNU Scientific Library>>> -->
## <a name="GNU Scientific Library"></a> GNU Scientific Library

"*The GNU Scientific Library (GSL) is a numerical library for [C](#c) and [C++](#cxx) programmers. It is free software under the [GNU General Public License](#licences_pour_logiciels_libres).*

*The library provides a wide range of mathematical routines such as random number generators, special functions and least-squares fitting. There are over 1000 functions in total.*

*Unlike the licenses of proprietary numerical libraries the license of GSL does not restrict scientific cooperation. It allows you to share your programs freely with others.*"

### Web

[http://www.gnu.org/software/gsl/#gsll](http://www.gnu.org/software/gsl/#gsll)

### Documentation

[http://www.gnu.org/software/gsl/manual/html_node/](http://www.gnu.org/software/gsl/manual/html_node/)

### Informations sur les formats de données

The GNU Scientific Library implements [BLAS](#blas) support as described in

[http://www.gnu.org/software/gsl/manual/html_node/BLAS-S#upportl](http://www.gnu.org/software/gsl/manual/html_node/BLAS-S#upportl)

<p>&nbsp;</p>

<!-- <<<GNU Triangulated Surface Library>>> -->
## <a name="GNU Triangulated Surface Library"></a> GNU Triangulated Surface Library

"*GTS stands for the GNU Triangulated Surface Library. It is an Open Source Free Software Library intended to provide a set of useful functions to deal with 3D surfaces meshed with interconnected triangles. The source code is available free of charge under the Free Software [LGPL](#licences_pour_logiciels_libres) license.*

*The code is written entirely in [C](#c) with an object-oriented approach based mostly on the design of GTK+. Careful attention is paid to performance related issues as the initial goal of GTS is to provide a simple and efficient library to scientists dealing with 3D computational surface meshes.*

*A brief summary of its main features:*

<ul>
*  *Simple object-oriented structure giving easy access to topological properties.*

*  *2D dynamic Delaunay and constrained Delaunay triangulations.*

*  *Robust geometric predicates (orientation, in circle) using fast adaptive floating point arithmetic (adapted from the fine work of Jonathan R. Shewchuk).*

*  *Robust set operations on surfaces (union, intersection, difference).*

*  *Surface refinement and coarsening (multiresolution models).*

*  *Dynamic view-independent continuous level-of-detail.*

*  *Preliminary support for view-dependent level-of-detail.*

*  *Bounding-boxes trees and Kd-trees for efficient point location and collision/intersection detection.*

*  *Graph operations: traversal, graph partitioning.*

*  *Metric operations (area, volume, curvature …).*

*  *Triangle strips generation for fast rendering.*"

</ul>

### Web

[http://gts.sourceforge.net/#indexl](http://gts.sourceforge.net/#indexl)

### Documentation

[http://gts.sourceforge.net/reference/#book1l](http://gts.sourceforge.net/reference/#book1l)

### Exemples

[http://gts.sourceforge.net/#galleryl](http://gts.sourceforge.net/#galleryl),

[http://gts.sourceforge.net/#samplesl](http://gts.sourceforge.net/#samplesl)

### Licence

[LGPL](#licences_pour_logiciels_libres)

<p>&nbsp;</p>

<!-- <<<gotm>>> -->
## <a name="gotm"></a> GOTM

"*GOTM is the abbreviation for 'General Ocean Turbulence Model'. It is a one-dimensional water column model for the most important
hydrodynamic and thermodynamic processes related to vertical mixing in natural waters. In addition, it has been designed such that it can
easily be coupled to 3-D circulation models, and used as a module for the computation of vertical turbulent mixing. The core of the model
computes solutions for the one-dimensional versions of the transport equations of momentum, salt and heat. The key component in solving
these equations is the model for the turbulent fluxes of these quantities. The strength of GOTM is the vast number of well-tested turbulence
models that have been implemented in the code. These models span the range from simple prescribed expressions for the turbulent
diffusivities up to complex Reynolds-stress models with several differential transport equations to solve. Even though, evidently, not all
turbulence models published in oceanography could be implemented, at least one member of every relevant model family can be found in GOTM:
empirical models, energy models, two-equation models, Explicit Algebraic Stress Models (EASM), and K-profile parameterisations (KPP).*"

### Web

[http://www.gotm.net/](http://www.gotm.net/)
    
<p>&nbsp;</p>

<!-- <<<GRUMMP>>> -->
## <A NAME="GRUMMP"></A> GRUMMP

"*GRUMMP — Generation and Refinement of Unstructured, Mixed-Element Meshes in Parallel*

*Goals of the GRUMMP Project*

*The goal of the GRUMMP project is to develop automatic mesh generation software for unstructured meshes with mixed element types. The software should produce high-quality meshes that meet user-defined mesh density requirements, using elements appropriate for the geometry and physics of a particular problem.*

*Automatic mesh generation for complex two and three dimensional domains is a topic of intensive research. It is imperative that automatic mesh generation tools be capable of generating quality finite element and finite volume meshes. There must be a balance between resolution of the boundary and surface features and complexity of the problem. In addition, for problems with isotropic physics, element aspect ratio must be small to minimize linear system condition number and interpolation error. On the other hand, problems with anisotropic physics (for example, a shear layer in viscous fluid flow) require highly anisotropic elements for efficient solution. A further level of complication is that for some physical problems and applications, quadrilateral (2D) or hexahedral (3D) elements are preferred, even though filling space with high quality elements is easier using triangular (2D) or tetrahedral (3D) elements.*

*A general-purpose automatic mesh generator should address all of these issues without excessive user intervention. We envision a system in which common types of physical problems have predefined mesh sizing and element aspect ratio functions, allowing easy generation of meshes for these applications areas. For flexibility and generality, the user will also be able to prescribe these functions (for totally different applications) or modify the predefined behaviors (to provide a quality mesh in the wake of an airplane wing, for example).*

*GRUMMP addresses these issues by implementing mesh manipulation primitives to generate or modify existing meshes so that criteria for element size and quality are met. In addition, automatic computation of local length scale is performed to provide a default in cases where solution-based adaptive length scales are not available.*"

### Web

[http://tetra.mech.ubc.ca/GRUMMP/](http://tetra.mech.ubc.ca/GRUMMP/)

### Documentation

[http://tetra.mech.ubc.ca/GRUMMP/UserG#uidel](http://tetra.mech.ubc.ca/GRUMMP/UserG#uidel)

### Licence

[http://tetra.mech.ubc.ca/GRUMMP/LICENSE](http://tetra.mech.ubc.ca/GRUMMP/LICENSE)

### Informations sur les formats de données

[http://tetra.mech.ubc.ca/GRUMMP/File_F#ormatsl](http://tetra.mech.ubc.ca/GRUMMP/File_F#ormatsl)

<p>&nbsp;</p>

<!-- <<<HDF>>> -->
## <A NAME="HDF"></A> HDF

"*WELCOME to the Hierarchical Data Format (HDF) home page at the National Center for Supercomputing Applications.

The HDF project involves the development and support of software and file formats for scientific data management. The HDF software includes
I/O libraries and tools for analyzing, visualizing, and converting scientific data. There are two HDF formats, HDF (4.x and previous
releases) and HDF5. These formats are completely different and NOT compatible. ( NOTE: There are no plans to drop support for HDF 4.x )

The HDF software is developed and supported by NCSA and is freely available. It is used world-wide in many fields, including Environmental
Science, Neutron Scattering, Non-Destructive Testing, and Aerospace, to name a few. Scientific projects that use HDF include NASA's
HDF-EOS project, and the DOE's Advanced Simulation and Computing Program. *"

### Documentation

[http://www.hdfgroup.org/HDF5/#indexl](http://www.hdfgroup.org/HDF5/#indexl)

<p>&nbsp;</p>

<!-- <<<Hypre>>> -->
## <a name="Hypre"></a> Hypre

"*The goal of the Scalable Linear Solvers project is to develop scalable algorithms and software for solving large, sparse linear systems of equations on parallel computers. The primary software product is hypre, a library of high performance preconditioners that features parallel multigrid methods for both structured and unstructured grid problems. The problems of interest arise in the simulation codes being developed at LLNL and elsewhere to study physical phenomena in the defense, environmental, energy, and biological sciences.*"

### Web

[http://www.llnl.gov/CASC/linear_solvers/](http://www.llnl.gov/CASC/linear_solvers/)

### Documentation

[Users' Manual](http://www.llnl.gov/CASC/hypre/hypre-1.6.0/HYPRE_usr_manual.ps),

[Reference Manual](http://www.llnl.gov/CASC/hypre/hypre-1.6.0/HYPRE_ref_manual.ps)

### Téléchargement

[http://www.llnl.gov/CASC/hypre/#softwarel](http://www.llnl.gov/CASC/hypre/#softwarel)

<p>&nbsp;</p>

<!-- <<<I-DEAS file format>>> -->
## <a name="I-DEAS file format"></a> I-DEAS file format

File format of the [I-DEAS computer-aided design software package](http://en.wikipedia.org/wiki/I-DEAS). It can be used in [Matlab](#matlab) : [http://www.mathworks.com/matlabcentral/fileexchange/loadFile.do?objectId=6395&amp;objectType=file](http://www.mathworks.com/matlabcentral/fileexchange/loadFile.do?objectId=6395&amp;objectType=file)
and [libMesh](#libmesh).

<p>&nbsp;</p>

<!-- <<<IGES>>> -->
## <A NAME="IGES"></A> IGES

"*Products may be designed as either a two-dimensional, three-view drawing layout, or as a full three-dimensional model with associated drawing views and dimensions using a Computer Aided Design (CAD) system. The IGES format serves as a neutral data format to transfer the design to a dissimilar system. Translators, developed to the IGES Standard, are used to export a design into an IGES file for exchange and for importing the IGES file into the destination system.*"

### Web

[http://en.wikipedia.org/wiki/IGES](http://en.wikipedia.org/wiki/IGES)

### Logiciels capables de lire ce format

[Netgen](#netgen), [Salomé](#salome)

### Logiciels capables d'écrire dans ce format

[Salomé](#salome)

<p>&nbsp;</p>

<!-- <<<IML++>>> -->
## <A NAME="IML++"></A> IML++

"*IML++ is a [C++](#cxx) templated library of modern iterative methods for solving both symmetric and nonsymmetric linear systems of equations. The algorithms are fully templated in that the same source code works for dense, sparse, and distributed matrices. Some of the numerical methods are presented in the book, Templates: Building Blocks for the Solution of Iterative Systems and include*

<ul>
*  *Richardson Iteration*

*  *Chebyshev Iteration*

*  *Conjugate Gradient (CG)*

*  *Conjugate Gradient Squared (CGS)*

*  *BiConjugate Gradient (BiCG)*

*  *BiConjugate Gradient Stabilized (BiCGSTAB)*

*  *Generalized Minimum Residual (GMRES)*

*  *Quasi-Minimal Residual Without Lookahead (QMR)*

</ul>

*The IML++ software also contains an optional test suite for sparse matrix computations, using [SparseLib++](#sparselib).*"

### Web

[http://math.nist.gov/iml++/](http://math.nist.gov/iml%2b%2b/)

<p>&nbsp;</p>

<!-- <<<Impact>>> -->
## <a name="Impact"></a> Impact

"*Impact is an open source finite element program suite which can be used to predict most dynamic events such as car crashes or metal sheet punch operations. They usually involve large deformations and high velocities.*

*Simulations are made on a virtual three dimensional model which can be created with a pre-processor or with the built-in Fembic language. Results are viewed in a post-processor.*

*Impact is designed to interface with the included pre- and postprocessor by default, but there are also interfaces available for more advanced pre-and postprocessors such as GiD or Gmsh. Impact also has rudamentary support for Nastran file format.*

*Development is made by a team of volunteers from all over the world with the aim of creating a clean and compact program which is simple to understand and use.*

*Impact is licensed under the [Gnu Public License](#licences_pour_logiciels_libres) which makes it free to use and modify as long as you release and publish your improvements under the same license.*

*Impact is written in Java which means it can be run on most hardware and operating systems.*"

### Web

[http://impact.sourceforge.net/](http://impact.sourceforge.net/)

<p>&nbsp;</p>

<!-- <<<ISAAC>>> -->
## <A NAME="ISAAC"></A> ISAAC

"*ISAAC (Integrated Solution Algorithm for Arbitrary Configurations) is a compressible Euler/Navier-Stokes computational fluid dynamics code. ISAAC includes the capability of calculating the Euler equations for inviscid flow or the Navier-Stokes equations for viscous flows. ISAAC uses a domain decomposition structure to accomodate complex physical configurations. ISAAC can calculate either steady-state or time dependent flow.*

*ISAAC was designed to test turbulence models. Various two equation turbulence models, explicit algebraic Reynolds stress models, and full differential Reynolds stress models are implemented in ISAAC. Several test cases are documented in the User's Guide.  *"

### Web

[http://isaac-cfd.sourceforge.net/](http://isaac-cfd.sourceforge.net/)

### Documentation

[http://isaac-cfd.sourceforge.net/man.pdf](http://isaac-cfd.sourceforge.net/man.pdf)

### Téléchargement

[http://isaac-cfd.sourceforge.net/#downloadl](http://isaac-cfd.sourceforge.net/#downloadl)

### Licence

[http://isaac-cfd.sourceforge.net/#licensel](http://isaac-cfd.sourceforge.net/#licensel)

<p>&nbsp;</p>

<!-- <<<ITPACK>>> -->
## <A NAME="ITPACK"></A> ITPACK

"*There are four packages in the ITPACK directory for solving large sparse linear systems by iterative methods: ITPACK 2C (single precision), ITPACK 2C (double precision), ITPACKV 2D (a vectorized version of ITPACK 2C for the Cray Y-MP and similar vector computers), and NSPCG.  ITPACK 2C and ITPACKV 2D are intended for symmetric and positive-definite matrix problems.  NSPCG has preconditioners and polynomial accelerators for nonsymmetric matrix problems as well.  Only single precision versions are available for ITPACKV 2D and NSPCG.  Machine-dependent constants and the timing function may need to be modified by the user when installing the packages for a particular computer.  They are located in routines DFAULT and TIMER in all four packages.*"

### Web

[http://www.netlib.org/itpack/](http://www.netlib.org/itpack/)

<p>&nbsp;</p>

<!-- <<<jCAE>>> -->
## <a name="jCAE"></a> jCAE

"*Features*

<ul>
*  *simple volumes modeler*

*  *finit elements mesher*

*  *portable on platforms which support Java and Opencascade*

*  *inherit module architecture of Netbeans*"

</ul>

### Web

[http://jcae.sourceforge.net](http://jcae.sourceforge.net)

### Exemples

[http://jcae.sourceforge.net/#screenshotsl](http://jcae.sourceforge.net/#screenshotsl)

<p>&nbsp;</p>

<!-- <<<LAPACK>>> -->
## <A NAME="LAPACK"></A> LAPACK

"*LAPACK is written in [Fortran](#fortran) 77 and provides routines for solving systems of simultaneous linear equations, least-squares solutions of linear systems of equations, eigenvalue problems, and singular value problems. The associated matrix factorizations (LU, Cholesky, QR, SVD, Schur, generalized Schur) are also provided, as are related computations such as reordering of the Schur factorizations and estimating condition numbers. Dense and banded matrices are handled, but not general sparse matrices. In all areas, similar functionality is provided for real and complex matrices, in both single and double precision.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/lapack)

### Documentation

[FAQ](http://www.netlib.org/lapack/#faql),

[User's guide](http://www.netlib.org/lapack/lug/#lapack_lugl)

### Autres indications

LAPACK should be used together with an optimized version of the [BLAS](#blas). For instance, see [Atlas](#atlas).

<p>&nbsp;</p>

<!-- <<<LaTeX>>> -->
## <a name="LaTeX"></a> LaTeX

"*LaTeX is a high-quality typesetting system, with features designed for the production of technical and scientific documentation. LaTeX is the de facto standard for the communication and publication of scientific documents.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/latex)

<ul>
*  Initiation : [FAQ](http://www.grappa.univ-lille3.fr/FAQ-LaTeX/) (Français), [http://www.maths.tcd.ie/~dwilkins/LaTeXPrimer](http://www.maths.tcd.ie/~dwilkins/LaTeXPrimer) (English)

*  Référence : [http://en.wikibooks.org/wiki/LaTeX](http://en.wikibooks.org/wiki/LaTeX)

*  Retrouver le nom d'un symbole LaTeX en le dessinant : [http://detexify.kirelabs.org/#classifyl](http://detexify.kirelabs.org/#classifyl)

</ul>

### Questions/Réponses

#### Transparents
<ul>
*  Beamer

*  Prosper : [styles disponibles](http://prosper.sourceforge.net/#viewerl)

*  Seminar : [seminar user's guide](http://tex.loria.fr/classes/sem-user.pdf)

</ul>

#### Graphiques avec TikZ

"*PGF is a TeX macro package for generating graphics. It is platform- and format-independent and works together with the most important TeX backend drivers, including pdftex and dvips. It comes with a user-friedly syntax layer called TikZ.*"

[https://sourceforge.net/projects/pgf/](https://sourceforge.net/projects/pgf/)

#### Comment récupérer les images d'un ancien article dont on ne possède plus que le PDF?

Sous Linux, ouvrir le PDF avec [evince](http://projects.gnome.org/evince), et glisser/déposer les images avec la souris sur le bureau.

#### Comment rédiger un document Latex avec Linux?

Avec [kile](http://kile.sourceforge.net)

#### Comment changer la numérotation des équations

citation de [http://www.math.uiuc.edu/~hildebr/tex/#displaysl](http://www.math.uiuc.edu/~hildebr/tex/#displaysl): *By default, LaTeX will number equations consecutively, as (1), (2), etc., assuming you use the automatic equation numbering mechanism. If the paper is very short, or if there are only a few numbered equations, this is fine, but once the numbers get into the twenties and higher, a scheme that numbers equations by section, as in (1.1), (1.2), …, (2.1), etc., is preferable. In fact, for the vast majority of journal articles, the latter is probably the best numbering scheme. To get equations numbered by section, just put the following into the preamble: “
\numberwithin{equation}{section} ”. For books, theses, or very long papers, an equation numbering scheme that is three levels deep (with numbers like (4.1.1), etc.) may be appropriate. To get this, just replace “section” above by “subsection”, or the corresponding innermost level. The same mechanism works for other counters, e.g., theorem counters, instead of “equation”.*

#### Imprimer un grand poster sur plusieurs feuilles A4 sous Linux

Utiliser [PosteRazor](http://posterazor.sourceforge.net).

#### Diminuer la taille d'un PDF pour une moins bonne qualité mais un téléchargement plus facile sur le web

Avec ghostscript:

<pre >gs -q -dNOPAUSE -dBATCH -dSAFER -sDEVICE=pdfwrite -dCompatibilityLevel=1.3 -dPDFSETTINGS=/screen \
-dEmbedAllFonts=true -dSubsetFonts=true -dColorImageDownsampleType=/Bicubic -dColorImageResolution=72 \
-dGrayImageDownsampleType=/Bicubic -dGrayImageResolution=72 -dMonoImageDownsampleType=/Bicubic \
-dMonoImageResolution=72 -dNumRenderingThreads=4 -sOutputFile=smalldoc.pdf bigdoc.pdf</pre>

#### Graphics with inkscape

inkscape is able to draw vector-based graphics and output them as pdf or postscript to be included in LateX documents.

#### Including .eps graphics in .pdf documents

It is as simple as including:

<pre >\usepackage{epstopdf}</pre>

On machines where the epstopdf external command is not available to LaTeX, one can also convert eps figures to pdf with:

<pre >convert figure.eps figure.pdf</pre>

<p>&nbsp;</p>

<!-- <<<libMesh>>> -->
## <a name="libMesh"></a> libMesh

"*The libMesh library is a [C++](#cxx) framework for the numerical simulation of partial differential equations on serial and parallel platforms. Development began in March 2002 with the intent of providing a friendly interface to a number of high-quality software packages that are currently available. Currently the library supports 2D and 3D steady and transient finite element simulations. [PETSc](#petsc) is currently used for the solution of linear systems on both serial and parallel platforms, and LASPack is included with the library to provide linear solver support on serial machines.*

*The libMesh library is actively developed at The University of Texas at Austin in the CFDLab and at Technische Universität Hamburg-Harburg, Modelling and Computation in Germany. Many thanks to SourceForge for hosting the project. You can find out what is currently happening in the development branch by checking out the CVS Logs online.*

*A major goal of the library is to provide support for adaptive mesh refinement (AMR) computations in parallel while allowing a research scientist to focus on the physics they are modeling.*"

<p>&nbsp;</p>

<!-- <<<Libtool>>> -->
## <a name="Libtool"></a> Libtool

"*GNU libtool is a generic library support script. Libtool hides the complexity of using shared libraries behind a consistent, portable interface.*

*To use libtool, add the new generic library building commands to your Makefile, Makefile.in, or Makefile.am. See the documentation for details.*"

### Web

[http://www.gnu.org/software/libtool/](http://www.gnu.org/software/libtool/)

### Documentation

[http://www.gnu.org/software/libtool/manual](http://www.gnu.org/software/libtool/manual)

### Licence

"*GNU Libtool is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.*"

<p>&nbsp;</p>

<!-- <<<Licences pour logiciels libres>>> -->
## <a name="Licences pour logiciels libres"></a> Licences pour logiciels libres

Pour les développeurs de logiciels dans les laboratoires de recherche (CNRS, universités, INRA…) :

<ul>
*  [Projet Plume FAQ : licence &amp; copyright pour les développements de logiciels libres de laboratoires de recherche](http://www.projet-plume.org/fr/ressource/faq-licence-copyright)

</ul>

Voici aussi une liste de licences gratuites, parmi les plus répandues :

<ul>
*  [BSD License](http://www.opensource.org/licenses/bsd-license.php)

*  [GNU General Public License (GPL)](http://www.gnu.org/copyleft/#gpll)

*  [GNU Lesser General Public License (LGPL)](http://www.fsf.org/licensing/licenses/#lgpll)

*  [Licence française de logiciel libre CeCILL](http://www.cecill.info)

</ul>

Et une autre liste en anglais : [List of Free Licenses from the Open Source Initiative](http://www.opensource.org/licenses/category)

<p>&nbsp;</p>

<!-- <<<Méfisto>>> -->
## <a name="Méfisto"></a> Méfisto

"*Ce logiciel gratuit comprend les modules exécutables à télécharger :*

<ul>
*  *Un initialisateur de fichiers numériques nécessaires pour les     modules suivants: Méfisto-INITIER;*

*  *Un générateur de maillages 2D ou 3D, structurés et/ou     non-structurés: Méfisto-MAILLER;*

*  *Un solveur du problème stationnaire ou instationnaire de     l'Élasticité linéaire: Méfisto-ELASTICER;*

*  *Un solveur du calcul des modes propres d'un objet 2d ou 3d:     Méfisto-ELASTICER;*

*  *Un solveur du problème thermique stationnaire ou     instationnaire linéaire ou non linéaire: Méfisto-THERMICER.*

*  *Un solveur du problème de l'équation des ondes planes:     Méfisto-THERMICER.*

*  *Un solveur du calcul des plus petites valeurs propres de     l'opérateur -div A grad: Méfisto-THERMICER.*

*  *Un solveur du problème de Stokes en 2d avec éléments finis de     Taylor-Hood ou Brezzi-Fortin: Méfisto-FLUIDER.

L'utilisation de ces modules est rendue conviviale par l'emploi systèmatique de menus, le recours à la souris, et une représentation graphique des résultats sur l'écran et éventuellement, dans un fichier d'instructions PostScript.*"

</ul>

### Auteur(s)

Alain Perronnet ([http://www.ljll.math.upmc.fr/perronnet](http://www.ljll.math.upmc.fr/perronnet)) 	

### Téléchargement

[http://www.ljll.math.upmc.fr/perronnet/mefisto.#genel](http://www.ljll.math.upmc.fr/perronnet/mefisto.#genel)

<p>&nbsp;</p>

<!-- <<<Mélina>>> -->
## <a name="Mélina"></a> Mélina

"*Le code MÉLINA est une bibliothèque de procédures pour la résolution de problèmes aux limites gouvernés par des équations aux dérivées partielles par la méthode des éléments finis en dimension 2 ou 3. Il a été développé par D.Martin (Université de RENNES 1) et O.deBayser (SMP, E.N.S.T.A. jusqu'en 1995) dans le cadre des problèmes étudiés au sein du groupe simulation et modélisation des phénomènes de propagation (S.M.P.). Ce code est essentiellement un code de recherche et fournit un ensemble d'outils aisément manipulables pour écrire rapidement des applications pour le traitement numérique de problèmes nouveaux ou/et la mise au point de nouveaux algorithmes.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/melina)

<p>&nbsp;</p>

<!-- <<<Matlab>>> -->
## <a name="Matlab"></a> Matlab
<ul>
*  [Historique](http://fr.wikipedia.org/wiki/MATLAB)

*  [Introduction au logiciel Matlab](http://www.ljll.math.upmc.fr/~postel/matlab)

*  Alternatives gratuites : [Octave](#octave), [Sage](#sage), [Scilab](#scilab)

</ul>

### Questions/Réponses

#### ssh sur Linux: Attention à TMOUT

Matlab est souvent lancé sur un serveur distant grâce à ssh suivi de la commande “matlab&amp;”. Il est conseillé d'ajouter la commande <strong>export TMOUT=0</strong> (TMOUT signifie time-out et représente le temps en secondes après lequel la session est déconnectée) après “ssh” avant “matlab” afin d'éviter toute déconnection automatique avant que le programme matlab soit terminé.

#### Limiter le nombre de coeurs de calcul utilisés par Matlab

Matlab utilise par défaut tous les coeurs disponibles. Pour éviter cela (par exemple quand il y a d'autres utilisateurs sur le même serveur de calcul), il faut utiliser l'option <strong>-singleCompThread</strong>

<pre >matlab -singleCompThread</pre>

(cf [http://www.mathworks.fr/help/techdoc/ref/#maxnumcompthreadsl](http://www.mathworks.fr/help/techdoc/ref/#maxnumcompthreadsl))

Les utilisateurs de MatlabMPI ont eux-aussi besoin de cette option car [MPI](#mpi)
  gère lui-même le parallélisme. Il faut donc ajouter <strong>-singleCompThread</strong> dans le fichier

<pre >MatlabMPI/src/MatMPI_Comm_settings.m</pre>

et sur la ligne de commande de tous les scripts MatlabMPI.

#### CUDA

Matlab est capable d'utiliser la carte [CUDA](#cuda) de la machine. Par exemple:

<pre ><span >%  feature('numCores')</span>
n = gpuDeviceCount;
<span >for</span> ii = <span >1</span>:n
    gpuDevice<span >&#40;</span>ii<span >&#41;</span>
<span >end</span>
&nbsp;
<span >%Transfer a 10-by-10 matrix of random single-precision values to the GPU, then use the GPU to square each element.</span>
&nbsp;
X = [<span >rand</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#randl)<span >&#40;</span><span >10</span>, <span >'single'</span><span >&#41;</span>;
G = gpuArray<span >&#40;</span>X<span >&#41;</span>;
isequal<span >&#40;</span>gather<span >&#40;</span>G<span >&#41;</span>, X<span >&#41;</span>  <span >% Returns true</span>
classUnderlying<span >&#40;</span>G<span >&#41;</span>     <span >% Returns 'single'</span>
G2 = G .* G            <span >% Uses times method defined for </span>
                       <span >% GPUArray objects</span>
&nbsp;
<span >for</span> ii = <span >1</span>:gpuDeviceCount
    g = gpuDevice<span >&#40;</span>ii<span >&#41;</span>;
    [<span >fprintf</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#fprintfl)<span >&#40;</span><span >1</span>, <span >'Device %i has ComputeCapability %s \n'</span>, <span >...</span>
            <span >g</span>.<span >Index</span>, g.<span >ComputeCapability</span><span >&#41;</span>
<span >end</span></pre>

#### Comment lancer une commande Matlab sans fenêtre graphique?
<pre >matlab -nodisplay -r commande</pre>

Ceci est très utile en conjonction avec [nohup](#nohup) ou [screen](#screen). Voici aussi un exemple de script [qsub](#qsub) :

<dl >
<dt>matlab.qsub</dt>
<dd><pre ><span >#!/bin/bash</span>
<span >#PBS -q seq</span>
<span >#PBS -N matlab</span>
<span >#PBS -j oe</span>
. <span >/</span>usr<span >/</span>share<span >/</span>modules<span >/</span>init<span >/</span><span >sh</span>
module load Matlab
<span >cd</span> <span >$PBS_O_WORKDIR</span>
matlab <span >-nodisplay</span> <span >-r</span> <span >&#91;</span>commande<span >&#93;</span></pre>
</dd></dl>

#### Les principales options de la commande Matlab
<pre >&gt; matlab -h

    Usage:  matlab [-h|-help] | [-n | -e]
                   [-arch | v=variant | v=arch/variant]
                   [-c licensefile] [-display Xdisplay | -nodisplay]
                   [-nosplash] [-mwvisual visualid] [-debug] [-softwareopengl]
                   [-desktop | -nodesktop | -nojvm]
                   [-jdb [port]]
                   [-r MATLAB_command] [-logfile log]
                   [-Ddebugger [options]]

    -h|-help             - Display arguments.
    -n                   - Display final environment variables,
                           arguments, and other diagnostic
                           information. MATLAB is not run.
    -e                   - Display ALL the environment variables and
                           their values to standard output. MATLAB
                           is not run. If the exit status is not
                           0 on return then the variables and values
                           may not be correct.
    -arch                - Start MATLAB assuming architecture arch.
    v=variant            - Start the version of MATLAB found
                           in bin/glnxa64/variant instead of bin/glnxa64.
    v=arch/variant       - Start the version of MATLAB found
                           in bin/arch/variant instead of bin/glnxa64.
    -c licensefile       - Set location of the license file that MATLAB
                           should use.  It can have the form port@host or
                           be a colon separated list of license files.
                           The LM_LICENSE_FILE and MLM_LICENSE_FILE
                           environment variables will be ignored.
    -display Xdisplay    - Send X commands to X server display, Xdisplay.
    -nodisplay           - Do not display any X commands. The MATLAB
                           desktop will not be started. However, unless
                           -nojvm is also provided the Java virtual machine
                           will be started.
    -nosplash            - Do not display the splash screen during startup.
    -mwvisual visualid   - The default X visual to use for figure windows.
    -debug               - Provide debugging information especially for X
                           based problems.
    -desktop             - Allow the MATLAB desktop to be started by a
                           process without a controlling terminal. This is
                           usually a required command line argument when
                           attempting to start MATLAB from a window manager
                           menu or desktop icon.
    -nodesktop           - Do not start the MATLAB desktop. Use the current
                           terminal for commands. The Java virtual machine
                           will be started.
    -nojvm               - Shut off all Java support by not starting the
                           Java virtual machine. In particular the MATLAB
                           desktop will not be started.
    -jdb [port]          - Enable remote Java debugging on port (default 4444)
    -r MATLAB_command    - Start MATLAB and execute the MATLAB_command.
    -logfile log         - Make a copy of any output to the command window
                           in file log. This includes all crash reports.
    -Ddebugger [options] - Start debugger to debug MATLAB.</pre>

#### Quel équivalent pour la commande Matlab ksdensity()?

avec [Octave](#octave) : [http://octave.sourceforge.net/econometrics/function/#kernel_densityl](http://octave.sourceforge.net/econometrics/function/#kernel_densityl)

#### Comment inverser une matrice?

Pour trouver l'inverse d'une matrice A, il y a plusieurs possibilités en fonction de l'utilisation prévue pour l'inverse:

<ul>
<li > simple mais très long à calculer: <strong>Inv(A)</strong>
</li>
<li > beaucoup plus rapide si on veut uniquement calculer le produit A^-1*B où B est un vecteur: <strong>A\\B</strong> (utilise la méthode de résolution matricielle par défaut).
</li>
<li > pour choisir une méthode de résolution matricielle particulière: appeler la fonction correspondante. Par exemple <strong>conjgrad(A,B,1e-8)</strong> pour le gradient conjugué.
</li>
</ul>

Quelques exemples avec les temps de calcul associés: [http://scicomp.stackexchange.com/questions/1001/how-does-the-matlab-backslash-operator-solve-ax-b-for-square-matrices](http://scicomp.stackexchange.com/questions/1001/how-does-the-matlab-backslash-operator-solve-ax-b-for-square-matrices)

#### Comment calculer les zéros des polynômes de Legendre?

Si on définit la fonction suivante dans le fichier <strong>leg.m</strong> (pour polynômes de Legendre associés à 2 indices n et m):

<dl >
<dt>leg.m</dt>
<dd><pre ><span >function</span> leg = leg<span >&#40;</span>n,m,x<span >&#41;</span>
y=[<span >legendre</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#legendrel)<span >&#40;</span>n,x<span >&#41;</span>;
leg=y<span >&#40;</span>m,:<span >&#41;</span>;</pre>
</dd></dl>

Alors par exemple un zéro de <strong>P^1_3</strong> dans l'intervalle <strong>[0.1,0.9]</strong> se calcule de la façon suivante:

<pre >&gt;&gt; n=<span >3</span>;m=<span >1</span>;[<span >fzero</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#fzerol)<span >&#40;</span>@<span >&#40;</span>x<span >&#41;</span> leg<span >&#40;</span>n,m,x<span >&#41;</span>,<span >&#91;</span><span >0.1</span> <span >0.9</span><span >&#93;</span><span >&#41;</span>
&nbsp;
[<span >ans</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#ansl) =
&nbsp;
    <span >0.7746</span></pre>

#### Emplacement du compilateur mex

Si l'exécutable matlab est dans le chemin suivant :

<pre >/usr/local/MATLAB/R2012b/bin/matlab</pre>

Il peut être nécessaire de préciser le chemin complet pour mex. Il est dans le même répertoire :

<pre >/usr/local/MATLAB/R2012b/bin/mex</pre>

#### Tester le multithreading

Ce petit programme peut utiliser 20 threads simultanées (visibles avec la commande “top”) si Matlab est correctement configuré:

<dl >
<dt>threading.m</dt>
<dd><pre ><span >% Benchmarking Ax = b algebraic system of equations with multithreading</span>
&nbsp;
n = <span >8000</span>;         <span >% set matrix size</span>
M = [<span >rand</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#randl)<span >&#40;</span>n<span >&#41;</span>;      <span >% create random matrix</span>
A = M + M';       <span >% create A as a symmetric real matrix</span>
x = [<span >ones</span>](http://www.mathworks.com/access/helpdesk/help/techdoc/ref/#onesl)<span >&#40;</span>n,<span >1</span><span >&#41;</span>;    <span >% define solution x as unity vector</span>
b = A * x;        <span >% compute RHS b from A and x</span>
&nbsp;
display &quot;start&quot;
&nbsp;
y = A\b;                <span >% solves Ay = b; y should equal x</span></pre>
</dd></dl>

<p>&nbsp;</p>

<!-- <<<Matlab MAT-Files>>> -->
## <a name="Matlab MAT-Files"></a> Matlab MAT-Files

(I do not describe the commercial Matlab software here but its file formats, because these are understood by many other programs)

"*MAT-files are double-precision, binary, [MATLAB](#matlab) format files. They can be created on one machine and later read by MATLAB on another machine with a different floating-point format, retaining as much accuracy and range as the different formats allow. They can also be manipulated by other programs external to MATLAB.*"

<ul>
*  Documentation: [http://www.mathworks.com/access/helpdesk/help/pdf_doc/matlab/matfile_format.pdf](http://www.mathworks.com/access/helpdesk/help/pdf_doc/matlab/matfile_format.pdf)

*  Logiciels capables de lire ce format: [Rheolef](#rheolef)

*  Logiciels capables d'écrire dans ce format: [Rheolef](#rheolef)

</ul>

<p>&nbsp;</p>

<!-- <<<Matrix Market Exchange Formats>>> -->
## <a name="Matrix Market Exchange Formats"></a> Matrix Market Exchange Formats

"*The Matrix Market (MM) exchange formats provide a simple mechanism to facilitate the exchange of matrix data. In particular, the objective has been to define a minimal base **ASCII** file format which can be very easily explained and parsed, but can easily adapted to applications with a more rigid structure, or extended to related data objects. The MM exchange format for matrices is really a collection of affiliated formats which share design elements. In our initial specification, two matrix formats are defined.*"

<ul>
*  Web: [http://math.nist.gov/MatrixMarket/#formatsl](http://math.nist.gov/MatrixMarket/#formatsl)

</ul>

<p>&nbsp;</p>

<!-- <<<Maxima>>> -->
## <a name="Maxima"></a> Maxima

"*Maxima is a system for the manipulation of symbolic and numerical expressions, including differentiation, integration, Taylor series, Laplace transforms, ordinary differential equations, systems of linear equations, and vectors, matrices, and tensors. Maxima produces high precision results by using exact fractions and arbitrarily long floating point representations, and can plot functions and data in two and three dimensions.

The Maxima source code can be compiled on many systems, including Windows, Linux, and MacOS X. The source code for all systems and precompiled binaries for Windows and Linux are available at the SourceForge file manager.

Maxima is a descendant of Macsyma, the legendary computer algebra system developed in the late 1960s at the Massachusetts Institute of Technology. It is the only system based on that effort still publicly available and with an active user community, thanks to its open source nature. Macsyma was revolutionary in its day, and many later systems, such as Maple and Mathematica, were inspired by it.*"

### Documentation

[http://maxima.sourceforge.net](http://maxima.sourceforge.net)

<p>&nbsp;</p>

<!-- <<<MayaVi>>> -->
## <a name="MayaVi"></a> MayaVi

"*MayaVi is a free, easy to use scientific data visualizer. It is written in [Python](#python) and uses the amazing Visualization Toolkit ([VTK](#vtk)) for the graphics. It provides a **GUI** written using Tkinter. MayaVi is free and distributed under the conditions of the BSD license. It is also cross platform and should run on any platform where both [Python](#python) and [VTK](#vtk) are available (which is almost any *nix, Mac OSX or Windows).*"

### Web

[http://mayavi.sourceforge.net/](http://mayavi.sourceforge.net/)

### Documentation

[http://mayavi.sourceforge.net/#docsl](http://mayavi.sourceforge.net/#docsl)

### Téléchargement

[http://mayavi.sourceforge.net/#downloadl](http://mayavi.sourceforge.net/#downloadl)

### Exemples

[http://mayavi.sourceforge.net/screenshots/#indexl](http://mayavi.sourceforge.net/screenshots/#indexl)

### Licence

"*MayaVi is free and distributed under the conditions of the BSD license*"

<p>&nbsp;</p>

<!-- <<<Mercurial>>> -->
## <a name="Mercurial"></a> Mercurial

#<!-- <<<FAQ>>> -->
## <A NAME="FAQ"></A> FAQ

#### Which diff3 software to use for merging?
<ul>
*  [kdiff3](http://kdiff3.sourceforge.net/) is available for Linux, Windows and MacOS (through [Macports](http://www.macports.org) or as a standalone binary).

*  Specific for MacOS: FileMerge [Using FileMerge as a diff command for Subversion (and Mercurial)](http://www.defraine.net/~brunod/fmdiff)

</ul>

#### Merging development heads

To see the different heads:

<pre >hg heads</pre>

To merge two heads:

<pre >hg merge
hg commit -m &quot;commit message&quot;</pre>

<em >note*: hg merge may ask to specify a version reference for each head (with *-r version_number*) if there is an ambiguity.

### How to view all changes as a graphical tree?

To view the tree in a text terminal:

<pre >hg glog</pre>

This requires the following lines to be added to the Mercurial configuration file:

<pre >[extensions]
graphlog = </pre>

<p>&nbsp;</p>

<!-- <<<METIS>>> -->
## <A NAME="METIS"></A> METIS

"*METIS is a family of programs for partitioning unstructured graphs and hypergraphs and computing fill-reducing orderings of sparse matrices. The underlying algorithms used by METIS are based on the state-of-the-art multilevel paradigm that has been shown to produce high quality results and scale to very large problems.*"

### Web

[http://glaros.dtc.umn.edu/gkhome/views/metis/](http://glaros.dtc.umn.edu/gkhome/views/metis/)

<p>&nbsp;</p>

<!-- <<<mpi>>> -->
## <a name="mpi"></a> MPI
    
"*MPI is a library specification for message-passing, proposed as a standard by a broadly based committee of vendors, implementors, and users.*"

*Reference:* [http://www.mcs.anl.gov/mpi/www](http://www.mcs.anl.gov/mpi/www)
*Voir aussi:* [BSP](#bsp).

<p>&nbsp;</p>

<!-- <<<MUMPS>>> -->
## <A NAME="MUMPS"></A> MUMPS

"*MUMPS: a MUltifrontal Massively Parallel sparse direct Solver*"

[Fiche PLUME](http://www.projet-plume.org/fiche/mumps)

<p>&nbsp;</p>

<!-- <<<NAPACK>>> -->
## <A NAME="NAPACK"></A> NAPACK

"*NAPACK is a collection of [Fortran](#fortran) subroutines for doing numerical linear algebra and optimization. It may be used to solve linear systems, to estimate the condition number or the norm of a matrix, to compute determinants, to multiply a matrix by a vector, to invert a matrix, to solve least squares problems, to perform unconstrained minimization, to compute eigenvalues, eigenvectors, the singular value decomposition, or the QR decomposition. The package has special routines for general, band, symmetric, indefinite, tridiagonal, upper Hessenberg, and circulant matrices.*"

### Web

[http://www.netlib.org/napack/](http://www.netlib.org/napack/)

<p>&nbsp;</p>

<!-- <<<NCO>>> -->
## <A NAME="NCO"></A> NCO

"*The NetCDF Operators, or NCO, are a suite of programs known as operators. Each operator is a standalone, command line program which is executed at the UNIX (or NT) shell-level like, e.g., ls or mkdir. The operators take NetCDF or [HDF](#hdf)4 files as input, then perform a set of operations (e.g., deriving new data, averaging, hyperslabbing, or metadata manipulation) and produce a NetCDF file as output. The operators are primarily designed to aid manipulation and analysis of gridded scientific data. The single command style of NCO allows users to manipulate and analyze files interactively and with simple scripts, avoiding the overhead (and some of the power) of a higher level programming environment. The NCO User's Guide illustrates their use with examples from the field of climate modeling and analysis.*

*The operators are as general as NetCDF itself: there are no restrictions on the contents of the NetCDF or [HDF](#hdf)4 file(s) used as input. The internal routines of NCO are completely dynamic which means that NCO imposes no limit on the number of dimensions, sizes of variables, files etc. NCO is designed to be used both interactively and with large batch jobs. There are plenty of command line (i.e., runtime) options, but the defaults settings are often sufficient for everyday needs. NCO works on AIX, IRIX, Linux, SunOS, Solaris, tru64, UNICOS, and Windows NT. The following operators are thoroughly described in the NCO User's Guide. Note that the “averagers” are misnamed because they can perform many non-linear operations as well, e.g., total, minimum, maximum, RMS.*"

### Web

[http://nco.sourceforge.net/](http://nco.sourceforge.net/)

<p>&nbsp;</p>

<!-- <<<Netgen>>> -->
## <a name="Netgen"></a> Netgen

"*NETGEN is an automatic 3d tetrahedral mesh generator. It accepts input from constructive solid geometry (CSG) or boundary representation (BRep) from [STL file format](#stl_file_format).  The connection to a geometry kernel allows the handling of [IGES](#iges) and [STEP](#step) files. NETGEN contains modules for mesh optimization and hierarchical mesh refinement. Netgen is open source based on the [LGPL license](#licences_pour_logiciels_libres). It is available for Unix/Linux and Windows.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/netgen)

### Format de données standard lus

[STL file format](#stl_file_format), [IGES](#iges) and [STEP](#step).

<p>&nbsp;</p>

<!-- <<<ngsolve>>> -->
## <a name="ngsolve"></a> NGSolve

"*NGSolve is a general purpose 3D finite element solver. Version 1.x supports scalar (heat flow), elasticity and magnetic field
problems. The package provides [C++](#cxx) source code such that more advanced problem solvers can be built around it. NGSolve performs
adaptive mesh refinement, the matrix equations are solved by optimal order multigrid methods.*"
    
<p>&nbsp;</p>

<!-- <<<NIST Sparse BLAS>>> -->
## <a name="NIST Sparse BLAS"></a> NIST Sparse BLAS

"*This page contains software for various libaries developed at NIST for the Sparse Basic Linear Algebra Subprograms ([BLAS](#blas)), which describes kernels operations for sparse vectors and matrices. The current distribution adheres to the ANSI [C](#c) interface of the [BLAS](#blas) Technical Forum Standard. Older libraries corresponding to previous designs are also included for archival and historical purposes.*"

### Web

[http://math.nist.gov/spblas](http://math.nist.gov/spblas)

### Documentation

[BLAS Technical Forum Standard](http://www.netlib.org/blas/blast-forum)

<p>&nbsp;</p>

<!-- <<<nohup>>> -->
## <a name="nohup"></a> nohup

exécute une commande en la rendant insensible aux déconnexions et stocke les résultats dans le fichier <strong>nohup.out</strong> :

<pre >nohup &lt;programme&gt; &amp;</pre>
<ul>
*  [FreeFem++](#freefem) :

</ul>
<pre >nohup FreeFem++-nw &lt;programme&gt;.edp &amp;</pre>
<ul>
*  [Matlab](#matlab) :

</ul>
<pre >nohup matlab -nodisplay -r commande &amp;</pre>
<ul>
*  [Scilab](#scilab) :

</ul>
<pre >nohup scilab -nw -f &lt;programme&gt;.sce &amp;</pre>

#<!-- <<<Interrompre un calcul lancé avec nohup>>> -->
## <a name="Interrompre un calcul lancé avec nohup"></a> Interrompre un calcul lancé avec nohup

Les calculs lancés en tâche de fond ne peuvent pas être stoppés avec Control-C. Il faut utiliser les commandes <strong>kill</strong> ou <strong>killall</strong>. Exemple : stopper les calculs [Matlab](#matlab) en cours sur gpu1:

<pre >killall MATLAB</pre>

(<em >NB:* ceci n'a *<em >aucun effet** sur les calculs Matlab lancés par les autres utilisateurs de la machine)

Pour interrompre un calcul précis, il faut connaître son identifiant (numéro compris entre 1 et 65536), avec la commande :

<pre >top</pre>

(L'identifiant se trouve dans la colonne de droite). Pour stopper un calcul :

<pre >kill &lt;identifiant&gt;</pre>

<p>&nbsp;</p>

<!-- <<<NSC2KE>>> -->
## <A NAME="NSC2KE"></A> NSC2KE

"*NSC2KE est un solveur Volumes-Finis-Galerkin pour le calcul d'écoulements 2D et axisymetriques utilisant des maillages non-structurés. Pour résoudre la partie Euler des equations, le flux de Roe, de Osher et un flux cinetique sont disponibles. Pour le calcul d'écoulements turbulents un modéle k-epsilon est disponible. La modélisation à bas nombre de Reynolds s'effectue soit par une technique bi-couche, soit à travers des lois de paroi. L'utilisation d'un shéma Runge-Kutta à 4 pas permet aussi la résolution de problèmes instationnaires.*"

[http://www.abbesazzi.com/nsc2ke-2](http://www.abbesazzi.com/nsc2ke-2) contient une présentation du logiciel et le code source.

NSC2KE utilise les maillages générés par [Bamg](#bamg) ou EMC2.

<p>&nbsp;</p>

<!-- <<<Octave>>> -->
## <a name="Octave"></a> Octave

"*GNU Octave is a high-level language, primarily intended for numerical computations. It provides a convenient command line interface for solving linear and nonlinear problems numerically, and for performing other numerical experiments using a language that is mostly compatible with [Matlab](#matlab). It may also be used as a batch-oriented language.

Octave has extensive tools for solving common numerical linear algebra problems, finding the roots of nonlinear equations, integrating ordinary functions, manipulating polynomials, and integrating ordinary differential and differential-algebraic equations. It is easily extensible and customizable via user-defined functions written in Octave's own language, or using dynamically loaded modules written in [C++](#cxx), [C](#c), [Fortran](#fortran), or other languages.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/octave)

### Documentation

[http://www.octave.org/doc/interpreter/](http://www.octave.org/doc/interpreter/)

### Informations sur les formats de données

[Gnuplot](#gnuplot) is used for plotting.

<p>&nbsp;</p>

<!-- <<<OFELI>>> -->
## <A NAME="OFELI"></A> OFELI

"*OFELI (Object Finite Element LIbrary) is an object oriented library of [C++](#cxx) classes for development of finite element codes. Its main features are :*

* *Various storage schemes of matrices (dense, sparse, skyline, tridiagonal).*
* *Direct methods and preconditioned iterative strategies for the solution of linear systems of equations.*
* *Shape functions of most “popular” finite elements*
* *Element arrays of most popular problems (Heat Transfer, Fluid Flow, Solid Mechanics, Electromagnetics, …).*

*The OFELI package is not only a library of classes for Finite Element developments. The package contains in addition :*

* *A guided tutorial to learn how to use and develop finite element codes using the library*
* *More elaborated codes for various types of problems*
* *An extensive documentation in PDF and **HTML** formats*
* *Utility programs to convert mesh and output files and to generate simple meshes*"

### Web

[http://ofeli.sourceforge.net/](http://ofeli.sourceforge.net/)

### Licence

[GPL](#licences_pour_logiciels_libres)

<p>&nbsp;</p>

<!-- <<<OFF>>> -->
## <A NAME="OFF"></A> OFF

"*This format, called OFF (for Object File Format), is general, flexible, and extensible. It supports **ASCII** text versions of objects for the purpose of interchange, and binary versions for efficiency of reading and writing.*"

### Documentation

### Logiciels capables de lire ce format

[Geomview](#geomview)

### Logiciels capables d'écrire dans ce format

[ADMesh](#admesh)

<p>&nbsp;</p>

<!-- <<<OOFEM>>> -->
## <A NAME="OOFEM"></A> OOFEM

"*OOFEM is free finite element code with object oriented architecture for solving mechanical, transport and fluid mechanics problems that operates on various platforms.*

*The aim of this project is to develop efficient and robust tool for FEM computations as well as to provide modular and extensible environment for future development.*"

### Web

[http://www.oofem.org/](http://www.oofem.org/)

### Documentation

[http://www.oofem.org/en/features/#featuresl](http://www.oofem.org/en/features/#featuresl),

[http://www.oofem.org/en/documentation/#manuall](http://www.oofem.org/en/documentation/#manuall)

### Téléchargement

[http://www.oofem.org/en/download/#downloadl](http://www.oofem.org/en/download/#downloadl)

### Exemples

[http://www.oofem.org/en/gallery/#galleryl](http://www.oofem.org/en/gallery/#galleryl)

### Licence

[http://www.oofem.org/en/license/#licensel](http://www.oofem.org/en/license/#licensel)

<p>&nbsp;</p>

<!-- <<<opendx>>> -->
## <a name="opendx"></a> OpenDX

"*OpenDX gives you new control over your data…and new insights into their meaning.  Yet OpenDX is easy to use because it lets you visualize
data in ways you've never dreamed of–without getting bogged down in the technology.*

*As its name implies, OpenDX is Open Source. The license allows you to freely create, distribute, and develop visualization solutions as you
see fit.*
	    
*OpenDX is a uniquely powerful, full-featured software package for the visualization of scientific, engineering and analytical data: Its
open system design is built on a standard interface environments. And its sophisticated data model provides users with great flexibility in
creating visualizations.*
	    
*With OpenDX, you can create the visualizations you want to create. OpenDX has been designed to be the place where the art of science and
the science of visualization come together. It's the place where they're combined into one powerful, flexible framework that lets you
“Simply Visualize.”*"
	    
<p>&nbsp;</p>

<!-- <<<Open Dynamics Engine>>> -->
## <a name="Open Dynamics Engine"></a> Open Dynamics Engine

"*ODE is an open source, high performance library for simulating rigid body dynamics. It is fully featured, stable, mature and platform independent with an easy to use [C](#c)/[C++](#cxx) **API**. It has advanced joint types and integrated collision detection with friction. ODE is useful for simulating vehicles, objects in virtual reality environments and virtual creatures. It is currently used in many computer games, 3D authoring tools and simulation tools.*"

### Web

[http://www.ode.org](http://www.ode.org)

### Documentation

[user guide](http://www.ode.org/ode-latest-#userguidel),

[slides](http://www.ode.org/slides/parc/#indexl)

### Licence

"*ODE's [BSD license](#licences_pour_logiciels_libres) allows you to use the source code free of charge in your commercial products.*"

<p>&nbsp;</p>

<!-- <<<openfem>>> -->
## <a name="openfem"></a> OpenFEM

"*OpenFEM is a finite element toolbox designed to be used within a matrix computing environment.  It is available for both [Matlab](#matlab)
and [Scilab](#scilab). So far, OpenFEM has been jointly developed by INRIA and SDTools, based on the existing software packages Modulef and
SDT (Structural Dynamics Toolbox). External contributions are strongly encouraged for the forthcoming versions in order to enlarge and
improve the toolbox.*"

<p>&nbsp;</p>

<!-- <<<openfoam>>> -->
## <a name="openfoam"></a> OpenFOAM
	  
"*The OpenFOAM (Open Field Operation and Manipulation) CFD Toolbox can simulate anything from complex fluid flows involving chemical
reactions, turbulence and heat transfer, to solid dynamics, electromagnetics and the pricing of financial options.*
	    
*The core technology of OpenFOAM is a flexible set of efficient [C++](#cxx) modules. These are used to build a wealth of: solvers, to
simulate specific problems in engineering mechanics; utilities, to perform pre- and post-processing tasks ranging from simple data
manipulations to visualisation and mesh processing; libraries, to create toolboxes that are accessible to the solvers/utilities, such as
libraries of physical models.*
	    
*OpenFOAM is supplied with numerous pre-configured solvers, utilities and libraries and so can be used like any typical simulation
package. However, it is open, not only in terms of source code, but also in its structure and hierarchical design, so that its solvers,
utilities and libraries are fully extensible.*
	    
*OpenFOAM uses finite volume numerics to solve systems of partial differential equations ascribed on any 3D unstructured mesh of polyhedral
cells. The fluid flow solvers are developed within a robust, implicit, pressure-velocity, iterative solution framework, although alternative
techniques are applied to other continuum mechanics solvers. Domain decomposition parallelism is fundamental to the design of OpenFOAM and
integrated at a low level so that solvers can generally be developed without the need for any 'parallel-specific' coding. *"

### Web

[http://www.opencfd.co.uk](http://www.opencfd.co.uk)

<p>&nbsp;</p>

<!-- <<<OpenMP>>> -->
## <a name="OpenMP"></a> OpenMP

"*OpenMP is a specification for a set of compiler directives, library routines, and environment variables that can be used to specify shared memory parallelism in [Fortran](#fortran) and [C](#c)/[C++](#cxx) programs.*"

<ul>
*  Web: [http://www.openmp.org/](http://www.openmp.org/)

</ul>

<p>&nbsp;</p>

<!-- <<<OpenSees>>> -->
## <a name="OpenSees"></a> OpenSees

"*[…] OpenSees, a software framework for developing applications to simulate the performance of structural and geotechnical systems subjected to earthquakes.*

*The goal of the OpenSees development is to improve the modeling and computational simulation in earthquake engineering through open-souce development. *"

### Web

[http://opensees.berkeley.edu/](http://opensees.berkeley.edu/)

### Documentation

[http://opensees.berkeley.edu/OpenSees/manuals/usermanual/#indexl](http://opensees.berkeley.edu/OpenSees/manuals/usermanual/#indexl),

[http://opensees.berkeley.edu/OpenSees/manuals/ExamplesManual/HTML/](http://opensees.berkeley.edu/OpenSees/manuals/ExamplesManual/HTML/)

<p>&nbsp;</p>

<!-- <<<ParaView>>> -->
## <a name="ParaView"></a> ParaView

"*Welcome to ParaView, an application designed with the need to visualize large data sets in mind. The goals of the ParaView project include the following:*

<ul>
*  *Develop an open-source, multi-platform visualization application.*

*  *Support distributed computation models to process large data sets.*

*  *Create an open, flexible, and intuitive user interface.*

*  *Develop an extensible architecture based on open standards.*

</ul>

*ParaView runs on distributed and shared memory parallel as well as single processor systems and has been succesfully tested on Windows, Linux and various Unix workstations and clusters. Under the hood, ParaView uses the [Visualization Toolkit](#vtk) as the data processing and rendering engine and has a user interface written using a unique blend of Tcl/Tk and [C++](#cxx).*"

[Fiche PLUME](http://www.projet-plume.org/fiche/paraview)

### Questions/Réponses

#### Comment relire un fichier de données VTK en dehors de Paraview?

Avec l'interface Python/VTK dont de nombreux exemples sont à [http://www.vtk.org/Wiki/VTK/Examples/Python](http://www.vtk.org/Wiki/VTK/Examples/Python)

#### Comment sauvegarder une image?

Menu “File/Save Screenshot…”

See also [http://www.paraview.org/Wiki/ParaView/Users_Guide/Saving_Data](http://www.paraview.org/Wiki/ParaView/Users_Guide/Saving_Data)

#### Comment changer le titre de la barre de couleurs?

Cliquer sur l'icône “Edit Color Map” qui se situe à côté de l'outil de barre des couleurs.

#### Comment changer les couleurs par défaut?

Menu “Edit/Settings…/Colors”

<p>&nbsp;</p>

<!-- <<<PARI/GP>>> -->
## <A NAME="PARI/GP"></A> PARI/GP

"* PARI/GP is a widely used computer algebra system designed for fast computations in number theory (factorizations, algebraic number theory, elliptic curves…), but also contains a large number of other useful functions to compute with mathematical entities such as matrices, polynomials, power series, algebraic numbers etc., and a lot of transcendental functions. PARI is also available as a [C](#c) library to allow for faster computations.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/pari-gp)

### Documentation

[http://pari.math.u-bordeaux.fr/#docl](http://pari.math.u-bordeaux.fr/#docl)

<p>&nbsp;</p>

<!-- <<<pARMS>>> -->
## <a name="pARMS"></a> pARMS

"*pARMS: parallel Algebraic Recursive Multilevel Solvers*

*pARMS is a library of parallel solvers for distributed sparse linear systems of equations. It is based on a preconditioned Krylov subspace approach, using a domain decomposition viewpoint. It offers a large selection of preconditioners for distributed sparse linear systems and a few of the best known accelerators. The basic methodology used relies on a Recursive Multi-level ILU factorization wich allows to develop many of the standard domain-decomposition type iterative solvers in a single framework. For example, the standard Schwarz procedures are included as are a number of Schur complement techniques.*"

### Web

[http://www-users.cs.umn.edu/~saad/software/pARMS/](http://www-users.cs.umn.edu/~saad/software/pARMS/)

<p>&nbsp;</p>

<!-- <<<PBLAS>>> -->
## <A NAME="PBLAS"></A> PBLAS

"*Parallel Basic Linear Algebra Subprograms (PBLAS)*"

### Web

[http://www.netlib.org/scalapack/#pblas_qrefl](http://www.netlib.org/scalapack/#pblas_qrefl)

<p>&nbsp;</p>

<!-- <<<Perl>>> -->
## <a name="Perl"></a> Perl

Perl is a general-purpose scripting language, like Tcl/Tk and [Python](#python). Il existe une [version pour Windows.](http://www.activestate.com/Products/ActivePerl)

### Documentation

Initiation : [http://www.comp.leeds.ac.uk/Perl/#startl](http://www.comp.leeds.ac.uk/Perl/#startl)

Référence : [http://www.perl.com/pub/q/documentation](http://www.perl.com/pub/q/documentation)

Opérateurs de test sur les fichiers : [http://www.cs.cf.ac.uk/Dave/PERL/#node69l](http://www.cs.cf.ac.uk/Dave/PERL/#node69l)

### Questions/Réponses

#### Comment extraire les informations importantes dans un nom de fichier

Voici par exemple un fichier dont le nom contient une valeur de vitesse. L'emplacement des parenthèses dans l'expression régulière permet
d'isoler l'information importante :

<pre >&gt; echo resultats_v=2.txt|perl -e 'while(&lt;&gt;){/resultats_v=(.*)\.txt/;print &quot;$1\n&quot;;}'
2</pre>

Un autre exemple avec plusieurs informations à extraire :

<pre >&gt; echo resultats_v=2_c=3.txt|perl -e 'while(&lt;&gt;){/resultats_v=(.*)_c=(.*)\.txt/;print &quot;v=$1 c=$2\n&quot;;}'
v=2 c=3</pre>

<p>&nbsp;</p>

<!-- <<<PETSc>>> -->
## <a name="PETSc"></a> PETSc

"*PETSc, the Portable, Extensible Toolkit for Scientific computation, provides sets of tools for the parallel (as well as serial), numerical solution of PDEs that require solving large-scale, sparse nonlinear systems of equations. PETSc includes nonlinear and linear equation solvers that employ a variety of Newton techniques and Krylov subspace methods. PETSc provides several parallel sparse matrix formats, including compressed row, block compressed row, and block diagonal storage.

PETSc is fully usable from [Fortran](#fortran), [C](#c) and [C++](#cxx), and is portable, running on most UNIX systems. PETSc uses [MPI](#mpi) for all parallel communication.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/petsc)

<p>&nbsp;</p>

<!-- <<<PLAPACK>>> -->
## <A NAME="PLAPACK"></A> PLAPACK

"*Coding parallel algorithms is generally regarded as a formidable task. To make this task manageable in the arena of linear algebra algorithms, we have developed the Parallel Linear Algebra Package (PLAPACK), an infrastructure for coding such algorithms at a high level of abstraction. It is often believed that by raising the level of abstraction in this fashion, performance is sacrificed. Throughout, we have maintained that indeed there is a performance penalty, but that by coding at a higher level of abstraction, more sophisticated algorithms can be implemented, which allows high levels of performance to be regained. In this paper, we show this to indeed be the case for the parallel solver package implemented using PLAPACK, which includes Cholesky, LU, and QR factorization based solvers for symmetric positive definite, general, and overdetermined systems of equations, respectively. Performance comparison with [ScaLAPACK](#scalapack) shows better performance is attained by our solvers.*"

### Web

[http://www.cs.utexas.edu/users/plapack/](http://www.cs.utexas.edu/users/plapack/)

### Documentation

[Overview](http://www.cs.utexas.edu/users/plapack/icpp98/#indexl),

[Users' Guide](http://www.cs.utexas.edu/users/plapack/Guide/G#uide_htmll)

### Exemples

[http://www.cs.utexas.edu/users/plapack/Code](http://www.cs.utexas.edu/users/plapack/Code)

<p>&nbsp;</p>

<!-- <<<Plotmtv>>> -->
## <a name="Plotmtv"></a> Plotmtv

"*The application plotmtv is a fast multi-purpose plotting program for visualization of scientific data in an X11-window environment. Each plot comes with a simple but functional Graphical User Interface which allows users to zoom in or pan to areas of interest on the plot or to toggle between 2D and 3D plots.*"

### Documentation

 Tutorial at [http://cauchy.math.colostate.edu/workshop/Plotmtv/#plotmtvl](http://cauchy.math.colostate.edu/workshop/Plotmtv/#plotmtvl)

<p>&nbsp;</p>

<!-- <<<POOMA>>> -->
## <A NAME="POOMA"></A> POOMA

"*POOMA is a high-performance [C++](#cxx) toolkit for parallel scientific computation. POOMA's object-oriented design facilitates rapid application development. POOMA has been optimized to take full advantage of massively parallel machines. POOMA is available free of charge in order to facilitate its use in both industrial and research environments.*"

### Web

[http://www.nongnu.org/freepooma/](http://www.nongnu.org/freepooma/)

### Documentation

[tutorial](http://www.nongnu.org/freepooma/tutorial/#indexl),

### Téléchargement

[http://savannah.nongnu.org/download/freepooma/](http://savannah.nongnu.org/download/freepooma/)

### Licence

"*FreePOOMA is free software; you can redistribute it and/or modify it under the terms of the Expat license. See LICENSE, LICENSE.pooma and LICENSE.pete for more information.  *"

<p>&nbsp;</p>

<!-- <<<Povray>>> -->
## <a name="Povray"></a> Povray

"*The Persistence of Vision Raytracer is a high-quality, totally free tool for creating stunning three-dimensional graphics. It is available in official versions for Windows, Mac **OS**/Mac **OS** X and i86 Linux. The source code is available for those wanting to do their own ports.*"

<ul>
*  Web: [http://www.povray.org/](http://www.povray.org/)

*  Documentation: [http://www.povray.org/documentation/](http://www.povray.org/documentation/)

*  Licence: [http://www.povray.org/#povlegall](http://www.povray.org/#povlegall)

</ul>

<p>&nbsp;</p>

<!-- <<<PRIMME>>> -->
## <A NAME="PRIMME"></A> PRIMME

"*PRIMME (PReconditioned Iterative MultiMethod Eigensolver)*

<ul>
*  *PRIMME is a [C](#c) library to find a number of eigenvalues and their corresponding eigenvectors of a Real Symmetric, or Complex Hermitian matrix A.*

</ul>
<ul>
*  *Preconditioning and finding largest, smallest or interior eigenvalues is supported.*

</ul>
<ul>
*  *PRIMME is a multimethod eigensolver. Based on Davidson/Jacobi-Davidson main iteration, it can transform to most known preconditioned eigensolvers, by the appropriate choice of parameters. Two of the choices, GD+1 and JDQMR, have proved nearly optimal eigensolvers (see 1,2). For user friendliness it provides the following predefined choices of methods.*

</ul>

### Web

[http://www.cs.wm.edu/~andreas/software](http://www.cs.wm.edu/~andreas/software)

### Licence

"*Available under the [Lesser GPL license](#licences_pour_logiciels_libres)*"

<p>&nbsp;</p>

<!-- <<<PRISM>>> -->
## <A NAME="PRISM"></A> PRISM

"*The goal of the PRISM (Parallel Research on Invariant Subspace Methods) project is to develop infrastructure and algorithms for the parallel solution of eigenvalue problems. We are currently investigating a complete eigensolver based on the Invariant Subspace Decomposition Algorithm for dense symmetric matrices (SYISDA).*"

### Web

[http://www-unix.mcs.anl.gov/prism/](http://www-unix.mcs.anl.gov/prism/)

### Documentation

[Introduction](http://www-unix.mcs.anl.gov/prism/lib/#introl),

[Hightlights and Performance](http://www-unix.mcs.anl.gov/prism/lib/#highlightl),

[Users' Guide](http://www-unix.mcs.anl.gov/prism/lib/techsrc/UsersGuide.ps)

<p>&nbsp;</p>

<!-- <<<pthreads>>> -->
## <a name="pthreads"></a> Pthreads

"*Historically, hardware vendors have implemented their own proprietary versions of threads. These implementations differed substantially
from each other making it difficult for programmers to develop portable threaded applications.*

*In order to take full advantage of the capabilities provided by threads, a standardized programming interface was required. For UNIX
systems, this interface has been specified by the IEEE POSIX 1003.1c standard (1995). Implementations which adhere to this standard are
referred to as POSIX threads, or Pthreads. Most hardware vendors now offer Pthreads in addition to their proprietary **API**'s.*

*Pthreads are defined as a set of [C](#c) language programming types and procedure calls, implemented with a pthread.h header/include file
and a thread library - though the this library may be part of another library, such as libc.*

*There are several drafts of the POSIX threads standard. It is important to be aware of the draft number of a given implementation, because
there are differences between drafts that can cause problems.*"
    
<p>&nbsp;</p>

<!-- <<<Python>>> -->
## <a name="Python"></a> Python

Python is a general-purpose scripting language, like Tcl/Tk and [Perl](#perl).

<ul>
<li > [Fiche PLUME](http://www.projet-plume.org/fiche/python)
</li>
<li > Documentation: [The Python Tutorial](http://docs.python.org/tutorial), [http://www.python.org/doc](http://www.python.org/doc)
</li>
<li > NumPy: "*NumPy is the fundamental package for scientific computing with Python.*" [http://www.numpy.org](http://www.numpy.org)
</li>
</ul>

### Questions/Réponses

#### Multithreading

Le multithreading est activé par “import threading”. Voir aussi [http://docs.python.org/library/#threadingl#module-threading](http://docs.python.org/library/#threadingl#module-threading) pour la liste des commandes et objets disponibles.

<p>&nbsp;</p>

<!-- <<<Commande de soumission de travaux &quot;qsub&quot;>>> -->
## <a name="Commande de soumission de travaux &quot;qsub&quot;"></a> Commande de soumission de travaux &quot;qsub&quot;

#<!-- <<<Questions/Réponses>>> -->
## <a name="Questions/Réponses"></a> Questions/Réponses

#### Comment assurer qu'un script soumis à qsub va être exécuté dans le répertoire où il a été soumis?

Par défault, un script est exécuté dans un répertoire temporaire différent du répertoire où il a été soumis. Pour changer ce comportement, ajouter au début du script:

<pre >cd $PBS_O_WORKDIR</pre>

#### Comment spécifier le nombre de processeurs à un seul endroit dans un script qsub?

Le nombre de processeurs demandés doit être écrit explicitement au moins une fois:

<pre >#PBS -l ncpus=18</pre>

Mais dans les lignes suivantes, ce nombre de processeurs peut être remplacé par <strong>$NCPUS</strong>. Par exemple:

<pre >mpirun -np $NCPUS ...</pre>

<p>&nbsp;</p>

<!-- <<<questions_reponses_langages_compiles>>> -->
## <a name="questions_reponses_langages_compiles"></a> Questions/Réponses sur les langages compilés

### Comment observer une fuite de mémoire?

Les fuites de mémoires arrivent le plus souvent quand tous les <strong>malloc()</strong> ne sont pas suivis par un <strong>free()</strong>. On observe, soit dans le Gestionnaire des tâches Windows ou MacOS, soit avec l'utilitaire Unix “top”, que le programme demande de plus en plus de RAM. S'il en demande trop, l'ordinateur peut bloquer. Dans l'exemple ci-dessous avec top, c'est la colonne “VIRT” (comme mémoire virtuelle) qui augmente avec le temps:

<pre >top - 10:25:38 up 5 days, 13 min, 10 users,  load average: 0,64, 0,51, 0,59
Tasks: 224 total,   1 running, 223 sleeping,   0 stopped,   0 zombie
%Cpu(s):  4,0 us,  2,8 sy,  0,0 ni, 92,7 id,  0,4 wa,  0,0 hi,  0,0 si,  0,0 st
KiB Mem:   8195840 total,  7593824 used,   602016 free,   758696 buffers
KiB Swap: 16777212 total,      284 used, 16776928 free,  2089788 cached

  PID USER      PR  NI  VIRT  RES  SHR S  %CPU %MEM    TIME+  COMMAND                     
14945 root      20   0  527m 297m  92m S  19,1  3,7 216:05.06 Xorg                        
    1 root      20   0 10636  760  648 S   0,0  0,0   0:05.24 init                        
    2 root      20   0     0    0    0 S   0,0  0,0   0:00.26 kthreadd                    
    3 root      20   0     0    0    0 S   0,0  0,0   0:06.51 ksoftirqd/0                 
    6 root      rt   0     0    0    0 S   0,0  0,0   0:00.00 migration/0                 
    7 root      rt   0     0    0    0 S   0,0  0,0   0:01.01 watchdog/0                  
    8 root      rt   0     0    0    0 S   0,0  0,0   0:00.00 migration/1                 
   10 root      20   0     0    0    0 S   0,0  0,0   0:06.20 ksoftirqd/1                 
   12 root      rt   0     0    0    0 S   0,0  0,0   0:00.73 watchdog/1                  
   13 root      rt   0     0    0    0 S   0,0  0,0   0:00.00 migration/2                 
   15 root      20   0     0    0    0 S   0,0  0,0   0:06.32 ksoftirqd/2                 
   16 root      rt   0     0    0    0 S   0,0  0,0   0:00.94 watchdog/2                  
   17 root      rt   0     0    0    0 S   0,0  0,0   0:00.00 migration/3                 
   19 root      20   0     0    0    0 S   0,0  0,0   0:06.56 ksoftirqd/3                 
   20 root      rt   0     0    0    0 S   0,0  0,0   0:00.68 watchdog/3                  
   21 root       0 -20     0    0    0 S   0,0  0,0   0:00.00 cpuset                      
   22 root       0 -20     0    0    0 S   0,0  0,0   0:00.00 khelper                     
   23 root      20   0     0    0    0 S   0,0  0,0   0:00.00 kdevtmpfs                   
   24 root       0 -20     0    0    0 S   0,0  0,0   0:00.00 netns                       </pre>

### Comment écrire des lignes différentes pour Windows, MacOS et Linux dans le même programme C?
<pre >#ifdef __linux__
   ...lignes valables uniquement sous linux...
#endif</pre>
<pre >#ifdef WIN32
   ...lignes valables uniquement sous Windows...
#endif</pre>
<pre >#ifdef __APPLE__
   ...lignes valables uniquement sous MacOS...
#endif</pre>

### How to check what symbols a compiled object contains?

On linux-type systems, use nm. <strong>T</strong> shows defined symbols, <strong>U</strong> shows undefined ones. eg:

<pre >&gt; nm prettyedp-env.o 
                 U _Unwind_Resume
0000000000000000 T _Z12getoneenvvarSs
00000000000003dc T _Z12readabledatev
                 U _Z7loggingbSs
                 U _Z7pathsepv
00000000000000b2 T _Z9envchangeSsSsbb
                 U _ZNKSs5c_strEv
                 U _ZNKSs7compareEPKc
                 U _ZNSaIcEC1Ev
                 U _ZNSaIcED1Ev
                 U _ZNSs6appendEPKc
                 U _ZNSs6appendERKSs
                 U _ZNSsC1EPKcRKSaIcE
                 U _ZNSsC1ERKSs
                 U _ZNSsD1Ev
                 U _ZNSsaSEPKc
                 U _ZNSsaSERKSs
0000000000000000 W _ZSteqIcSt11char_traitsIcESaIcEEbRKSbIT_T0_T1_EPKS3_
0000000000000000 W _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_ERKS6_PKS3_
0000000000000000 W _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_ERKS6_S8_
0000000000000030 r _ZZL18__gthread_active_pvE20__gthread_active_ptr
                 U __gxx_personality_v0
                 U getenv
                 U localtime
                 w pthread_cancel
                 U setenv
                 U strftime
                 U time</pre>

<!-- <<<history>>> [[file:history.php]] -->
<script src="//www.ljll.math.upmc.fr/lehyaric/history.php?page=freesoft-infomath" type="text/javascript"></script>

### How to deal with a &quot;segmentation fault&quot; in a compiled program?

The source for the program is needed. First try to locate where this error appears. This is done by adding <strong>-g</strong> when compiling and running the code through [gdb](#gdb). If there is no programming error at the location where the error occurs, it can be the consequence of an earlier error (memory errors may not be detected immediately). If this is the case then [valgrind](http://valgrind.org) may be able to detect where the first error occurred:

<pre >&gt; valgrind ./prettyedp
==7341== Memcheck, a memory error detector
==7341== Copyright (C) 2002-2011, and GNU GPL'd, by Julian Seward et al.
==7341== Using Valgrind-3.7.0 and LibVEX; rerun with -h for copyright info
==7341== Command: ./prettyedp
==7341== 
* prettyedp: error: please specify a file
==7341== 
==7341== HEAP SUMMARY:
==7341==     in use at exit: 85,096 bytes in 2,008 blocks
==7341==   total heap usage: 2,106 allocs, 98 frees, 114,551 bytes allocated
==7341== 
==7341== LEAK SUMMARY:
==7341==    definitely lost: 0 bytes in 0 blocks
==7341==    indirectly lost: 0 bytes in 0 blocks
==7341==      possibly lost: 33,608 bytes in 998 blocks
==7341==    still reachable: 51,488 bytes in 1,010 blocks
==7341==         suppressed: 0 bytes in 0 blocks
==7341== Rerun with --leak-check=full to see details of leaked memory
==7341== 
==7341== For counts of detected and suppressed errors, rerun with: -v
==7341== ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 4 from 4)</pre>

<p>&nbsp;</p>

<!-- <<<questions_reponses_sur_freefem>>> -->
## <a name="questions_reponses_sur_freefem"></a> Questions/Réponses sur FreeFem++

### Numérotation des maillages

Les fichiers maillage .mesh lu à la fois par Medit et par FreeFem++ ne sont pas gérés de la même façon dans les deux logiciels. Medit
affiche des numéros d'éléments (point, triangle) commençant au numéro 1 (comme le fichier) tandis que FreeFem++ commence la numérotation à
zéro, ce qui décale tous les numéros de 1.

### Solveur par défaut pour les problèmes 3D

Les problèmes 3D occupent rapidement toute la RAM d'une machine moyenne (2 Goctets ou plus). [UMFPACK](#umfpack), le solveur par défault de
FreeFem++, n'est pas le bon choix dans ce cas car il demande lui-aussi une portion équivalente de la mémoire. Il vaut mieux utiliser un
solveur plus lent mais peu gourmand en mémoire (CG ou GMRES si la matrice le permet, ou alors un solveur parallèle intégré à FreeFem++ comme
[MUMPS](#mumps)).

### Fichiers de données en format binaire

Le format binaire peut diminuer la taille des fichiers de données numériques produits par FreeFem++ par un facteur 2 environ. Ce n'est pas
forcément mieux que la compression avec un utilitaire comme <strong>zip</strong>. Actuellement le plus simple pour produire un fichier
binaire est d'utiliser le [C++](#cxx). Voici un exemple où le fichier à traduire contient un vecteur : la première ligne contient la taille
du vecteur, les lignes suivantes ses coordonnées.

<pre >
#include &lt;stdio.h&gt;
#include &lt;iostream&gt;
#include &lt;fstream&gt;
using namespace std;

int main(int argc,char *argv[]){

  // Paramètres de la ligne de commande
  if(argc!=3){
    cout&lt;&lt;&quot;./asc2bin in out&quot;&lt;&lt;endl;
    return 1;
  }

  ifstream i(argv[1],ifstream::in);
  if(!i){
    cout&lt;&lt;&quot;problème avec le fichier d'entrée&quot;&lt;&lt;endl;
    return 1;
  }

  FILE *o=fopen(argv[2],&quot;w&quot;);
  if(!o){
    cout&lt;&lt;&quot;problème avec le fichier de sortie&quot;&lt;&lt;endl;
    return 1;
  }

  // lit et réécrit le nombre d'éléments du vecteur
  int n;
  i&gt;&gt;n;
  cout&lt;&lt;n&lt;&lt;&quot; elements&quot;&lt;&lt;endl;

  fwrite(&amp;n,sizeof(int),1,o);

  // lit et réécrit les composantes du vecteur
  for(int j=0;j&lt;n;j++){
    double d;
    i&gt;&gt;d;
    fwrite(&amp;d,sizeof(double),1,o);
  }

  // ferme tous les fichiers
  i.close();
  fclose(o);

  return 0;
}
</pre>

### Différences entre vecteurs et tableaux FreeFem++

Si les vecteurs uh et vh sont définis par

<pre >fespace Vh(Th,P13d);
Vh uh,vh;</pre>

alors

<pre >uh = randreal1();
vh = randreal1();</pre>

interpole la valeur donnée par la fonction randreal1() sur le maillage. La fonction est appelée autant de fois qu'il y a de points d'intégration.

Tandis que

<pre >vh[] = randreal1();
uh[] = randreal1();</pre>

initialise les tableaux avec une valeur constante donnée par un appel unique à randreal1().

### Validation d'un problème 2D avec des résultats numériques 1D déjà connus

Il peut être utile dans certains cas que la description 2D contenue dans un script FreeFem++ donne les mêmes résultats numériques qu'un cas-test 1D déjà validé. Pour cela il suffit de configurer le domaine 2D comme une bande rectangulaire dont les côtés obéissent à une condition aux limites périodique. For more information on how to specify a periodic boundary condition, see the <strong>fespace</strong> keyword.

### A quel moment FreeFem++ effectue-t-il les calculs correspondant à &quot;matrix A=f(...,solver=...)&quot; et &quot;x=A^-1*b&quot;?
<ul>
<li > cas de <strong>CG</strong> et <strong>GMRES</strong> : la résolution itérative a lieu au moment du calcul de x.
</li>
<li > cas de <strong>UMFPACK</strong> : c'est une méthode de résolution directe. La décomposition LU a lieu lors de la définition de A (par un appel à umfpack_di_numeric() dans le fichier C++ ff/src/fflib/UMFPack_Solver.cpp). Le calcul de <strong>x</strong> exploite les matrices triangulaires L et U calculées auparavant.
</li>
<li > autres solveurs : il faut rechercher l'implémentation correspondante de la classe abstraite MatriceMorse&lt;R&gt;::VirtualSolver dans le répertoire src/solver du source C++ de FreeFem++.
</li>
</ul>

### Comment fixer une échelle constante sur plusieurs images successives? (par exemple pour créer un film)

Utiliser <strong>plot(nbiso=…,viso=…)</strong>. Par exemple :

<dl >
<dt>echelle.edp</dt>
<dd><pre ><span >// maillage simple pour l'exemple</span>
mesh M<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span><span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>M,P1<span >&#41;</span><span >;</span>
Vh xh<span >=</span>x<span >;</span>
&nbsp;
<span >// liste d'isovaleurs constantes d'une image à l'autre</span>
<span >int</span> ni<span >=</span><span >4</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> vi<span >&#40;</span><span >4</span><span >&#41;</span><span >;</span>
vi<span >&#91;</span><span >0</span><span >&#93;</span><span >=</span><span >0</span><span >;</span>
vi<span >&#91;</span><span >1</span><span >&#93;</span><span >=</span><span >1</span><span >;</span>
vi<span >&#91;</span><span >2</span><span >&#93;</span><span >=</span><span >2</span><span >;</span>
vi<span >&#91;</span><span >3</span><span >&#93;</span><span >=</span><span >3</span><span >;</span>
&nbsp;
<span >// première image</span>
plot<span >&#40;</span>xh,value<span >=</span><span >1</span>,nbiso<span >=</span>ni,viso<span >=</span>vi<span >&#41;</span><span >;</span>
&nbsp;
<span >// deuxième image avec des valeurs deux fois plus grandes mais la même échelle</span>
xh<span >=</span><span >2</span><span >*</span>x<span >;</span>
plot<span >&#40;</span>xh,value<span >=</span><span >1</span>,nbiso<span >=</span>ni,viso<span >=</span>vi<span >&#41;</span><span >;</span></pre>
</dd></dl>

### Comment changer les couleurs d'un graphique?

utiliser <strong>plot(…,hsv=[…],…)</strong>, comme dans l'exemple suivant (examples++-tutorial/plot.edp):

<dl >
<dt>couleurs.edp</dt>
<dd><pre ><span >int</span> n<span >=</span><span >20</span>,nn<span >=</span>n<span >+</span><span >10</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> xx<span >&#40;</span>nn<span >&#41;</span>,yy<span >&#40;</span>nn<span >&#41;</span><span >;</span>
<span >//  \url{from:   http://en.wikipedia.org/wiki/HSV_color_space} </span>
<span >//The HSV (Hue, Saturation, Value) model, </span>
<span >//   defines a color space in terms of three constituent components:</span>
<span >//</span>
<span >//HSV color space as a color wheel</span>
<span >//Hue, the color type (such as red, blue, or yellow):</span>
<span >//   Ranges from 0-360 (but normalized to 0-100% h ere)</span>
<span >// Saturation, the &quot;vibrancy&quot; of the color: Ranges     from 0-100%</span>
<span >//    The lower the saturation of a color, the more &quot;grayness&quot; is present </span>
<span >//    and the more faded the color will appear.</span>
<span >// Value, the brightness of the color:</span>
<span >//   Ranges from 0-100%</span>
<span >// </span>
real<span >&#91;</span><span >int</span><span >&#93;</span> colorhsv<span >=</span><span >&#91;</span>  <span >// color hsv model</span>
  <span >4</span>.<span >/</span><span >6</span>., <span >1</span> , <span >0.5</span>, <span >// dark blue</span>
  <span >4</span>.<span >/</span><span >6</span>., <span >1</span> , <span >1</span>, <span >//  blue</span>
  <span >5</span>.<span >/</span><span >6</span>., <span >1</span> , <span >1</span>, <span >//  magenta</span>
  <span >1</span>, <span >1</span>. , <span >1</span>, <span >//  red</span>
  <span >1</span>, <span >0.5</span> , <span >1</span> <span >// light red </span>
   <span >&#93;</span><span >;</span>
mesh Th<span >=</span>square<span >&#40;</span><span >5</span>,<span >5</span><span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P2<span >&#41;</span><span >;</span>
Vh uh<span >=</span>x<span >*</span>x<span >+</span>y<span >*</span>y,vh<span >=</span><span >-</span>y<span >^</span><span >2</span><span >+</span>x<span >^</span><span >2</span><span >;</span>
<span >assert</span><span >&#40;</span>n<span >+</span><span >1</span> <span >&lt;</span> nn<span >&#41;</span><span >;</span>
<span >//  compute a cut </span>
<span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;=</span>n<span >;</span>i<span >++</span><span >&#41;</span>
 <span >&#123;</span>
   xx<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >;</span>
   yy<span >&#91;</span>i<span >&#93;</span><span >=</span>uh<span >&#40;</span>real<span >&#40;</span>i<span >&#41;</span><span >/</span>n,real<span >&#40;</span>i<span >&#41;</span><span >/</span>n<span >&#41;</span><span >;</span> <span >// value of uh at point (i/10. , i/10.) </span>
 <span >&#125;</span>
&nbsp;
 plot<span >&#40;</span>Th,uh,<span >&#91;</span>uh,vh<span >&#93;</span>,value<span >=</span><span >true</span>,ps<span >=</span><span >&quot;three.eps&quot;</span>,wait<span >=</span><span >true</span><span >&#41;</span><span >;</span> <span >// plot mesh, isovalue, and vector</span>
 <span >//  zoom on box defined by the two corner points [0.1,0.2] and [0.5,0.6]</span>
 plot<span >&#40;</span>uh,<span >&#91;</span>uh,vh<span >&#93;</span>,bb<span >=</span><span >&#91;</span><span >&#91;</span><span >0.1</span>,<span >0.2</span><span >&#93;</span>,<span >&#91;</span><span >0.5</span>,<span >0.6</span><span >&#93;</span><span >&#93;</span>,wait<span >=</span><span >true</span>,grey<span >=</span><span >1</span>,fill<span >=</span><span >1</span>,value<span >=</span><span >1</span>,ps<span >=</span><span >&quot;threeg.eps&quot;</span><span >&#41;</span><span >;</span>  <span >// in grey with filling</span>
 plot<span >&#40;</span><span >&#91;</span>xx<span >&#40;</span><span >0</span><span >:</span>n<span >&#41;</span>,yy<span >&#40;</span><span >0</span><span >:</span>n<span >&#41;</span><span >&#93;</span>,<span >&#91;</span>xx<span >&#40;</span><span >0</span><span >:</span>n<span >:</span><span >5</span><span >&#41;</span>,yy<span >&#40;</span><span >0</span><span >:</span>n<span >:</span><span >5</span><span >&#41;</span><span >&#93;</span>,ps<span >=</span><span >&quot;likegnu.eps&quot;</span>,wait<span >=</span><span >true</span><span >&#41;</span><span >;</span> <span >//  like gnuplot plot a cut of uh</span>
&nbsp;
 real<span >&#91;</span><span >int</span><span >&#93;</span> viso<span >&#40;</span><span >31</span><span >&#41;</span><span >;</span>
&nbsp;
 <span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span>viso.<span >n</span><span >;</span>i<span >++</span><span >&#41;</span>
   viso<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >*</span><span >0.1</span><span >;</span>
&nbsp;
 plot<span >&#40;</span>uh,viso<span >=</span>viso<span >&#40;</span><span >0</span><span >:</span>viso.<span >n</span><span >-</span><span >1</span><span >&#41;</span>,value<span >=</span><span >1</span>,fill<span >=</span><span >1</span>,wait<span >=</span><span >1</span>,hsv<span >=</span>colorhsv,ps<span >=</span><span >&quot;threehsv.eps&quot;</span><span >&#41;</span><span >;</span></pre>
</dd></dl>

### Comment sauvegarder les graphiques 3D sous forme de fichiers images PNG ou JPEG?

Utiliser [FreeFem++-cs](#freefem_cs).

### Comment connaître les différents numéros d'un même point dans plusieurs maillages superposés?

Grâce à l'interpolation entre les deux maillages:

<dl >
<dt>renumerotation.edp</dt>
<dd><pre ><span >// petit maillage m sous-ensemble du grand maillage M</span>
mesh M<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span><span >&#41;</span><span >;</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;nombre de points dans M=&quot;</span><span >&lt;&lt;</span>M.<span >nv</span><span >&lt;&lt;</span>endl<span >;</span>
mesh m<span >=</span>trunc<span >&#40;</span>M,x<span >&lt;</span><span >.5</span><span >&#41;</span><span >;</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;nombre de points dans m=&quot;</span><span >&lt;&lt;</span>m.<span >nv</span><span >&lt;&lt;</span>endl<span >;</span>
&nbsp;
<span >// matrices d'interpolation entre maillages</span>
fespace EM<span >&#40;</span>M,P1<span >&#41;</span><span >;</span>
fespace Em<span >&#40;</span>m,P1<span >&#41;</span><span >;</span>
matrix m2M<span >=</span>interpolate<span >&#40;</span>EM,Em<span >&#41;</span><span >;</span>
matrix M2m<span >=</span>interpolate<span >&#40;</span>Em,EM<span >&#41;</span><span >;</span>
&nbsp;
<span >// vecteur representant les numeros des points dans le petit maillage</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >&#93;</span> nm<span >&#40;</span>m.<span >nv</span><span >&#41;</span><span >;</span>
nm<span >=</span><span >0</span><span >:</span><span >&#40;</span>m.<span >nv</span><span >-</span><span >1</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// vecteur du grand maillage contenant les numeros des memes points</span>
<span >// dans le petit maillage</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >&#93;</span> nM<span >&#40;</span>M.<span >nv</span><span >&#41;</span><span >;</span>
nM<span >=</span>m2M<span >*</span>nm<span >;</span>
&nbsp;
<span >// verification</span>
<span >// ------------</span>
&nbsp;
<span >// choisit un point dans le grand maillage</span>
<span >int</span> n<span >=</span><span >35</span><span >;</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;numero dans le grand maillage=&quot;</span><span >&lt;&lt;</span>n<span >&lt;&lt;</span>endl<span >;</span>
EM F<span >=</span><span >0</span><span >;</span>
F<span >&#91;</span><span >&#93;</span><span >&#91;</span>n<span >&#93;</span><span >=</span><span >1</span><span >;</span>
plot<span >&#40;</span>F,cmm<span >=</span><span >&quot;F&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// affiche le meme point dans le petit maillage par interpolation</span>
Em f<span >=</span><span >0</span><span >;</span>
f<span >&#91;</span><span >&#93;</span><span >=</span>M2m<span >*</span>F<span >&#91;</span><span >&#93;</span><span >;</span>
plot<span >&#40;</span>f,cmm<span >=</span><span >&quot;interpolate&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// affiche le meme point dans le petit maillage par renumerotation</span>
f<span >=</span><span >0</span><span >;</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;numero dans le petit maillage=&quot;</span><span >&lt;&lt;</span>nM<span >&#40;</span>n<span >&#41;</span><span >&lt;&lt;</span>endl<span >;</span>
f<span >&#91;</span><span >&#93;</span><span >&#91;</span>nM<span >&#40;</span>n<span >&#41;</span><span >&#93;</span><span >=</span><span >1</span><span >;</span>
plot<span >&#40;</span>f,cmm<span >=</span><span >&quot;renumerotation&quot;</span><span >&#41;</span><span >;</span></pre>
</dd></dl>

### Comment trouver la matrice élémentaire sur un élément d'un maillage?

Voici une méthode impliquant un maillage “élémentaire” contenant un seul élément:

<dl >
<dt>element.edp</dt>
<dd><pre ><span >// petit maillage m sous-ensemble du grand maillage M</span>
<span >// m = maillage avec un seul élément (numéro 55 choisi au hasard)</span>
mesh M<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span><span >&#41;</span><span >;</span>
mesh m<span >=</span>trunc<span >&#40;</span>M,M<span >&#40;</span>x,y<span >&#41;</span>.<span >nuTriangle</span><span >==</span><span >55</span><span >&#41;</span><span >;</span>
&nbsp;
<span >cout</span><span >&lt;&lt;</span><span >&quot;nombre de points dans M=&quot;</span><span >&lt;&lt;</span>M.<span >nv</span><span >&lt;&lt;</span>endl<span >;</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;nombre de points dans m=&quot;</span><span >&lt;&lt;</span>m.<span >nv</span><span >&lt;&lt;</span>endl<span >;</span>
&nbsp;
<span >// matrices d'interpolation entre maillages</span>
fespace EM<span >&#40;</span>M,P1<span >&#41;</span><span >;</span>
fespace Em<span >&#40;</span>m,P1<span >&#41;</span><span >;</span>
matrix m2M<span >=</span>interpolate<span >&#40;</span>EM,Em<span >&#41;</span><span >;</span>
matrix M2m<span >=</span>interpolate<span >&#40;</span>Em,EM<span >&#41;</span><span >;</span>
&nbsp;
<span >// vecteur representant les numeros des points dans le grand maillage</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> nM<span >&#40;</span>M.<span >nv</span><span >&#41;</span><span >;</span>
nM<span >=</span><span >0</span><span >:</span><span >&#40;</span>M.<span >nv</span><span >-</span><span >1</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// vecteur du petit maillage contenant les numeros des memes points</span>
<span >// dans le grand maillage</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >&#93;</span> nm<span >&#40;</span>m.<span >nv</span><span >&#41;</span><span >;</span>
nm<span >=</span>M2m<span >*</span>nM<span >;</span>
&nbsp;
<span >// Affiche les numéros des points du petit maillage dans le grand maillage</span>
<span >cout</span><span >&lt;&lt;</span><span >&quot;numeros des points = &quot;</span><span >;</span>
<span >int</span> p<span >;</span>
<span >for</span><span >&#40;</span>p<span >=</span><span >0</span><span >;</span>p<span >&lt;</span>m.<span >nv</span><span >;</span>p<span >++</span><span >&#41;</span><span >cout</span><span >&lt;&lt;</span>nm<span >&#40;</span>p<span >&#41;</span><span >&lt;&lt;</span><span >&quot; &quot;</span><span >;</span>
<span >cout</span><span >&lt;&lt;</span>endl<span >;</span>
&nbsp;
<span >// affiche les points du petit maillage dans le grand maillage pour vérifier</span>
<span >// qu'ils constituent bien un triangle</span>
EM F<span >;</span>
<span >for</span><span >&#40;</span>p<span >=</span><span >0</span><span >;</span>p<span >&lt;</span>m.<span >nv</span><span >;</span>p<span >++</span><span >&#41;</span><span >&#123;</span>F<span >&#91;</span><span >&#93;</span><span >&#91;</span>nm<span >&#40;</span>p<span >&#41;</span><span >&#93;</span><span >=</span><span >1</span><span >;</span><span >&#125;</span>
plot<span >&#40;</span>F,cmm<span >=</span><span >&quot;verification&quot;</span><span >&#41;</span><span >;</span></pre>
</dd></dl>

La matrice élémentaire peut ensuite être obtenue en appliquant le problème global au petit maillage.

### Comment créer une échelle de couleurs monochrome rouge ou verte?

Voici l'exemple examples++-tutorial/plot.edp avec une échelle monochrome rouge. Pour une échelle verte, remplacer la première coordonnée de chaque couleur (hue) par 0.33.

<dl >
<dt>plot.edp</dt>
<dd><pre ><span >int</span> n<span >=</span><span >20</span>,nn<span >=</span>n<span >+</span><span >10</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> xx<span >&#40;</span>nn<span >&#41;</span>,yy<span >&#40;</span>nn<span >&#41;</span><span >;</span>
<span >//  \url{from:   http://en.wikipedia.org/wiki/HSV_color_space} </span>
<span >//The HSV (Hue, Saturation, Value) model, </span>
<span >//   defines a color space in terms of three constituent components:</span>
<span >//</span>
<span >//HSV color space as a color wheel</span>
<span >//Hue, the color type (such as red, blue, or yellow):</span>
<span >//   Ranges from 0-360 (but normalized to 0-100% h ere)</span>
<span >// Saturation, the &quot;vibrancy&quot; of the color: Ranges     from 0-100%</span>
<span >//    The lower the saturation of a color, the more &quot;grayness&quot; is present </span>
<span >//    and the more faded the color will appear.</span>
<span >// Value, the brightness of the color:</span>
<span >//   Ranges from 0-100%</span>
<span >// </span>
real<span >&#91;</span><span >int</span><span >&#93;</span> colorhsv<span >=</span><span >&#91;</span>  <span >// color hsv model</span>
  <span >1</span>, <span >1</span>, <span >0</span>,
  <span >1</span>, <span >1</span>, <span >0.25</span>,
  <span >1</span>, <span >1</span>, <span >0.5</span>,
  <span >1</span>, <span >1</span>, <span >0.75</span>,
  <span >1</span>, <span >1</span>, <span >1</span>
   <span >&#93;</span><span >;</span>
mesh Th<span >=</span>square<span >&#40;</span><span >5</span>,<span >5</span><span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P2<span >&#41;</span><span >;</span>
Vh uh<span >=</span>x<span >*</span>x<span >+</span>y<span >*</span>y,vh<span >=</span><span >-</span>y<span >^</span><span >2</span><span >+</span>x<span >^</span><span >2</span><span >;</span>
<span >assert</span><span >&#40;</span>n<span >+</span><span >1</span> <span >&lt;</span> nn<span >&#41;</span><span >;</span>
<span >//  compute a cut </span>
<span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;=</span>n<span >;</span>i<span >++</span><span >&#41;</span>
 <span >&#123;</span>
   xx<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >;</span>
   yy<span >&#91;</span>i<span >&#93;</span><span >=</span>uh<span >&#40;</span>real<span >&#40;</span>i<span >&#41;</span><span >/</span>n,real<span >&#40;</span>i<span >&#41;</span><span >/</span>n<span >&#41;</span><span >;</span> <span >// value of uh at point (i/10. , i/10.) </span>
 <span >&#125;</span>
&nbsp;
 plot<span >&#40;</span>Th,uh,<span >&#91;</span>uh,vh<span >&#93;</span>,value<span >=</span><span >true</span>,ps<span >=</span><span >&quot;three.eps&quot;</span>,wait<span >=</span><span >true</span><span >&#41;</span><span >;</span> <span >// plot mesh, isovalue, and vector</span>
 <span >//  zoom on box defined by the two corner points [0.1,0.2] and [0.5,0.6]</span>
 plot<span >&#40;</span>uh,<span >&#91;</span>uh,vh<span >&#93;</span>,bb<span >=</span><span >&#91;</span><span >&#91;</span><span >0.1</span>,<span >0.2</span><span >&#93;</span>,<span >&#91;</span><span >0.5</span>,<span >0.6</span><span >&#93;</span><span >&#93;</span>,wait<span >=</span><span >true</span>,grey<span >=</span><span >1</span>,fill<span >=</span><span >1</span>,value<span >=</span><span >1</span>,ps<span >=</span><span >&quot;threeg.eps&quot;</span><span >&#41;</span><span >;</span>  <span >// in grey with filling</span>
 plot<span >&#40;</span><span >&#91;</span>xx<span >&#40;</span><span >0</span><span >:</span>n<span >&#41;</span>,yy<span >&#40;</span><span >0</span><span >:</span>n<span >&#41;</span><span >&#93;</span>,<span >&#91;</span>xx<span >&#40;</span><span >0</span><span >:</span>n<span >:</span><span >5</span><span >&#41;</span>,yy<span >&#40;</span><span >0</span><span >:</span>n<span >:</span><span >5</span><span >&#41;</span><span >&#93;</span>,ps<span >=</span><span >&quot;likegnu.eps&quot;</span>,wait<span >=</span><span >true</span><span >&#41;</span><span >;</span> <span >//  like gnuplot plot a cut of uh</span>
&nbsp;
 real<span >&#91;</span><span >int</span><span >&#93;</span> viso<span >&#40;</span><span >31</span><span >&#41;</span><span >;</span>
&nbsp;
 <span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span>viso.<span >n</span><span >;</span>i<span >++</span><span >&#41;</span>
   viso<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >*</span><span >0.1</span><span >;</span>
&nbsp;
 plot<span >&#40;</span>uh,viso<span >=</span>viso<span >&#40;</span><span >0</span><span >:</span>viso.<span >n</span><span >-</span><span >1</span><span >&#41;</span>,value<span >=</span><span >1</span>,fill<span >=</span><span >1</span>,wait<span >=</span><span >1</span>,hsv<span >=</span>colorhsv,ps<span >=</span><span >&quot;threehsv.eps&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
&nbsp;</pre>
</dd></dl>

### Quelle est la signification du paramètre &quot;tgv&quot; pour la définition matricielle d'un problème?

*tgv* est la méthode utilisée par défaut par FreeFem++ pour implémenter les conditions de Dirichlet. *tgv* signifie “très grande valeur”
(10^30 par défaut). Elle est imposée sur le terme diagonal de la matrice (ce qui rend les autres termes de la même ligne négligeables) et au
second membre. Un avantage de cette méthode est de ne modifier qu'un seul terme de la matrice. Un désavantage est de créer une très grande
valeur propre dans le système à résoudre, ce qui peut mettre en difficulté la méthode de résolution choisie.

En cas de difficulté, une valeur négative pour le paramètre *tgv* force FreeFem++ à utiliser une autre méthode: mettre 1 sur la diagonale et
annuler tous les autres termes de la ligne de la matrice.

### Comment créer rapidement un maillage 3D en forme de sphère?
<dl >
<dt>sphere.edp</dt>
<dd><pre >load <span >&quot;msh3&quot;</span>
&nbsp;
border cc<span >&#40;</span>t<span >=</span><span >0</span>,<span >2</span><span >*</span>pi<span >&#41;</span><span >&#123;</span>x<span >=</span><span >cos</span><span >&#40;</span>t<span >&#41;</span><span >;</span>y<span >=</span><span >sin</span><span >&#40;</span>t<span >&#41;</span><span >;</span>label<span >=</span><span >1</span><span >;</span><span >&#125;</span>
mesh Th2<span >=</span> buildmesh<span >&#40;</span>cc<span >&#40;</span><span >500</span><span >&#41;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// eps is there to avoid square roots of negative values</span>
<span >// and thin triangles close to the equator</span>
real eps<span >=</span><span >1e-2</span><span >;</span>
&nbsp;
func zmin<span >=</span><span >-</span><span >sqrt</span><span >&#40;</span><span >1</span><span >+</span>eps<span >-</span>x<span >*</span>x<span >-</span>y<span >*</span>y<span >&#41;</span><span >;</span>
func zmax<span >=</span><span >sqrt</span><span >&#40;</span><span >1</span><span >+</span>eps<span >-</span>x<span >*</span>x<span >-</span>y<span >*</span>y<span >&#41;</span><span >;</span>
&nbsp;
<span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> rup<span >=</span><span >&#91;</span><span >0</span>,<span >2</span><span >&#93;</span>,rdown<span >=</span><span >&#91;</span><span >0</span>,<span >1</span><span >&#93;</span>,rmid<span >=</span><span >&#91;</span><span >1</span>,<span >3</span>,<span >2</span>,<span >3</span>,<span >3</span>,<span >3</span>,<span >4</span>,<span >3</span><span >&#93;</span><span >;</span>
&nbsp;
mesh3 Th<span >=</span>buildlayers<span >&#40;</span>Th2,<span >20</span>,
  zbound<span >=</span><span >&#91;</span>zmin,zmax<span >&#93;</span>,
  labelmid<span >=</span>rmid, 
  reffaceup <span >=</span> rup,
  reffacelow <span >=</span> rdown<span >&#41;</span><span >;</span>
&nbsp;
plot<span >&#40;</span>Th<span >&#41;</span><span >;</span></pre>
</dd></dl>

ce qui donne :

ffquasisphere.png <!-- ALHTODO find in dokuwiki backups -->

### Comment convertir une image SVG en maillage FreeFem++?

Voici un script [perl](#perl) qui sait traduire les SVG qui contiennent des courbes de Bézier cubiques et des lignes droites :

<dl >
<dt>svg2edp</dt>
<dd><pre ><span >#!/usr/bin/perl</span>
<span ># ======================================================================</span>
<span ># Written by Antoine Le Hyaric</span>
<span ># http://www.ljll.math.upmc.fr/lehyaric</span>
<span ># ======================================================================</span>
<span ># headeralh mine perl start=20/02/2012</span>
&nbsp;
<span ># Converts a 2D SVG picture (eg obtained with inkscape &quot;Path/Trace Bitmap...&quot;) into a list of FreeFem++ borders and</span>
<span ># meshes. Examples use: &quot;svg2edp &lt; file.svg  &gt; file.edp 2&gt; file.gnuplot&quot;</span>
&nbsp;
<span >use</span> strict<span >;</span>
&nbsp;
<span ># final list of all borders</span>
<span >my</span> <span >@borders</span><span >;</span>
&nbsp;
<span ># numbering borders</span>
<span >my</span> <span >$numb</span><span >=</span><span >0</span><span >;</span>
&nbsp;
<span >sub</span> straightborder<span >&#123;</span>
  <span >my</span><span >&#40;</span><span >$x0</span><span >,</span><span >$y0</span><span >,</span><span >$x1</span><span >,</span><span >$y1</span><span >&#41;</span><span >=</span><span >@_</span><span >;</span>
&nbsp;
  [<span >die</span>](http://perldoc.perl.org/functions/#diel) <span >if</span> <span >&#40;</span>[<span >abs</span>](http://perldoc.perl.org/functions/#absl)<span >&#40;</span><span >$x1</span><span >-</span><span >$x0</span><span >&#41;</span><span >+</span>[<span >abs</span>](http://perldoc.perl.org/functions/#absl)<span >&#40;</span><span >$y1</span><span >-</span><span >$y0</span><span >&#41;</span><span >&#41;</span><span >&lt;</span>1e<span >-</span>6<span >;</span>
&nbsp;
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;border b$numb(t=0,1){<span >\n</span>&quot;</span><span >;</span>
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;<span >\t</span>x=$x0*t+$x1*(1-t);<span >\n</span>&quot;</span><span >;</span>
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;<span >\t</span>y=$y0*t+$y1*(1-t);<span >\n</span>&quot;</span><span >;</span>
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;}<span >\n</span>&quot;</span><span >;</span>
  [<span >push</span>](http://perldoc.perl.org/functions/#pushl) <span >@borders</span><span >,</span><span >&quot;b$numb(-2)&quot;</span><span >;</span>
  <span >$numb</span><span >++;</span>
&nbsp;
  <span ># stderr contains the same data for debugging via gnuplot</span>
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >STDERR</span> <span >&quot;$x0 $y0<span >\n</span>&quot;</span><span >;</span>
  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >STDERR</span> <span >&quot;$x1 $y1<span >\n</span>&quot;</span><span >;</span>
<span >&#125;</span>
&nbsp;
<span >sub</span> bezierinterp<span >&#123;</span>
  <span >my</span><span >&#40;</span><span >$p0</span><span >,</span><span >$q0</span><span >,</span><span >$q1</span><span >,</span><span >$p1</span><span >,</span><span >$t</span><span >&#41;</span><span >=</span><span >@_</span><span >;</span>
  [<span >return</span>](http://perldoc.perl.org/functions/#returnl) <span >$p0</span><span >*</span><span >&#40;</span><span >1</span><span >-</span><span >$t</span><span >&#41;</span><span >**</span><span >3</span><span >+</span><span >$q0</span><span >*</span><span >3</span><span >*</span><span >&#40;</span><span >1</span><span >-</span><span >$t</span><span >&#41;</span><span >**</span><span >2</span><span >*$t</span><span >+</span><span >$q1</span><span >*</span><span >3</span><span >*</span><span >&#40;</span><span >1</span><span >-</span><span >$t</span><span >&#41;</span><span >*$t</span><span >**</span><span >2</span><span >+</span><span >$p1</span><span >*$t</span><span >**</span><span >3</span><span >;</span>
<span >&#125;</span>
&nbsp;
<span >sub</span> bezierborder<span >&#123;</span>
  <span >my</span><span >&#40;</span><span >$p1x</span><span >,</span><span >$p1y</span><span >,</span><span >$q1x</span><span >,</span><span >$q1y</span><span >,</span><span >$q2x</span><span >,</span><span >$q2y</span><span >,</span><span >$p2x</span><span >,</span><span >$p2y</span><span >&#41;</span><span >=</span><span >@_</span><span >;</span>
  <span >my</span> <span >$xprev</span><span >=</span><span >$p1x</span><span >;</span>
  <span >my</span> <span >$yprev</span><span >=</span><span >$p1y</span><span >;</span>
&nbsp;
  <span >for</span><span >&#40;</span><span >my</span> <span >$t</span><span >=</span><span >0.1</span><span >;</span><span >$t</span><span >&lt;=</span><span >1</span><span >;</span><span >$t</span><span >+=</span><span >0.1</span><span >&#41;</span><span >&#123;</span>
    <span >my</span> <span >$xnext</span><span >=</span>bezierinterp<span >&#40;</span><span >$p1x</span><span >,</span><span >$q1x</span><span >,</span><span >$q2x</span><span >,</span><span >$p2x</span><span >,</span><span >$t</span><span >&#41;</span><span >;</span>
    <span >my</span> <span >$ynext</span><span >=</span>bezierinterp<span >&#40;</span><span >$p1y</span><span >,</span><span >$q1y</span><span >,</span><span >$q2y</span><span >,</span><span >$p2y</span><span >,</span><span >$t</span><span >&#41;</span><span >;</span>
&nbsp;
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;border b$numb(t=0,1){<span >\n</span>&quot;</span><span >;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;<span >\t</span>x=$xprev*t+$xnext*(1-t);<span >\n</span>&quot;</span><span >;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;<span >\t</span>y=$yprev*t+$ynext*(1-t);<span >\n</span>&quot;</span><span >;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;<span >\t</span>label=1;<span >\n</span>&quot;</span><span >;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;}<span >\n</span>&quot;</span><span >;</span>
    [<span >push</span>](http://perldoc.perl.org/functions/#pushl) <span >@borders</span><span >,</span><span >&quot;b$numb(-2)&quot;</span><span >;</span>
    <span >$numb</span><span >++;</span>
&nbsp;
    <span ># stderr contains the same data for debugging via gnuplot</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >STDERR</span> <span >&quot;$xprev $yprev<span >\n</span>&quot;</span><span >;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >STDERR</span> <span >&quot;$xnext $ynext<span >\n</span>&quot;</span><span >;</span>
&nbsp;
    <span >$xprev</span><span >=</span><span >$xnext</span><span >;</span>
    <span >$yprev</span><span >=</span><span >$ynext</span><span >;</span>
  <span >&#125;</span>
<span >&#125;</span>
&nbsp;
<span ># numbering meshes</span>
<span >my</span> <span >$numm</span><span >=</span><span >0</span><span >;</span>
&nbsp;
<span ># read input file</span>
<span >while</span><span >&#40;</span><span >&lt;STDIN&gt;</span><span >&#41;</span><span >&#123;</span>
  <span >next</span> <span >unless</span> <span >/ d=&quot;(.*)&quot;/</span><span >;</span>
  <span >my</span> <span >$path</span><span >=</span><span >$1</span><span >;</span>
&nbsp;
  <span ># scan path</span>
  <span >my</span> <span >$num</span><span >=</span><span >'([-.0-9]+)'</span><span >;</span>
&nbsp;
  <span ># current point in absolute coordinates</span>
  <span >my</span> <span >$curx</span><span >=</span><span >0</span><span >;</span>
  <span >my</span> <span >$cury</span><span >=</span><span >0</span><span >;</span>
&nbsp;
  <span ># first point (to close a curve) in absolute coordinates</span>
  <span >my</span> <span >$firstx</span><span >;</span>
  <span >my</span> <span >$firsty</span><span >;</span>
  <span >my</span> <span >$firstok</span><span >=</span><span >0</span><span >;</span>
&nbsp;
  <span ># list of all SVG commands [[http://www.w3.org/TR/SVG11/#pathsl#PathDataMovetoCommands]]</span>
  <span >my</span> <span >$state</span><span >=</span><span >''</span><span >;</span>
  <span >my</span> <span >$abs</span><span >=</span><span >0</span><span >;</span>
  <span >my</span> <span >@args</span><span >;</span>
  <span >while</span><span >&#40;</span><span >$path</span><span >=~</span>[<span >m</span>](http://perldoc.perl.org/functions/#ml)<span >/</span> <span >*</span><span >&#40;</span>[<span >m</span>](http://perldoc.perl.org/functions/#ml)<span >|</span>c<span >|</span>l<span >|</span>z<span >|</span><span >$num</span><span >,</span><span >$num</span><span >&#41;</span><span >/</span>gi<span >&#41;</span><span >&#123;</span>
    <span >my</span> <span >$Command</span><span >=</span><span >$1</span><span >;</span>
    <span >my</span> <span >$command</span><span >=</span>[<span >lc</span>](http://perldoc.perl.org/functions/#lcl)<span >&#40;</span><span >$Command</span><span >&#41;</span><span >;</span>
    <span >my</span> <span >$x</span><span >=</span><span >$2</span><span >;</span>
    <span >my</span> <span >$y</span><span >=</span><span >$3</span><span >;</span>
    <span >if</span><span >&#40;</span><span >$command</span> <span >eq</span> <span >'m'</span> <span >||</span> <span >$command</span> <span >eq</span> <span >'c'</span> <span >||</span> <span >$command</span> <span >eq</span> <span >'l'</span><span >&#41;</span><span >&#123;</span>
      <span >$state</span><span >=</span>[<span >lc</span>](http://perldoc.perl.org/functions/#lcl)<span >&#40;</span><span >$command</span><span >&#41;</span><span >;</span>
&nbsp;
      <span ># capital letters represent absolute coordinates</span>
      <span >$abs</span><span >=</span><span >0</span><span >;</span>
      <span >$abs</span><span >=</span><span >1</span> <span >if</span> [<span >ord</span>](http://perldoc.perl.org/functions/#ordl)<span >&#40;</span><span >$Command</span><span >&#41;</span><span >&lt;</span><span >97</span><span >;</span>
&nbsp;
      <span >@args</span><span >=</span><span >&#40;</span><span >&#41;</span><span >;</span>
    <span >&#125;</span>
&nbsp;
    <span ># SVG command for closing the curve</span>
    <span >elsif</span><span >&#40;</span><span >$command</span> <span >eq</span> <span >'z'</span><span >&#41;</span><span >&#123;</span>
      [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;// closing the curve<span >\n</span>&quot;</span><span >;</span>
      <span >###straightborder($curx,$cury,$firstx,$firsty);</span>
      <span >$curx</span><span >=</span><span >$firstx</span><span >;</span>
      <span >$cury</span><span >=</span><span >$firsty</span><span >;</span>
    <span >&#125;</span>
&nbsp;
    <span ># SVG commands followed by coordinates</span>
    <span >else</span><span >&#123;</span>
&nbsp;
      <span ># initial point</span>
      <span >if</span><span >&#40;</span><span >$state</span> <span >eq</span> <span >'m'</span><span >&#41;</span><span >&#123;</span>
	<span >$curx</span><span >=</span>abscoord<span >&#40;</span><span >$curx</span><span >,</span><span >$x</span><span >,</span><span >$abs</span><span >&#41;</span><span >;</span>
	<span >$cury</span><span >=</span>abscoord<span >&#40;</span><span >$cury</span><span >,</span><span >$y</span><span >,</span><span >$abs</span><span >&#41;</span><span >;</span>
	[<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;// moving to [$curx,$cury]<span >\n</span>&quot;</span><span >;</span>
	<span >if</span><span >&#40;</span><span >!</span><span >$firstok</span><span >&#41;</span><span >&#123;</span>
	  <span >$firstx</span><span >=</span><span >$curx</span><span >;</span>
	  <span >$firsty</span><span >=</span><span >$cury</span><span >;</span>
	  <span >$firstok</span><span >=</span><span >1</span><span >;</span>
	<span >&#125;</span>
      <span >&#125;</span>
&nbsp;
      <span ># line</span>
      <span >elsif</span><span >&#40;</span><span >$state</span> <span >eq</span> <span >'l'</span><span >&#41;</span><span >&#123;</span>
	[<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;// line<span >\n</span>&quot;</span><span >;</span>
	<span >my</span> <span >$tox</span><span >=</span>abscoord<span >&#40;</span><span >$curx</span><span >,</span><span >$x</span><span >,</span><span >$abs</span><span >&#41;</span><span >;</span>
	<span >my</span> <span >$toy</span><span >=</span>abscoord<span >&#40;</span><span >$cury</span><span >,</span><span >$y</span><span >,</span><span >$abs</span><span >&#41;</span><span >;</span>
	straightborder<span >&#40;</span><span >$curx</span><span >,</span><span >$cury</span><span >,</span><span >$tox</span><span >,</span><span >$toy</span><span >&#41;</span><span >;</span>
	<span >$curx</span><span >=</span><span >$tox</span><span >;</span>
	<span >$cury</span><span >=</span><span >$toy</span><span >;</span>
      <span >&#125;</span>
&nbsp;
      <span ># bezier curve</span>
      <span >elsif</span><span >&#40;</span><span >$state</span> <span >eq</span> <span >'c'</span><span >&#41;</span><span >&#123;</span>
&nbsp;
	[<span >push</span>](http://perldoc.perl.org/functions/#pushl) <span >@args</span><span >,</span>abscoord<span >&#40;</span><span >$curx</span><span >,</span><span >$x</span><span >,</span><span >$abs</span><span >&#41;</span><span >,</span>abscoord<span >&#40;</span><span >$cury</span><span >,</span><span >$y</span><span >,</span><span >$abs</span><span >&#41;</span><span >;</span>
&nbsp;
	<span ># draw one bezier segment when is fully defined (ie with 2 points + 2 control points)</span>
	<span >if</span><span >&#40;</span><span >$#args</span><span >==</span><span >5</span><span >&#41;</span><span >&#123;</span>
	  [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;// bezier curve<span >\n</span>&quot;</span><span >;</span>
&nbsp;
	  <span >my</span> <span >$tox</span><span >=</span><span >$args</span><span >&#91;</span><span >4</span><span >&#93;</span><span >;</span>
	  <span >my</span> <span >$toy</span><span >=</span><span >$args</span><span >&#91;</span><span >5</span><span >&#93;</span><span >;</span>
	  bezierborder<span >&#40;</span><span >$curx</span><span >,</span><span >$cury</span><span >,</span><span >$args</span><span >&#91;</span><span >0</span><span >&#93;</span><span >,</span><span >$args</span><span >&#91;</span><span >1</span><span >&#93;</span><span >,</span><span >$args</span><span >&#91;</span><span >2</span><span >&#93;</span><span >,</span><span >$args</span><span >&#91;</span><span >3</span><span >&#93;</span><span >,</span><span >$tox</span><span >,</span><span >$toy</span><span >&#41;</span><span >;</span>
&nbsp;
	  <span ># the next bezier point may come without an explicit 'c'</span>
	  <span >@args</span><span >=</span><span >&#40;</span><span >&#41;</span><span >;</span>
	  <span >$curx</span><span >=</span><span >$tox</span><span >;</span>
	  <span >$cury</span><span >=</span><span >$toy</span><span >;</span>
	<span >&#125;</span>
      <span >&#125;</span>
    <span >&#125;</span>
  <span >&#125;</span>
&nbsp;
  <span ># create corresponding mesh</span>
  <span >if</span><span >&#40;</span><span >$#borders</span><span >&gt;=</span><span >0</span><span >&#41;</span><span >&#123;</span>
    [<span >print</span>](http://perldoc.perl.org/functions/#printl) <span >&quot;mesh Th$numm=buildmesh(&quot;</span><span >.</span>[<span >join</span>](http://perldoc.perl.org/functions/#joinl)<span >&#40;</span><span >&quot;+&quot;</span><span >,</span><span >@borders</span><span >&#41;</span><span >.</span><span >&quot;);<span >\n</span>&quot;</span><span >;</span>
    <span >$numm</span><span >++;</span>
  <span >&#125;</span>
<span >&#125;</span>
&nbsp;
<span ># choose between relative and absolute coordinates</span>
<span >sub</span> abscoord<span >&#123;</span>
  <span >my</span><span >&#40;</span><span >$x0</span><span >,</span><span >$x</span><span >,</span><span >$abs</span><span >&#41;</span><span >=</span><span >@_</span><span >;</span>
  [<span >return</span>](http://perldoc.perl.org/functions/#returnl) <span >$x</span> <span >if</span> <span >$abs</span><span >;</span>
  [<span >return</span>](http://perldoc.perl.org/functions/#returnl) <span >$x</span><span >+</span><span >$x0</span><span >;</span>
<span >&#125;</span>
&nbsp;
<span ># Local Variables:</span>
<span ># mode:cperl</span>
<span ># ispell-local-dictionary:&quot;british&quot;</span>
<span ># coding:utf-8</span>
<span ># End:</span></pre>
</dd></dl>

### Comment passer du 2D au 3D dans FreeFem++?

Les points importants pour convertir un script .edp du 2D au 3D:

<ul>
<li > ajouter <strong>load “msh3”</strong> (et <strong>load “tetgen”</strong> si nécessaire) au début du script
</li>
<li > utiliser le mot-clé <strong>mesh3</strong> au lieu de <strong>mesh</strong> pour définir les maillages 3D
</li>
<li > créer un maillage 3D grâce à (au choix):
<ul>
<li > <strong>buildlayers()</strong>
</li>
<li > <strong>tetg()</strong>
</li>
<li > en incluant les géométries définies dans MeshSurface.idp (sphère et boite carrée)
</li>
<li > en chargeant un maillage externe au format .mesh construit avec [Gmsh](#gmsh) par exemple
</li>
</ul>
</li>
<li > si nécessaire, changer la méthode de résolution par défaut de FreeFem++ ([Umfpack](#umfpack)) pour limiter la consommation de mémoire vive (essayer par exemple <strong>CG</strong> ou <strong>GMRES</strong>).
</li>
</ul>

### Comment extraire les matrices contruites par FreeFem++?

Le mot-clé <strong>problem</strong> ne permet pas de manipuler les matrices. Il faut utiliser le mot-clé <strong>varf</strong> avec les précautions suivantes:

<ul>
<li > un “problem” doit être traduit en deux matrices: une matrice carrée A et un second membre B qui donnent l'équation Ax=B
</li>
<li > le second membre B calculé par varf est <em >du signe opposé* à celui calculé par problem. Ce changement de signe est contenu <em >implicitement* dans l'écriture des conditions de Dirichlet “on(…)” mais pas dans les termes intégraux dépendant de l'edp traitée.
</li>
</ul>

Voici un exemple:

<dl >
<dt>problem2varf.edp</dt>
<dd><pre >mesh Th<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span><span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
Vh uh,vh<span >;</span>
func f<span >=</span><span >1</span><span >;</span>
func g<span >=</span><span >1</span><span >;</span>
&nbsp;
<span >// Résolution d'une EDP avec le mot-clé problem</span>
problem laplace<span >&#40;</span>uh,vh<span >&#41;</span><span >=</span>int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>uh<span >&#41;</span><span >*</span>dx<span >&#40;</span>vh<span >&#41;</span><span >+</span>dy<span >&#40;</span>uh<span >&#41;</span><span >*</span>dy<span >&#40;</span>vh<span >&#41;</span><span >&#41;</span><span >-</span>int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>f<span >*</span>vh<span >&#41;</span><span >+</span>on<span >&#40;</span><span >1</span>,<span >2</span>,<span >3</span>,<span >4</span>,uh<span >=</span>g<span >&#41;</span><span >;</span>
laplace<span >;</span>
plot<span >&#40;</span>uh<span >&#41;</span><span >;</span>
&nbsp;
<span >// Résolution de la même EDP sous forme matricielle</span>
varf laplaceA<span >&#40;</span>uh,vh<span >&#41;</span><span >=</span>int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>uh<span >&#41;</span><span >*</span>dx<span >&#40;</span>vh<span >&#41;</span><span >+</span>dy<span >&#40;</span>uh<span >&#41;</span><span >*</span>dy<span >&#40;</span>vh<span >&#41;</span><span >&#41;</span><span >;</span>
matrix A<span >=</span>laplaceA<span >&#40;</span>Vh,Vh<span >&#41;</span><span >;</span>
&nbsp;
varf laplaceB<span >=</span>int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>f<span >*</span>vh<span >&#41;</span><span >+</span>on<span >&#40;</span><span >1</span>,<span >2</span>,<span >3</span>,<span >4</span>,uh<span >=</span>g<span >&#41;</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> B<span >=</span>laplaceB<span >&#40;</span><span >0</span>,Vh<span >&#41;</span><span >;</span>
&nbsp;
uh<span >&#91;</span><span >&#93;</span><span >=</span>A<span >^</span><span >-</span><span >1</span><span >*</span>B<span >;</span>
plot<span >&#40;</span>uh<span >&#41;</span><span >;</span></pre>
</dd></dl>

### Comment coupler plusieurs problèmes en construisant une matrice par blocs?
<ul>
<li > Il faut extraire les matrices des deux problèmes A11, A22, B1, B2. Puis construire les blocs rectangulaires A12 et A21
</li>
</ul>
<pre >matrix A12<span >=</span>probleme1<span >&#40;</span>Vh2,Vh1<span >&#41;</span><span >;</span>
matrix A21<span >=</span>probleme1<span >&#40;</span>Vh1,Vh2<span >&#41;</span><span >;</span></pre>
<ul>
<li > Puis construire la matrice par blocs
</li>
</ul>
<pre >matrix A<span >=</span><span >&#91;</span><span >&#91;</span>A11,A12<span >&#93;</span>,<span >&#91;</span>A21,A22<span >&#93;</span><span >&#93;</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> B<span >=</span><span >&#91;</span>B1,B2<span >&#93;</span><span >;</span></pre>
<ul>
<li > Puis calculer les deux solutions couplées
</li>
</ul>
<pre >Vh1 u1<span >;</span>
Vh2 u2<span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> T<span >=</span>A<span >^</span><span >-</span><span >1</span><span >*</span>B<span >;</span>
<span >&#91;</span>u1<span >&#91;</span><span >&#93;</span>,u2<span >&#91;</span><span >&#93;</span><span >&#93;</span><span >=</span>T<span >;</span></pre>

### Comment afficher un domaine de calcul très étroit?

Quand une dimension du domaine de calcul est très petite par rapport aux autres, il est très difficile de voir les valeurs affichées sur le domaine qui ressemble plus à une ligne qu'à une surface. Voici comment augmenter la petite dimension du domaine juste pour afficher les valeurs numériques de manière visible.

<pre ><span >// very thin domain (x range is very small with respect to y)</span>
mesh Th<span >=</span>square<span >&#40;</span><span >1</span>,<span >100</span>,<span >&#91;</span><span >.01</span><span >*</span>x,y<span >&#93;</span><span >&#41;</span><span >;</span> 
plot<span >&#40;</span>Th<span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
&nbsp;
<span >// example of value on this very this domain</span>
Vh uh<span >=</span><span >1e4</span><span >*</span>x<span >*</span>x<span >+</span>y<span >*</span>y<span >;</span>
plot<span >&#40;</span>uh<span >&#41;</span><span >;</span>
&nbsp;
<span >// wider mesh</span>
mesh Thzoom<span >=</span>square<span >&#40;</span><span >100</span>,<span >100</span>,<span >&#91;</span>x,y<span >&#93;</span><span >&#41;</span><span >;</span> 
plot<span >&#40;</span>Thzoom<span >&#41;</span><span >;</span>
fespace Vhzoom<span >&#40;</span>Thzoom,P1<span >&#41;</span><span >;</span>
&nbsp;
<span >// values from the thin domain displayed on the wider domain</span>
Vhzoom uhzoom<span >=</span>uh<span >&#40;</span>x<span >/</span><span >100</span>,y<span >&#41;</span><span >;</span>
plot<span >&#40;</span>uhzoom<span >&#41;</span><span >;</span></pre>

### Dessiner une frontière dans un maillage

Une solution pour dessiner une frontière à l'intérieur d'un maillage FreeFem++ est de créer un espace blanc (vide):

<pre ><span >// Maillage complet</span>
mesh Th<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span>,<span >&#91;</span><span >2</span><span >*</span>x,y<span >&#93;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// Maillages séparés par un vide représentant une frontière dans le domaine</span>
mesh Th1<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span>,<span >&#91;</span>x<span >*</span><span >0.99</span>,y<span >&#93;</span><span >&#41;</span><span >;</span>
mesh Th2<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span>,<span >&#91;</span>x<span >*</span><span >.9</span><span >+</span><span >1</span>,y<span >&#93;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// Exemple de problème résolu sur Th et visualisé avec une frontière</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
Vh uh,vh<span >;</span>
func f<span >=</span><span >1</span><span >;</span>
func g<span >=</span><span >0</span><span >;</span>
problem laplace<span >&#40;</span>uh,vh,solver<span >=</span>GMRES,tgv<span >=</span><span >1e5</span><span >&#41;</span> <span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span> dx<span >&#40;</span>uh<span >&#41;</span><span >*</span>dx<span >&#40;</span>vh<span >&#41;</span> <span >+</span> dy<span >&#40;</span>uh<span >&#41;</span><span >*</span>dy<span >&#40;</span>vh<span >&#41;</span> <span >&#41;</span>
  <span >-</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span> f<span >*</span>vh <span >&#41;</span>
  <span >+</span> on<span >&#40;</span><span >2</span>,uh<span >=</span>g<span >&#41;</span> <span >;</span>
&nbsp;
laplace<span >;</span>
&nbsp;
<span >// Interpolation de la solution continue sur le maillage avec frontière</span>
fespace Vh1<span >&#40;</span>Th1,P1<span >&#41;</span><span >;</span>
fespace Vh2<span >&#40;</span>Th2,P1<span >&#41;</span><span >;</span>
Vh1 uh1<span >=</span>uh<span >;</span>
Vh2 uh2<span >=</span>uh<span >;</span>
&nbsp;
<span >// Dessin avec frontière visible</span>
plot<span >&#40;</span>uh1,uh2<span >&#41;</span><span >;</span></pre>

### Convertir un maillage vers FreeFem++

Cet exemple peut facilement être transformé pour lire tout autre format de maillage 2D enregistré dans un fichier texte :

<pre ><span >// mesh data</span>
<span >int</span> nodes<span >;</span>
<span >int</span> equations<span >;</span>
<span >int</span> elements<span >;</span>
<span >int</span> nodesperelem<span >;</span>
<span >int</span> spacedim<span >;</span>
<span >int</span> ni<span >;</span>
<span >int</span> nj<span >;</span>
real<span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> coordinates<span >&#40;</span><span >3</span>,<span >1</span><span >&#41;</span><span >;</span>
real<span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> geometry<span >&#40;</span><span >3</span>,<span >1</span><span >&#41;</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> subdomain<span >&#40;</span><span >1</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// Load mesh</span>
<span >&#123;</span>
  ifstream i<span >&#40;</span><span >&quot;mesh.data&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
  <span >// skip some textual data (7 words)</span>
  string l<span >;</span>
  i<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >;</span>
&nbsp;
  <span >// read mesh size</span>
  i<span >&gt;&gt;</span>nodes<span >;</span>
  i<span >&gt;&gt;</span>elements<span >;</span>
  i<span >&gt;&gt;</span>nodesperelem<span >;</span>
  i<span >&gt;&gt;</span>spacedim<span >;</span>
  i<span >&gt;&gt;</span>ni<span >;</span>
  i<span >&gt;&gt;</span>nj<span >;</span>
&nbsp;
  coordinates.<span >resize</span><span >&#40;</span><span >3</span>,nodes<span >&#41;</span><span >;</span>
  geometry.<span >resize</span><span >&#40;</span><span >3</span>,elements<span >&#41;</span><span >;</span>
  subdomain.<span >resize</span><span >&#40;</span>elements<span >&#41;</span><span >;</span>
&nbsp;
  <span >// skip textual title (1 word)</span>
  i<span >&gt;&gt;</span>l<span >;</span>
&nbsp;
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>nodes<span >;</span>n<span >++</span><span >&#41;</span><span >&#123;</span>
    <span >for</span><span >&#40;</span><span >int</span> d<span >=</span><span >0</span><span >;</span>d<span >&lt;</span><span >3</span><span >;</span>d<span >++</span><span >&#41;</span><span >&#123;</span>
      i<span >&gt;&gt;</span>coordinates<span >&#40;</span>d,n<span >&#41;</span><span >;</span>
    <span >&#125;</span>
  <span >&#125;</span>
&nbsp;
  <span >// skip textual title (1 word)</span>
  i<span >&gt;&gt;</span>l<span >;</span>
&nbsp;
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>elements<span >;</span>n<span >++</span><span >&#41;</span><span >&#123;</span>
    <span >for</span><span >&#40;</span><span >int</span> d<span >=</span><span >0</span><span >;</span>d<span >&lt;</span><span >3</span><span >;</span>d<span >++</span><span >&#41;</span><span >&#123;</span>
      i<span >&gt;&gt;</span>geometry<span >&#40;</span>d,n<span >&#41;</span><span >;</span>
      geometry<span >&#40;</span>d,n<span >&#41;</span><span >=</span>geometry<span >&#40;</span>d,n<span >&#41;</span><span >-</span><span >1</span><span >;</span>
    <span >&#125;</span>
  <span >&#125;</span>
&nbsp;
  <span >// skip textual title (4 words)</span>
  i<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >&gt;&gt;</span>l<span >;</span>
&nbsp;
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>elements<span >;</span>n<span >++</span><span >&#41;</span>i<span >&gt;&gt;</span>subdomain<span >&#40;</span>n<span >&#41;</span><span >;</span>
<span >&#125;</span>
&nbsp;
<span >// save mesh in FreeFem++ 2D .msh format</span>
<span >&#123;</span>
  ofstream o<span >&#40;</span><span >&quot;mesh.msh&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
  <span >// numbers of points, elements, edges</span>
  o<span >&lt;&lt;</span>nodes<span >&lt;&lt;</span><span >&quot; &quot;</span><span >&lt;&lt;</span>elements<span >&lt;&lt;</span><span >&quot; &quot;</span><span >&lt;&lt;</span><span >0</span><span >&lt;&lt;</span>endl<span >;</span>
&nbsp;
  <span >// points</span>
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>nodes<span >;</span>n<span >++</span><span >&#41;</span><span >&#123;</span>
&nbsp;
    <span >// 2D coordinates</span>
    <span >for</span><span >&#40;</span><span >int</span> c<span >=</span><span >0</span><span >;</span>c<span >&lt;</span><span >2</span><span >;</span>c<span >++</span><span >&#41;</span><span >&#123;</span>
      o<span >&lt;&lt;</span>coordinates<span >&#40;</span>c,n<span >&#41;</span><span >&lt;&lt;</span><span >&quot; &quot;</span><span >;</span>
    <span >&#125;</span>
&nbsp;
    <span >// label</span>
    o<span >&lt;&lt;</span><span >0</span><span >&lt;&lt;</span>endl<span >;</span>
  <span >&#125;</span>
&nbsp;
  <span >// elements</span>
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>elements<span >;</span>n<span >++</span><span >&#41;</span><span >&#123;</span>
&nbsp;
    <span >// connectivity</span>
    <span >for</span><span >&#40;</span><span >int</span> c<span >=</span><span >0</span><span >;</span>c<span >&lt;</span><span >3</span><span >;</span>c<span >++</span><span >&#41;</span><span >&#123;</span>
      o<span >&lt;&lt;</span>geometry<span >&#40;</span>c,n<span >&#41;</span><span >+</span><span >1</span><span >&lt;&lt;</span><span >&quot; &quot;</span><span >;</span>
    <span >&#125;</span>
&nbsp;
    <span >// label</span>
    o<span >&lt;&lt;</span><span >0</span><span >&lt;&lt;</span>endl<span >;</span>
  <span >&#125;</span>
<span >&#125;</span>
&nbsp;
<span >// reload the mesh in the FreeFem++ format</span>
mesh Th<span >=</span>readmesh<span >&#40;</span><span >&quot;mesh.msh&quot;</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// load some values</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
Vh u,v<span >;</span>
<span >&#123;</span>
  ifstream i<span >&#40;</span><span >&quot;solution.data&quot;</span><span >&#41;</span><span >;</span>
  <span >int</span> rank<span >;</span>
  <span >for</span><span >&#40;</span><span >int</span> n<span >=</span><span >0</span><span >;</span>n<span >&lt;</span>nodes<span >;</span>n<span >++</span><span >&#41;</span><span >&#123;</span>
&nbsp;
      <span >// u</span>
      i<span >&gt;&gt;</span>u<span >&#91;</span><span >&#93;</span><span >&#40;</span>n<span >&#41;</span><span >;</span>
&nbsp;
      <span >// v</span>
      i<span >&gt;&gt;</span>v<span >&#91;</span><span >&#93;</span><span >&#40;</span>n<span >&#41;</span><span >;</span>
    <span >&#125;</span>
  <span >&#125;</span>
<span >&#125;</span>
&nbsp;
<span >// display values in FreeFem++</span>
plot<span >&#40;</span>Th,<span >&#91;</span>u,v<span >&#93;</span>,value<span >=</span><span >1</span>,cmm<span >=</span><span >&quot;u,v&quot;</span><span >&#41;</span><span >;</span></pre>

### Un exemple d'écoulement de Stokes en FreeFem++

L'exemple suivant se trouve dans le dossier examples++-chapt3/stokes.edp de FreeFem++ :

<pre ><span >//file Stokes.edp</span>
<span >int</span> n<span >=</span><span >3</span><span >;</span>
mesh Th<span >=</span>square<span >&#40;</span><span >10</span><span >*</span>n,<span >10</span><span >*</span>n<span >&#41;</span><span >;</span>
fespace Uh<span >&#40;</span>Th,P1b<span >&#41;</span><span >;</span> Uh u,v,uu,vv<span >;</span>
fespace Ph<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>  Ph p,pp<span >;</span>
&nbsp;
solve stokes<span >&#40;</span><span >&#91;</span>u,v,p<span >&#93;</span>,<span >&#91;</span>uu,vv,pp<span >&#93;</span><span >&#41;</span> <span >=</span>
    int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>u<span >&#41;</span><span >*</span>dx<span >&#40;</span>uu<span >&#41;</span><span >+</span>dy<span >&#40;</span>u<span >&#41;</span><span >*</span>dy<span >&#40;</span>uu<span >&#41;</span> <span >+</span> dx<span >&#40;</span>v<span >&#41;</span><span >*</span>dx<span >&#40;</span>vv<span >&#41;</span><span >+</span> dy<span >&#40;</span>v<span >&#41;</span><span >*</span>dy<span >&#40;</span>vv<span >&#41;</span>
            <span >+</span> dx<span >&#40;</span>p<span >&#41;</span><span >*</span>uu <span >+</span> dy<span >&#40;</span>p<span >&#41;</span><span >*</span>vv <span >+</span> pp<span >*</span><span >&#40;</span>dx<span >&#40;</span>u<span >&#41;</span><span >+</span>dy<span >&#40;</span>v<span >&#41;</span><span >&#41;</span>
            <span >-</span><span >1e-10</span><span >*</span>p<span >*</span>pp<span >&#41;</span>            
            <span >+</span> on<span >&#40;</span><span >1</span>,<span >2</span>,<span >4</span>,u<span >=</span><span >0</span>,v<span >=</span><span >0</span><span >&#41;</span> <span >+</span> on<span >&#40;</span><span >3</span>,u<span >=</span><span >1</span>,v<span >=</span><span >0</span><span >&#41;</span><span >;</span>
plot<span >&#40;</span><span >&#91;</span>u,v<span >&#93;</span>,p,wait<span >=</span><span >1</span><span >&#41;</span><span >;</span></pre>

### Un exemple de simulation de Navier-Stokes dans une cavité entrainée avec plusieurs vortex?

Voici un exemple standard de FreeFem qui montre un vortex en bas de la cavité entrainée.

<pre ><span >// remark: the sign of p is correct </span>
real s0<span >=</span><span >clock</span><span >&#40;</span><span >&#41;</span><span >;</span>
mesh Th<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span><span >&#41;</span><span >;</span>
fespace Vh2<span >&#40;</span>Th,P2<span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
Vh2 u2,v2,up1,up2<span >;</span>
Vh2 u1,v1<span >;</span> 
Vh  u1x<span >=</span><span >0</span>,u1y,u2x,u2y, vv<span >;</span>
&nbsp;
real reylnods<span >=</span><span >1000</span><span >;</span>
<span >//cout &lt;&lt; &quot; Enter the reynolds number :&quot;; cin &gt;&gt; reylnods;</span>
<span >assert</span><span >&#40;</span>reylnods<span >&gt;</span><span >1</span> <span >&amp;&amp;</span> reylnods <span >&lt;</span> <span >100000</span><span >&#41;</span><span >;</span> 
up1<span >=</span><span >0</span><span >;</span>
up2<span >=</span><span >0</span><span >;</span> 
func g<span >=</span><span >&#40;</span>x<span >&#41;</span><span >*</span><span >&#40;</span><span >1</span><span >-</span>x<span >&#41;</span><span >*</span><span >4</span><span >;</span> 
Vh p<span >=</span><span >0</span>,q<span >;</span>
real alpha<span >=</span><span >0</span><span >;</span>
real  nu<span >=</span><span >1</span><span >;</span>
<span >int</span> i<span >=</span><span >0</span>,iter<span >=</span><span >0</span><span >;</span>
real dt<span >=</span><span >0</span><span >;</span>
solve NS <span >&#40;</span><span >&#91;</span>u1,u2,p<span >&#93;</span>,<span >&#91;</span>v1,v2,q<span >&#93;</span>,solver<span >=</span>Crout,init<span >=</span>i<span >&#41;</span> <span >=</span>
    int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>
             alpha<span >*</span><span >&#40;</span> u1<span >*</span>v1 <span >+</span> u2<span >*</span>v2<span >&#41;</span> 
            <span >+</span> nu <span >*</span> <span >&#40;</span> dx<span >&#40;</span>u1<span >&#41;</span><span >*</span>dx<span >&#40;</span>v1<span >&#41;</span> <span >+</span> dy<span >&#40;</span>u1<span >&#41;</span><span >*</span>dy<span >&#40;</span>v1<span >&#41;</span>
            <span >+</span>        dx<span >&#40;</span>u2<span >&#41;</span><span >*</span>dx<span >&#40;</span>v2<span >&#41;</span> <span >+</span> dy<span >&#40;</span>u2<span >&#41;</span><span >*</span>dy<span >&#40;</span>v2<span >&#41;</span> <span >&#41;</span>
            <span >+</span> p<span >*</span>q<span >*</span><span >&#40;</span><span >0.000001</span><span >&#41;</span> 
            <span >-</span> p<span >*</span>dx<span >&#40;</span>v1<span >&#41;</span> <span >-</span> p<span >*</span>dy<span >&#40;</span>v2<span >&#41;</span>
            <span >-</span> dx<span >&#40;</span>u1<span >&#41;</span><span >*</span>q <span >-</span> dy<span >&#40;</span>u2<span >&#41;</span><span >*</span>q
           <span >&#41;</span>
  <span >+</span> int2d<span >&#40;</span>Th<span >&#41;</span> <span >&#40;</span> <span >-</span>alpha<span >*</span>convect<span >&#40;</span><span >&#91;</span>up1,up2<span >&#93;</span>,<span >-</span>dt,up1<span >&#41;</span><span >*</span>v1 <span >-</span>alpha<span >*</span>convect<span >&#40;</span><span >&#91;</span>up1,up2<span >&#93;</span>,<span >-</span>dt,up2<span >&#41;</span><span >*</span>v2 <span >&#41;</span>
  <span >+</span> on<span >&#40;</span><span >3</span>,u1<span >=</span>g,u2<span >=</span><span >0</span><span >&#41;</span> 
  <span >+</span> on<span >&#40;</span><span >1</span>,<span >2</span>,<span >4</span>,u1<span >=</span><span >0</span>,u2<span >=</span><span >0</span><span >&#41;</span> <span >;</span>
plot<span >&#40;</span>coef<span >=</span><span >0.2</span>,cmm<span >=</span><span >&quot; [u1,u2] et p  &quot;</span>,p,<span >&#91;</span>u1,u2<span >&#93;</span>,ps<span >=</span><span >&quot;StokesP2P1.eps&quot;</span>,value<span >=</span><span >1</span>,wait<span >=</span><span >1</span><span >&#41;</span><span >;</span>
<span >&#123;</span>
  real<span >&#91;</span><span >int</span><span >&#93;</span> xx<span >&#40;</span><span >21</span><span >&#41;</span>,yy<span >&#40;</span><span >21</span><span >&#41;</span>,pp<span >&#40;</span><span >21</span><span >&#41;</span><span >;</span>
  <span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span><span >21</span><span >;</span>i<span >++</span><span >&#41;</span>
   <span >&#123;</span>
     yy<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >/</span><span >20</span>.<span >;</span>
     xx<span >&#91;</span>i<span >&#93;</span><span >=</span>u1<span >&#40;</span><span >0.5</span>,i<span >/</span><span >20</span>.<span >&#41;</span><span >;</span>
     pp<span >&#91;</span>i<span >&#93;</span><span >=</span>p<span >&#40;</span>i<span >/</span><span >20</span>.,<span >0.999</span><span >&#41;</span><span >;</span>
    <span >&#125;</span>
      <span >cout</span> <span >&lt;&lt;</span> <span >&quot; &quot;</span> <span >&lt;&lt;</span> yy <span >&lt;&lt;</span> endl<span >;</span>
     plot<span >&#40;</span><span >&#91;</span>xx,yy<span >&#93;</span>,wait<span >=</span><span >1</span>,cmm<span >=</span><span >&quot;u1 x=0.5 cup&quot;</span><span >&#41;</span><span >;</span>
     plot<span >&#40;</span><span >&#91;</span>yy,pp<span >&#93;</span>,wait<span >=</span><span >1</span>,cmm<span >=</span><span >&quot;pressure y=0.999 cup&quot;</span><span >&#41;</span><span >;</span>
<span >&#125;</span>
&nbsp;
dt <span >=</span> <span >0.1</span><span >;</span>
<span >int</span> nbiter <span >=</span> <span >5</span><span >;</span>
real coefdt <span >=</span> <span >0.25</span><span >^</span><span >&#40;</span><span >1</span>.<span >/</span>nbiter<span >&#41;</span><span >;</span>
real coefcut <span >=</span> <span >0.25</span><span >^</span><span >&#40;</span><span >1</span>.<span >/</span>nbiter<span >&#41;</span> , cut<span >=</span><span >0.01</span><span >;</span>
real tol<span >=</span><span >0.5</span>,coeftol <span >=</span> <span >0.25</span><span >^</span><span >&#40;</span><span >1</span>.<span >/</span>nbiter<span >&#41;</span><span >;</span>
nu<span >=</span><span >1</span>.<span >/</span>reylnods<span >;</span>   
&nbsp;
<span >for</span> <span >&#40;</span>iter<span >=</span><span >1</span><span >;</span>iter<span >&lt;=</span>nbiter<span >;</span>iter<span >++</span><span >&#41;</span>
<span >&#123;</span>
  <span >cout</span> <span >&lt;&lt;</span> <span >&quot; dt = &quot;</span> <span >&lt;&lt;</span> dt <span >&lt;&lt;</span> <span >&quot; ------------------------ &quot;</span> <span >&lt;&lt;</span> endl<span >;</span>
  alpha<span >=</span><span >1</span><span >/</span>dt<span >;</span>
  <span >for</span> <span >&#40;</span>i<span >=</span><span >0</span><span >;</span>i<span >&lt;=</span><span >50</span><span >;</span>i<span >++</span><span >&#41;</span>
   <span >&#123;</span>
     up1<span >=</span>u1<span >;</span>
     up2<span >=</span>u2<span >;</span>
     NS<span >;</span>
     <span >if</span> <span >&#40;</span> <span >!</span><span >&#40;</span>i <span >%</span> <span >10</span><span >&#41;</span><span >&#41;</span> 
     plot<span >&#40;</span>coef<span >=</span><span >0.2</span>,cmm<span >=</span><span >&quot; [u1,u2] et p  &quot;</span>,p,<span >&#91;</span>u1,u2<span >&#93;</span>,ps<span >=</span><span >&quot;plotNS_&quot;</span><span >+</span>iter<span >+</span><span >&quot;_&quot;</span><span >+</span>i<span >+</span><span >&quot;.eps&quot;</span><span >&#41;</span><span >;</span>  
     <span >cout</span> <span >&lt;&lt;</span> <span >&quot;CPU &quot;</span> <span >&lt;&lt;</span> <span >clock</span><span >&#40;</span><span >&#41;</span><span >-</span>s0 <span >&lt;&lt;</span> <span >&quot;s &quot;</span> <span >&lt;&lt;</span> endl<span >;</span>     
   <span >&#125;</span> 
&nbsp;
  <span >if</span> <span >&#40;</span>iter<span >&gt;=</span> nbiter<span >&#41;</span> <span >break</span><span >;</span>
&nbsp;
  Th<span >=</span>adaptmesh<span >&#40;</span>Th,<span >&#91;</span>dx<span >&#40;</span>u1<span >&#41;</span>,dy<span >&#40;</span>u1<span >&#41;</span>,dx<span >&#40;</span>u1<span >&#41;</span>,dy<span >&#40;</span>u2<span >&#41;</span><span >&#93;</span>,
              abserror<span >=</span><span >0</span>,cutoff<span >=</span>cut,err<span >=</span>tol, inquire<span >=</span><span >0</span>,ratio<span >=</span><span >1.5</span>,hmin<span >=</span><span >1</span>.<span >/</span><span >1000</span><span >&#41;</span><span >;</span>
  plot<span >&#40;</span>Th,ps<span >=</span><span >&quot;ThNS.eps&quot;</span><span >&#41;</span><span >;</span>
  dt <span >=</span> dt<span >*</span>coefdt<span >;</span>
  tol <span >=</span> tol <span >*</span>coeftol<span >;</span>
  cut <span >=</span> cut <span >*</span>coefcut<span >;</span>
<span >&#125;</span>
<span >cout</span> <span >&lt;&lt;</span> <span >&quot;CPU &quot;</span> <span >&lt;&lt;</span> <span >clock</span><span >&#40;</span><span >&#41;</span><span >-</span>s0 <span >&lt;&lt;</span> <span >&quot;s &quot;</span> <span >&lt;&lt;</span> endl<span >;</span>     </pre>

ce qui donne:

freefem-ns-vortex.png <!-- ALHTODO find in dokuwiki backups -->

### Comment savoir à quel région d'un maillage un point appartient?

Utiliser le mot clé “region”.

### Comment afficher la valeur des labels dans tout le maillage?
<pre ><span >// Un exemple de maillage</span>
load <span >&quot;msh3&quot;</span>
<span >int</span> nn<span >=</span><span >4</span><span >;</span>
mesh Th2<span >=</span> square<span >&#40;</span>nn,nn<span >&#41;</span><span >;</span>
<span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> rup<span >=</span><span >&#91;</span><span >0</span>,<span >0</span><span >&#93;</span>,  rdown<span >=</span><span >&#91;</span><span >0</span>,<span >0</span><span >&#93;</span>, rmid<span >=</span><span >&#91;</span><span >1</span>,<span >1</span>,<span >2</span>,<span >2</span>,<span >3</span>,<span >3</span>,<span >4</span>,<span >4</span><span >&#93;</span><span >;</span>
real zmin<span >=</span><span >0</span>,zmax<span >=</span><span >1</span><span >;</span>
mesh3 Th<span >=</span>buildlayers<span >&#40;</span>Th2,nn,
  zbound<span >=</span><span >&#91;</span>zmin,zmax<span >&#93;</span>,
  labelmid<span >=</span>rmid, 
  reffaceup <span >=</span> rup,
  reffacelow <span >=</span> rdown
<span >&#41;</span><span >;</span>
&nbsp;
<span >// Une fonction 'b' contenant les valeurs des labels en chaque point</span>
fespace Vh<span >&#40;</span>Th,P1<span >&#41;</span><span >;</span>
Vh b<span >;</span>
<span >int</span> t<span >;</span>
<span >for</span><span >&#40;</span>t<span >=</span><span >0</span><span >;</span>t<span >&lt;</span>Th.<span >nt</span><span >;</span>t<span >++</span><span >&#41;</span><span >&#123;</span>
	<span >int</span> p<span >;</span>
	<span >for</span><span >&#40;</span>p<span >=</span><span >0</span><span >;</span>p<span >&lt;</span><span >4</span><span >;</span>p<span >++</span><span >&#41;</span><span >&#123;</span>
		b<span >&#91;</span><span >&#93;</span><span >&#40;</span>Th<span >&#91;</span>t<span >&#93;</span><span >&#91;</span>p<span >&#93;</span><span >&#41;</span><span >=</span>Th<span >&#91;</span>t<span >&#93;</span><span >&#91;</span>p<span >&#93;</span>.<span >label</span><span >;</span>
	<span >&#125;</span>
<span >&#125;</span>
&nbsp;
<span >// Représentation graphique de b</span>
plot<span >&#40;</span>b,nbiso<span >=</span><span >20</span>,value<span >=</span><span >1</span><span >&#41;</span><span >;</span></pre>

### Multiplying matrices

This is possible when loading the “lapack” module. eg:

<pre >load <span >&quot;lapack&quot;</span>
real<span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> a<span >&#40;</span><span >2</span>,<span >2</span><span >&#41;</span><span >;</span>
a<span >=</span><span >&#91;</span><span >&#91;</span><span >1</span>,<span >2</span><span >&#93;</span>,<span >&#91;</span><span >3</span>,<span >4</span><span >&#93;</span><span >&#93;</span><span >;</span>
real<span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> b<span >&#40;</span><span >2</span>,<span >2</span><span >&#41;</span><span >;</span>
b<span >=</span>a<span >*</span>a<span >;</span>
<span >cout</span><span >&lt;&lt;</span>b<span >;</span></pre>

See also [http://www.um.es/freefem/ff++/pmwiki.php?n=Main.SparseMatrixTypeOperations](http://www.um.es/freefem/ff++/pmwiki.php?n=Main.SparseMatrixTypeOperations)

### What is the equivalent of #include in FreeFem++?
<pre >include &quot;file.idp&quot;</pre>

The “idp” extension is frequently used for included scripts but not required.

### How to return a vector as the result of a function?

Returning a vector as the value of a function may sometimes pose problems. If the case arises, just tranform the return value into a function parameter.

### Are FreeFem++ functions recursive?

Not at the moment.

### How to make a script wait for a fixed amount of time?

Just use an external sleep command:

<pre ><span >int</span> i<span >;</span>
<span >for</span><span >&#40;</span>i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span><span >10</span><span >;</span>i<span >++</span><span >&#41;</span><span >&#123;</span>
  <span >cout</span><span >&lt;&lt;</span>i<span >&lt;&lt;</span>endl<span >;</span>
  exec<span >&#40;</span><span >&quot;sleep 2&quot;</span><span >&#41;</span><span >;</span> <span >// seconds</span>
<span >&#125;</span></pre>

### How to refine a part of a mesh

Example on a plain square mesh:

<pre >mesh Th1<span >=</span>square<span >&#40;</span><span >30</span>,<span >30</span><span >&#41;</span><span >;</span>
plot<span >&#40;</span>Th1,cmm<span >=</span><span >&quot;Th1&quot;</span><span >&#41;</span><span >;</span></pre>

Refine mesh center and keep structured mesh around it (r2 and u can be changed at will):

<pre >func r2<span >=</span><span >&#40;</span>x<span >-</span><span >0.5</span><span >&#41;</span><span >*</span><span >&#40;</span>x<span >-</span><span >0.5</span><span >&#41;</span><span >+</span><span >&#40;</span>y<span >-</span><span >0.5</span><span >&#41;</span><span >*</span><span >&#40;</span>y<span >-</span><span >0.5</span><span >&#41;</span><span >;</span>
func u<span >=</span><span >1</span><span >+</span><span >1</span><span >/</span><span >&#40;</span><span >0.2</span><span >+</span><span >10</span><span >*</span>r2<span >&#41;</span><span >;</span>
mesh Th2<span >=</span>splitmesh<span >&#40;</span>Th1,u<span >&#41;</span><span >;</span>
plot<span >&#40;</span>Th2,cmm<span >=</span><span >&quot;Th2&quot;</span><span >&#41;</span><span >;</span></pre>

### FreeFem++ quadrature formulae

<em >note:* all quadrature formulae with letter “T” apply to triangles, and “E” apply to edges.

### How to start writing to a file from scratch and then append to it?

<pre ><span >&#123;</span>
  ofstream f<span >&#40;</span><span >&quot;toto.txt&quot;</span><span >&#41;</span><span >;</span>
  f <span >&lt;&lt;</span> <span >&quot;coucou'<span >\n</span>&quot;</span><span >;</span>
<span >&#125;</span><span >;</span></pre>

Then to append to the same file:

<pre ><span >&#123;</span>
  ofstream f<span >&#40;</span><span >&quot;toto.txt&quot;</span><span >,</span>append<span >&#41;</span><span >;</span>
  f <span >&lt;&lt;</span> <span >&quot;add coucou'<span >\n</span>&quot;</span><span >;</span>
<span >&#125;</span><span >;</span></pre>

### How to randomize a symetric mesh to check if its regularity has an impact on numerical results?

Here is an example with a square:

<pre ><span >int</span> n<span >=</span><span >10</span><span >;</span>
mesh m<span >=</span>square<span >&#40;</span>n<span >,</span>n<span >&#41;</span><span >;</span>
<span >for</span><span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span><span >100</span><span >;</span>i<span >++</span><span >&#41;</span><span >&#123;</span>
  m<span >=</span>adaptmesh<span >&#40;</span>m<span >,</span><span >1</span>.<span >/</span>n<span >,</span>IsMetric<span >=</span><span >1</span><span >&#41;</span><span >;</span>
  plot<span >&#40;</span>m<span >&#41;</span><span >;</span>
<span >&#125;</span></pre>

### How to copy a sparse matrix into a dense matrix?
<pre ><span >// Construction d'une matrice creuse</span>
&nbsp;
mesh Th<span >=</span>square<span >&#40;</span><span >10</span><span >,</span><span >10</span><span >&#41;</span><span >;</span>
plot<span >&#40;</span>Th<span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th<span >,</span>P1<span >&#41;</span><span >;</span>
Vh uh<span >,</span>vh<span >;</span>
varf laplaceA<span >&#40;</span>uh<span >,</span>vh<span >&#41;</span><span >=</span>int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>uh<span >&#41;</span><span >*</span>dx<span >&#40;</span>vh<span >&#41;</span><span >+</span>dy<span >&#40;</span>uh<span >&#41;</span><span >*</span>dy<span >&#40;</span>vh<span >&#41;</span><span >&#41;</span><span >;</span>
matrix SA<span >=</span>laplaceA<span >&#40;</span>Vh<span >,</span>Vh<span >&#41;</span><span >;</span>
&nbsp;
<span >// Conversion de la matrice creuse en matrice pleine</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >,</span><span >int</span><span >&#93;</span> FA<span >&#40;</span>SA.<span >n</span><span >,</span>SA.<span >n</span><span >&#41;</span><span >;</span>
&nbsp;
<span >// This does not work</span>
<span >// &quot;error operator =  &lt;P3KNMIdE&gt;, &lt;14Matrice_CreuseIdE&gt;&quot;</span>
&nbsp;
<span >//FA=SA;</span>
&nbsp;
<span >// This does not work</span>
<span >// &quot;Error: the coef a(0,2)  do'nt exist in sparse matrix  Matrix  type = P14Matrice_CreuseIdE&quot;</span>
&nbsp;
<span >//for(int i=0;i&lt;SA.n;i++)</span>
<span >//  for(int j=0;j&lt;SA.n;j++)</span>
<span >//    FA(i,j)=SA(i,j);</span>
&nbsp;
<span >// This is ok</span>
&nbsp;
<span >&#123;</span>
  real<span >&#91;</span><span >int</span><span >&#93;</span> coef<span >;</span>
  <span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> lg<span >;</span>
  <span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> cl<span >;</span>
  <span >&#91;</span>lg<span >,</span>cl<span >,</span>coef<span >&#93;</span><span >=</span>SA<span >;</span> 
&nbsp;
  FA<span >=</span><span >0</span><span >;</span>
  <span >for</span><span >&#40;</span><span >int</span> c<span >=</span><span >0</span><span >;</span>c<span >&lt;</span>coef.<span >n</span><span >;</span>c<span >++</span><span >&#41;</span>FA<span >&#40;</span>lg<span >&#40;</span>c<span >&#41;</span><span >,</span>cl<span >&#40;</span>c<span >&#41;</span><span >&#41;</span><span >=</span>coef<span >&#40;</span>c<span >&#41;</span><span >;</span>
<span >&#125;</span>
&nbsp;
<span >// just a test to see if SA and FA are identical</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >&#93;</span> one<span >&#40;</span>SA.<span >n</span><span >&#41;</span><span >;</span>
one<span >=</span><span >1</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> SAone<span >=</span>SA<span >*</span>one<span >;</span>
cout<span >&lt;&lt;</span>SAone.<span >max</span><span >&lt;&lt;</span>endl<span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> FAone<span >=</span>FA<span >*</span>one<span >;</span>
cout<span >&lt;&lt;</span>FAone.<span >max</span><span >&lt;&lt;</span>endl<span >;</span></pre>

### Comment déterminer les valeurs et vecteurs propres d'un matrice?

Voici l'exemple LapEigenValue.edp

<pre ><span >//  Computation of the eigen value and eigen vector of the </span>
<span >// Dirichlet problem  on square $]0,\pi[^2$</span>
<span >// ----------------------------------------</span>
<span >// we use the inverse shift mode </span>
<span >// the shift is given with sigma real</span>
<span >// -------------------------------------</span>
<span >//  find $\lamda$ such that:</span>
<span >// $$  \int_{\omega}  \nabla u_ \nabla v = \lamba \int_{\omega} u \nabla v  $$</span>
verbosity<span >=</span><span >1</span><span >;</span>
mesh Th<span >=</span>square<span >&#40;</span><span >20</span>,<span >20</span>,<span >&#91;</span>pi<span >*</span>y,pi<span >*</span>x<span >&#93;</span><span >&#41;</span><span >;</span>
fespace Vh<span >&#40;</span>Th,P2<span >&#41;</span><span >;</span>
Vh u1,u2<span >;</span>
&nbsp;
&nbsp;
real sigma <span >=</span> <span >00</span><span >;</span>  <span >// value of the shift </span>
&nbsp;
varf  a<span >&#40;</span>u1,u2<span >&#41;</span><span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>  dx<span >&#40;</span>u1<span >&#41;</span><span >*</span>dx<span >&#40;</span>u2<span >&#41;</span> <span >+</span> dy<span >&#40;</span>u1<span >&#41;</span><span >*</span>dy<span >&#40;</span>u2<span >&#41;</span> <span >-</span> sigma<span >*</span> u1<span >*</span>u2 <span >&#41;</span>
                    <span >+</span>  on<span >&#40;</span><span >1</span>,<span >2</span>,<span >3</span>,<span >4</span>,u1<span >=</span><span >0</span><span >&#41;</span> <span >;</span>  <span >// Boundary condition</span>
&nbsp;
varf b<span >&#40;</span><span >&#91;</span>u1<span >&#93;</span>,<span >&#91;</span>u2<span >&#93;</span><span >&#41;</span> <span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>  u1<span >*</span>u2 <span >&#41;</span> <span >;</span> <span >// no  Boundary condition</span>
&nbsp;
matrix A<span >=</span> a<span >&#40;</span>Vh,Vh,solver<span >=</span>Crout,factorize<span >=</span><span >1</span><span >&#41;</span><span >;</span> 
matrix B<span >=</span> b<span >&#40;</span>Vh,Vh,solver<span >=</span>CG,eps<span >=</span><span >1e-20</span><span >&#41;</span><span >;</span> 
&nbsp;
<span >// important remark:</span>
<span >// the boundary condition is make with exact penalisation:</span>
<span >//     we put 1e30=tgv  on the diagonal term of the lock degre of freedom.</span>
<span >//  So take dirichlet boundary condition just on $a$ variationnal form</span>
<span >// and not on  $b$ variationnanl form.</span>
<span >// because we solve</span>
<span >//  $$ w=A^-1*B*v $$</span>
&nbsp;
<span >int</span> nev<span >=</span><span >20</span><span >;</span>  <span >// number of computed eigen valeu close to sigma</span>
&nbsp;
real<span >&#91;</span><span >int</span><span >&#93;</span> ev<span >&#40;</span>nev<span >&#41;</span><span >;</span> <span >// to store nev eigein value</span>
Vh<span >&#91;</span><span >int</span><span >&#93;</span> eV<span >&#40;</span>nev<span >&#41;</span><span >;</span>   <span >// to store nev eigen vector</span>
&nbsp;
&nbsp;
<span >int</span> k<span >=</span>EigenValue<span >&#40;</span>A,B,sym<span >=</span><span >true</span>,sigma<span >=</span>sigma,value<span >=</span>ev,vector<span >=</span>eV,tol<span >=</span><span >1e-10</span>,maxit<span >=</span><span >0</span>,ncv<span >=</span><span >0</span><span >&#41;</span><span >;</span>
<span >//   tol= the tolerace</span>
<span >//   maxit= the maximal iteration see arpack doc.</span>
<span >//   ncv   see arpack doc.</span>
<span >//  the return value is number of converged eigen value.</span>
k<span >=</span>min<span >&#40;</span>k,nev<span >&#41;</span><span >;</span> <span >//  some time the number of converged eigen value </span>
              <span >// can be greater than nev;</span>
<span >int</span> nerr<span >=</span><span >0</span><span >;</span>
real<span >&#91;</span><span >int</span><span >&#93;</span>  eev<span >&#40;</span><span >36</span><span >&#41;</span><span >;</span>
eev<span >=</span><span >1e100</span><span >;</span>
<span >for</span><span >&#40;</span><span >int</span> i<span >=</span><span >1</span>,k<span >=</span><span >0</span><span >;</span>i<span >&lt;</span><span >6</span><span >;</span><span >++</span>i<span >&#41;</span>
<span >for</span><span >&#40;</span><span >int</span> j<span >=</span><span >1</span><span >;</span>j<span >&lt;</span><span >6</span><span >;</span><span >++</span>j<span >&#41;</span>
  eev<span >&#91;</span>k<span >++</span><span >&#93;</span><span >=</span>i<span >*</span>i<span >+</span>j<span >*</span>j<span >;</span>
eev.<span >sort</span><span >;</span>
<span >cout</span> <span >&lt;&lt;</span> eev <span >&lt;&lt;</span> endl<span >;</span>
<span >for</span> <span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span>k<span >;</span>i<span >++</span><span >&#41;</span>
<span >&#123;</span>
  u1<span >=</span>eV<span >&#91;</span>i<span >&#93;</span><span >;</span>
  real gg <span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>u1<span >&#41;</span><span >*</span>dx<span >&#40;</span>u1<span >&#41;</span> <span >+</span> dy<span >&#40;</span>u1<span >&#41;</span><span >*</span>dy<span >&#40;</span>u1<span >&#41;</span><span >&#41;</span><span >;</span>
  real mm<span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>u1<span >*</span>u1<span >&#41;</span> <span >;</span>
  real err <span >=</span> int2d<span >&#40;</span>Th<span >&#41;</span><span >&#40;</span>dx<span >&#40;</span>u1<span >&#41;</span><span >*</span>dx<span >&#40;</span>u1<span >&#41;</span> <span >+</span> dy<span >&#40;</span>u1<span >&#41;</span><span >*</span>dy<span >&#40;</span>u1<span >&#41;</span> <span >-</span> <span >&#40;</span>ev<span >&#91;</span>i<span >&#93;</span><span >&#41;</span><span >*</span>u1<span >*</span>u1<span >&#41;</span> <span >;</span>
  <span >if</span><span >&#40;</span><span >abs</span><span >&#40;</span>err<span >&#41;</span> <span >&gt;</span> <span >1e-6</span><span >&#41;</span> nerr<span >++</span><span >;</span>
  <span >if</span><span >&#40;</span><span >abs</span><span >&#40;</span>ev<span >&#91;</span>i<span >&#93;</span><span >-</span>eev<span >&#91;</span>i<span >&#93;</span><span >&#41;</span> <span >&gt;</span> <span >1e-1</span><span >&#41;</span> nerr<span >++</span><span >;</span>
  <span >cout</span> <span >&lt;&lt;</span> <span >&quot; ---- &quot;</span> <span >&lt;&lt;</span>  i<span >&lt;&lt;</span> <span >&quot; &quot;</span> <span >&lt;&lt;</span> ev<span >&#91;</span>i<span >&#93;</span> <span >&lt;&lt;</span> <span >&quot; == &quot;</span> <span >&lt;&lt;</span> eev<span >&#91;</span>i<span >&#93;</span> <span >&lt;&lt;</span> <span >&quot; err= &quot;</span> <span >&lt;&lt;</span> err <span >&lt;&lt;</span> <span >&quot; --- &quot;</span><span >&lt;&lt;</span>endl<span >;</span>
&nbsp;
  <span >// FFCS: add 3D view capabilities</span>
  plot<span >&#40;</span>eV<span >&#91;</span>i<span >&#93;</span>,cmm<span >=</span><span >&quot;Eigen  Vector &quot;</span><span >+</span>i<span >+</span><span >&quot; valeur =&quot;</span> <span >+</span> ev<span >&#91;</span>i<span >&#93;</span>  ,wait<span >=</span><span >1</span>,value<span >=</span><span >1</span>,ps<span >=</span><span >&quot;eigen&quot;</span><span >+</span>i<span >+</span><span >&quot;.eps&quot;</span>,dim<span >=</span><span >3</span>,fill<span >=</span><span >1</span>,CutPlane<span >=</span><span >0</span>,ShowAxes<span >=</span><span >0</span><span >&#41;</span><span >;</span>
<span >&#125;</span>
<span >assert</span><span >&#40;</span>nerr<span >==</span><span >0</span><span >&#41;</span><span >;</span></pre>

### Comment arrondir une valeur réelle à un nombre fixe de décimales?
<pre >real a<span >=</span><span >1</span>.<span >/</span><span >3</span>.<span >;</span>
<span >cout</span><span >&lt;&lt;</span>a<span >&lt;&lt;</span>endl<span >;</span>
a<span >=</span><span >int</span><span >&#40;</span>a<span >*</span><span >1000</span>.<span >&#41;</span><span >/</span><span >1000</span>.<span >;</span>
<span >cout</span><span >&lt;&lt;</span>a<span >&lt;&lt;</span>endl<span >;</span></pre>

Résultat :

<pre >0.333333
0.333
times: compile 0.01s, execution 1.10961e-18s,  mpirank:0
 CodeAlloc : nb ptr  2373,  size :160416 mpirank: 0
Bien: On a fini Normalement</pre>

### Comment lire une matrice calculée par FreeFem++ dans Matlab?

Voici un [script Matlab](http://www.um.es/freefem/ff++/uploads/Main/FFmatrix_fread.m) écrit par Richard MICHEL et publié sur le [wiki FreeFem++](http://www.um.es/freefem/ff++/pmwiki.php).

### Comment appeler ARPACK pour une matrice sans maillage associé?
<pre ><span >int</span> nev<span >=</span><span >5</span><span >;</span> <span >// number of computed eigenvalue close to sigma</span>
real<span >&#91;</span><span >int</span><span >&#93;</span> ev<span >&#40;</span>nev<span >&#41;</span><span >;</span> <span >// to store nev eigenvalues</span>
real<span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> eV<span >&#40;</span>AA.<span >n</span>,nev<span >&#41;</span><span >;</span> <span >// to store nev eigenvectors</span>
<span >int</span> k<span >=</span>EigenValue<span >&#40;</span>AA,BB,sym<span >=</span><span >true</span>,value<span >=</span>ev,rawvector<span >=</span>eV<span >&#41;</span><span >;</span></pre>

### Comment exécuter Matlab depuis FreeFem++?

Dans le script FreeFem++ : (testé sur Windows et Linux)

<pre >exec(&quot;matlab -automation -r \&quot;run('/path/vers/le/script/matlab.m')\&quot; &quot;)</pre>

### Fusionner deux maillages le long d'une frontière interne

L'important est de donner un label distinct à la portion de frontière qui sera à l'intérieur du maillage pour que les conditions aux bords ne lui soient pas appliquées:

<pre ><span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> l1<span >=</span><span >&#91;</span><span >1</span>,<span >2</span>,<span >1</span>,<span >1</span><span >&#93;</span><span >;</span>
mesh m1<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span>,label<span >=</span>l1<span >&#41;</span><span >;</span>
<span >int</span><span >&#91;</span><span >int</span><span >&#93;</span> l2<span >=</span><span >&#91;</span><span >1</span>,<span >1</span>,<span >1</span>,<span >2</span><span >&#93;</span><span >;</span>
mesh m2<span >=</span>square<span >&#40;</span><span >10</span>,<span >10</span>,<span >&#91;</span>x<span >+</span><span >1</span>,y<span >&#93;</span>,label<span >=</span>l2<span >&#41;</span><span >;</span>
plot<span >&#40;</span>m1,m2<span >&#41;</span><span >;</span>
mesh m<span >=</span>m1<span >+</span>m2<span >;</span>
plot<span >&#40;</span>m<span >&#41;</span><span >;</span></pre>

### Créer une matrice pleine et la convertir en matrice creuse

<pre ><span >int</span> N<span >=</span><span >10</span><span >;</span>
complex <span >&#91;</span><span >int</span>,<span >int</span><span >&#93;</span> A<span >&#40;</span>N,N<span >&#41;</span><span >;</span>
A<span >=</span><span >0</span><span >;</span>
<span >for</span><span >&#40;</span><span >int</span> i<span >=</span><span >0</span><span >;</span>i<span >&lt;</span>N<span >;</span>i<span >++</span><span >&#41;</span><span >&#123;</span>
  A<span >&#40;</span>i,i<span >&#41;</span><span >=</span><span >1</span>.<span >+</span>i<span >;</span>
  <span >if</span><span >&#40;</span>i<span >+</span><span >1</span> <span >&lt;</span> N<span >&#41;</span>    A<span >&#40;</span>i,i<span >+</span><span >1</span><span >&#41;</span><span >=</span><span >-</span>i<span >-</span>1i<span >*</span>i<span >;</span>
  a<span >&#91;</span>i<span >&#93;</span><span >=</span>i<span >*</span><span >&#40;</span><span >1</span>.<span >+</span>2i<span >&#41;</span><span >;</span>
<span >&#125;</span>
&nbsp;
matrix<span >&lt;</span>complex<span >&gt;</span> sparseA<span >=</span>A<span >;</span>
<span >cout</span> <span >&lt;&lt;</span> sparseA <span >&lt;&lt;</span> endl<span >;</span></pre>

Voir aussi [How to copy a sparse matrix into a dense matrix?](#how_to_copy_a_sparse_matrix_into_a_dense_matrix)

<p>&nbsp;</p>

<!-- <<<Radia>>> -->
## <a name="Radia"></a> Radia

"*Main features - Saturated iron &amp; anisotropic materials - Polyhedron shapes - Straight and curved current coils - Easy modeling and meshing - Fast 3D visualization with QuickDraw 3D or Mathematica - Parameterization of the models in the Mathematica Language - Fast solving - Semi-analytical computation of field, field integrals and forces - Operates on MacOs and Windows 95/NT - Authors  : O. Chubar, P.  Elleaume, J. Chavanne*"

### Web

[http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia](http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia)

### Documentation

[http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia/Documentation](http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia/Documentation)

### Exemples

[http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia/Examples](http://www.esrf.fr/Accelerators/Groups/InsertionDevices/Software/Radia/Examples)

### Autres indications

Binary only download. Requires Mathematica.

<p>&nbsp;</p>

<!-- <<<reutilisation>>> -->
## <a name="reutilisation"></a> Formats Standard Réutilisables et Conversions entre Formats
<ul>
<li > Formats standard : [3D-Studio](#3d_studio), [AutoCAD DXF](#autocad_dxf), [HDF](#hdf), [I-DEAS file format](#i_deas_file_format), [IGES](#iges), [Matlab MAT-Files](#matlab_mat_files), [Matrix Market Exchange Formats](#matrix_market_exchange_formats), [OFF](#off), [Povray](#povray), [Salomé MED](#salome), [STEP](#step), [STL file format](#stl_file_format), [VRML](#vrml)
</li>
</ul>
<ul>
<li > Conversion entre formats de données : [medit2dx](#medit2dx), [NCO](#nco)
</li>
</ul>

<p>&nbsp;</p>

<!-- <<<Rheolef>>> -->
## <a name="Rheolef"></a> Rheolef

"*This is rheolef, a computer environment that serves as a convenient “laboratory” for computations involving finite element-like methods. It provides a set of unix commands and [C++](#cxx) algorithms and containers. This environment is currently under development.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/rheolef)

<ul>
<li > Documentation: [User guide](http://ljk.imag.fr/membres/Pierre.Saramito/rheolef/usrman.pdf), [Reference manual](http://ljk.imag.fr/membres/Pierre.Saramito/rheolef/#rheolefl)
</li>
<li > Informations sur les formats de données: Rheolef understands the following formats (among others) : [Bamg](#bamg), [VTK](#vtk),  [Matrix Market Exchange Formats](#matrix_market_exchange_formats), [Matlab](#matlab), Postscript, [Geomview](#geomview), [Gnuplot](#gnuplot), [Plotmtv](#plotmtv), x3d
</li>
</ul>

<p>&nbsp;</p>

<!-- <<<rlabplus>>> -->
## <a name="rlabplus"></a> rlabplus

"*.. RLaB is an interactive, interpreted scientific programming environment. RLaB is a very high level language intended to provide fast prototyping and program development, as well as easy data-visualization, and processing. RLaB is not a clone of languages such as those used by tools like [Matlab](#matlab) or Matrix-X/Xmath. However, as RLaB focuses on creating a good experimental environment (or laboratory) in which to do matrix math, it can be called ”[Matlab](#matlab)-like“; since the programming language possesses similar operators and concepts.*

*RLaB does not try to be a [Matlab](#matlab) clone. Instead, it borrows what I believe are the best features of the [Matlab](#matlab) language and provides improved language syntax and semantics. The syntax has been improved to allow users more expression and reduce ambiguities. The variable scoping rules have been improved to facilitate creation of larger programs and program libraries. A heterogeneous associative array has been added to allow users to create and operate on arbitrary data structures. The fundamental data type is a floating point matrix (either real or complex), though RLaB also includes string matrices, and sparse numerical matrices (both real and complex).*

*Project rlabplus is a continuation of work on an open-source scripting environment for scientific computations RLaB2.  Project rlabplus provides release 2 of RLaB2, which contains upgrades of the numerical libraries used in the first release, and many new libraries and toolkits, e.g., [GNU Scientific Library](#gnu_scientific_library) (GSL). Original RLaB was created by Ian Searle and collaborators. Rlabplus is a creation of Marijan Kostrun.*"

<ul>
<li > Web: [http://rlabplus.sourceforge.net/](http://rlabplus.sourceforge.net/)
</li>
<li > Documentation: [http://sourceforge.net/project/showfiles.php?group_id=109254](http://sourceforge.net/project/showfiles.php?group_id=109254), [screenshot](http://rlabplus.sourceforge.net/rlab-screenshot1.jpg)
</li>
</ul>

<p>&nbsp;</p>

<!-- <<<Sage>>> -->
## <a name="Sage"></a> Sage

"*Sage is a free open-source mathematics software system licensed under the **GPL**. It combines the power of many existing open-source packages into a common [Python](#python)-based interface. Mission: Creating a viable free open source alternative to Magma, Maple, Mathematica and Matlab.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/sage)

<p>&nbsp;</p>

<!-- <<<Salomé>>> -->
## <a name="Salomé"></a> Salomé

"*SALOME is a free software that provides a generic platform for Pre and Post-Processing for numerical simulation. It is based on an open and flexible architecture made of reusable components available as free software.  It is open-source ([LGPL](#licences_pour_logiciels_libres)), and you can download both the sourcecode and the executables from this site.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/salome)

<em >Format de données standard lus :* [Code_Aster](#code_aster), [Gmsh](#gmsh), [I-DEAS file format](#i_deas_file_format), [IGES](#iges), [Netgen](#netgen), <span >[Salomé MED](#salome)</span>, [STEP](#step)

<em >Format de données standard écrits :* [Code_Aster](#code_aster), [Gmsh](#gmsh), [I-DEAS file format](#i_deas_file_format), [IGES](#iges), [Netgen](#netgen), <span >[Salomé MED](#salome)</span>, [STEP](#step)

#<!-- <<<Questions/Réponses>>> -->
## <a name="Questions/Réponses"></a> Questions/Réponses

#### Version Windows

Une version pour Windows (version de test, pas la plus récente mais fonctionnelle) est téléchargeable à [http://files.salome-platform.org/cea/adam/salomewindows/download](http://files.salome-platform.org/cea/adam/salomewindows/download)

<p>&nbsp;</p>

<!-- <<<ScaLAPACK>>> -->
## <a name="ScaLAPACK"></a> ScaLAPACK

"*The ScaLAPACK (or Scalable LAPACK) library includes a subset of [LAPACK](#lapack) routines redesigned for distributed memory MIMD parallel computers. It is currently written in a Single-Program-Multiple-Data style using explicit message passing for interprocessor communication. It assumes matrices are laid out in a two-dimensional block cyclic decomposition.*

*ScaLAPACK is designed for heterogeneous computing and is portable on any computer that supports [MPI](#mpi) or PVM.*

*Like [LAPACK](#lapack), the ScaLAPACK routines are based on block-partitioned algorithms in order to minimize the frequency of data movement between different levels of the memory hierarchy. (For such machines, the memory hierarchy includes the off-processor memory of other processors, in addition to the hierarchy of registers, cache, and local memory on each processor.) The fundamental building blocks of the ScaLAPACK library are distributed memory versions ([PBLAS](#pblas)) of the Level 1, 2 and 3 BLAS, and a set of Basic Linear Algebra Communication Subprograms ([BLACS](#blacs)) for communication tasks that arise frequently in parallel linear algebra computations. In the ScaLAPACK routines, all interprocessor communication occurs within the [PBLAS](#pblas) and the [BLACS](#blacs). One of the design goals of ScaLAPACK was to have the ScaLAPACK routines resemble their [LAPACK](#lapack) equivalents as much as possible.*"

### Web

[http://www.netlib.org/scalapack/#scalapack_homel](http://www.netlib.org/scalapack/#scalapack_homel)

### Documentation

[Tutorial](http://www.netlib.org/scalapack/tutorial/#indexl),

[User's guide](http://www.netlib.org/scalapack/slug/#indexl), 

[FAQ](http://www.netlib.org/scalapack/#faql)

### Exemples

[http://www.netlib.org/scalapack/examples/#indexl](http://www.netlib.org/scalapack/examples/#indexl)

<p>&nbsp;</p>

<!-- <<<Scilab>>> -->
## <a name="Scilab"></a> Scilab

"*Scilab (developped since 1989 by Scilab Group) is a scientific software package for numerical computations providing a powerful open computing environment for engineering and scientific applications. Distributed freely via the Internet since 1994, Scilab is currently being used in educational and industrial environnments around the world.*

*Scilab includes hundreds of mathematical functions with the possibility to add interactively programs from various languages ([C](#c), [Fortran](#fortran)…). It has sophisticated data structures (including lists, polynomials, rational functions, linear systems…), an interpreter and a high level programming language.*

*Scilab has been conceived to be an open system where the user can define new data types and operations on these data types by using overloading.*

[Fiche PLUME](http://www.projet-plume.org/fiche/scilab)

<p>&nbsp;</p>

### Questions/Réponses

#### Quelques commandes pour démarrer

Lire une matrice stockée dans un fichier texte

<pre >  A = fscanfMat('fichier')</pre>

Extraire une ligne ou une colonne de cette matrice

<pre >A(:,1)</pre>

Un graphe en 2D

<pre >plot2d(A)</pre>

Executer un script enregistré dans un fichier

<pre >exec('fichier')</pre>

<p>&nbsp;</p>

<!-- <<<screen>>> -->
## <a name="screen"></a> screen

exécute chaque commande comme si elle disposait de son propre écran virtuel :

<ul>
<li > Démarrer un programme avec son propre écran :
</li>
</ul>
<pre >screen &lt;programme&gt;</pre>
<ul>
<li > Cacher un écran (sans arrêter les programmes qu'il contient m&amp;ecirc;me si on se d&amp;eacute;connecte) : Control-A d
</li>
<li > Revenir à un écran caché :
</li>
</ul>
<pre >screen -r</pre>
<ul>
<li > Aide :
</li>
</ul>
<pre >man screen</pre>

<p>&nbsp;</p>

<!-- <<<SLEPc>>> -->
## <a name="SLEPc"></a> SLEPc

"*SLEPc, the Scalable Library for Eigenvalue Problem Computations, is a software library for the solution of large sparse eigenproblems on parallel computers. It can be used for the solution of problems formulated in either standard or generalized form, as well as other related problems such as the singular value decomposition.*

*The emphasis of the software is on methods and techniques appropriate for problems in which the associated matrices are sparse, for example, those arising after the discretization of partial differential equations. Therefore, most of the methods offered by the library are projection methods or other methods with similar properties. Examples of these methods are Arnoldi, Lanczos and Subspace Iteration, to name a few. SLEPc implements these basic methods as well as more sophisticated algorithms. It also provides built-in support for spectral transformations such as the shift-and-invert technique. SLEPc is a general library in the sense that it covers standard and generalized eigenvalue problems, both Hermitian and non-Hermitian, with either real or complex arithmetic.*

*SLEPc is built on top of [PETSc](#petsc), the Portable, Extensible Toolkit for Scientific Computation. It can be considered an extension of PETSc providing all the functionality necessary for the solution of eigenvalue problems. This means that PETSc must be previously installed in order to use SLEPc. PETSc users will find SLEPc very easy to use, since it enforces the same programming paradigm. For those users which are not familiar with PETSc yet, our recommendation is to fully understand its basic concepts before proceeding with SLEPc.*"

### Web

[http://www.grycap.upv.es/slepc/](http://www.grycap.upv.es/slepc/)

### Informations sur les formats de données

"*SLEPc interfaces to some external software packages such as [ARPACK](#arpack), BLZPACK, PLANSO, TRLAN and LOBPCG.*"

<p>&nbsp;</p>

<!-- <<<SLFCFD>>> -->
## <A NAME="SLFCFD"></A> SLFCFD

"*SLFCFD stands for San Le's Free Computational Fluid Dynamics. It is a package of scientific software and graphical user interfaces for use in computational fluid dynamics. It is written in ANSI [C](#c) by San Le and distributed under the terms of the [GNU](#licences_pour_logiciels_libres) license.*"

### Web

[http://slfcfd.sourceforge.net/](http://slfcfd.sourceforge.net/)

### Documentation

[http://slfcfd.sourceforge.net/#faql](http://slfcfd.sourceforge.net/#faql)

### Téléchargement

[http://sourceforge.net/projects/slfcfd/](http://sourceforge.net/projects/slfcfd/)

### Exemples

[http://slfcfd.sourceforge.net/#galleryl](http://slfcfd.sourceforge.net/#galleryl)

<p>&nbsp;</p>

<!-- <<<SLFFEA>>> -->
## <A NAME="SLFFEA"></A> SLFFEA

"*SLFFEA stands for San Le's Free Finite Element Analysis. It is a package of scientific software and graphical user interfaces for use in finite element analysis. It is written in ANSI [C](#c) by San Le and distributed under the terms of the [GNU license](#licences_pour_logiciels_libres).*"

### Web

[http://slffea.sourceforge.net/](http://slffea.sourceforge.net/)

### Documentation

[http://slffea.sourceforge.net/#faql](http://slffea.sourceforge.net/#faql)

### Téléchargement

[http://slffea.sourceforge.net/#downloadl](http://slffea.sourceforge.net/#downloadl)

### Exemples

[http://slffea.sourceforge.net/#galleryl](http://slffea.sourceforge.net/#galleryl)

<p>&nbsp;</p>

<!-- <<<SPARSE>>> -->
## <A NAME="SPARSE"></A> SPARSE

"*SPARSE consists of a set of [C](#c) procedures for solving large sparse real or complex linear systems. Besides being able to solve linear systems, it solves transposed systems, finds determinants, and estimates errors due to ill-conditioning in the system of equations and instability in the computations. SPARSE does not require symmetry and is able to perform numerical pivoting (either diagonal or complete) to avoid unnecessary error in the solution. It was originally written for use in circuit simulators and is particularly apt at handling node- and modified-node admittance matrices.*"

### Web

[http://www.netlib.org/sparse/#indexl](http://www.netlib.org/sparse/#indexl)

### Documentation

[http://www.netlib.org/sparse/readme](http://www.netlib.org/sparse/readme)

<p>&nbsp;</p>

<!-- <<<SparseLib++>>> -->
## <a name="SparseLib++"></a> SparseLib++

"*SparseLib++ is a [C++](#cxx) class library for efficient sparse matrix computations across various computational platforms. The software package consists of matrix classes encompassing several sparse storage formats (e.g. compressed row, compressed column and coordinate formats), and providing basic functionality for managing sparse matrices. The Sparse BLAS Toolkit is used to for efficient kernel mathematical operations (e.g. sparse matrix-vector multiply) and to enhance portability and performance across a wide range of computer architectures. Included in the package are various preconditioners commonly used in iterative solvers for linear systems of equations. The focus is on computational support for iterative methods (for example, see IML++), but the sparse matrix objects presented here can be used in their own right.*

*SparseLib++ matrices can be built out of nearly any C++ matrix/vector classes; it is shipped with the MV++ classes by default.*"

### Auteur(s)

"*Sparselib++ authors are Roldan Pozo, Karin Remington, and Andrew Lumsdaine.*"

### Web

[http://math.nist.gov/sparselib++](http://math.nist.gov/sparselib%2b%2b)

### Documentation

[SparseLib++ Sparse Matrix Class Library, User's Guide](http://math.nist.gov/sparselib%2b%2b/parselib-userguide.pdf)

<p>&nbsp;</p>

<!-- <<<SPOOLES>>> -->
## <A NAME="SPOOLES"></A> SPOOLES

"*SPOOLES 2.2 : SParse Object Oriented Linear Equations Solver*"

"*SPOOLES is a library for solving sparse real and complex linear systems of equations, written in the [C](#c) language using object
oriented design. At present, there is the following functionality:*

1. *Compute multiple minimum degree, generalized nested dissection and multisection orderings of matrices with symmetric structure.*
2. *Factor and solve square linear systems of equations with symmetric structure, with or without pivoting for stability. The factorization
   can be symmetric LDLT, Hermitian LDLH, or nonsymmetric LDU. A direct factorization or a drop tolerance factorization can be computed. The
   factors and solve can be done in serial mode, multithreaded with Solaris or POSIX threads, or with [MPI](#mpi).*
3. *Factor and solve overdetermined full rank systems of equations using a multifrontal QR factorization, in serial or using POSIX threads.*
4. *Solve square linear systems using a variety of Krylov iterative methods. The preconditioner is a drop tolerance factorization,
   constructed with or without pivoting for stability.*"

### Web

[http://www.netlib.org/linalg/spooles/spooles.2.#2l](http://www.netlib.org/linalg/spooles/spooles.2.#2l)

### Licence

"*This release is entirely within the public domain; there are no licensing restrictions, and there is no warranty of any sort.*"

<p>&nbsp;</p>

<!-- <<<STEP>>> -->
## <A NAME="STEP"></A> STEP

"*STEP, the Standard for the Exchange of Product Model Data, is a comprehensive ISO standard (ISO 10303) that describes how to represent and
exchange digital product information.*"

### Web

[http://www.steptools.com/library/standard/](http://www.steptools.com/library/standard/)

### Logiciels capables de lire ce format

[Netgen](#netgen), [Salomé](#salome)

### Logiciels capables d'écrire dans ce format

[Salomé](#salome)

<p>&nbsp;</p>

<!-- <<<STL file format>>> -->
## <a name="STL file format"></a> STL file format

"*The .stl or stereolithography format is an **ASCII** or binary file used in manufacturing. It is a list of the triangular surfaces that
describe a computer generated solid model. This is the standard input for most rapid prototyping machines.*"

### Documentation

[http://www.ennex.com/~fabbers/StL.asp](http://www.ennex.com/~fabbers/StL.asp)

### Logiciels capables de lire ce format

[ADMesh](#admesh)

### Logiciels capables d'écrire dans ce format

[ADMesh](#admesh)

<p>&nbsp;</p>

<!-- <<<SuperLU>>> -->
## <a name="SuperLU"></a> SuperLU

"*SuperLU is a general purpose library for the direct solution of large, sparse, nonsymmetric systems of linear equations on high
performance machines. The library is written in [C](#c) and is callable from either [C](#c) or [Fortran](#fortran). The library routines
will perform an LU decomposition with partial pivoting and triangular system solves through forward and back substitution. The LU
factorization routines can handle non-square matrices but the triangular solves are performed only for square matrices. The matrix columns
may be preordered (before factorization) either through library or user supplied routines. This preordering for sparsity is completely
separate from the factorization. Working precision iterative refinement subroutines are provided for improved backward stability. Routines
are also provided to equilibrate the system, estimate the condition number, calculate the relative backward error, and estimate error bounds
for the refined solutions.*"

### Web

[http://crd.lbl.gov/~xiaoye/SuperLU/](http://crd.lbl.gov/~xiaoye/SuperLU/)

### Documentation

[http://crd.lbl.gov/~xiaoye/SuperLU/superlu_ug.pdf](http://crd.lbl.gov/~xiaoye/SuperLU/superlu_ug.pdf)

<p>&nbsp;</p>

<!-- <<<TetGen>>> -->
## <a name="TetGen"></a> TetGen

"*TetGen generates tetrahedral meshes. The algorithms used in TetGen are of Delaunay type. For a three-dimensional domain, defined by its
boundary (such as a surface mesh), TetGen generates the boundary constrained (Delaunay) tetrahedralization, conforming Delaunay
tetrahedralization, and quality Delaunay mesh. For a three-dimensional point set, the Delaunay tetrahedralization and convex hull are
generated.*

*TetGen is written in [C++](#cxx). It can be compiled into an executable program or a library for integrating into other applications. All
major operating systems, e.g. Unix/Linux, MacOS, Windows, etc, are supported. *"

<p>&nbsp;</p>

<!-- <<<Triangle>>> -->
## <a name="Triangle"></a> Triangle

"*A Two-Dimensional Quality Mesh Generator and Delaunay Triangulator.*

*Triangle generates exact Delaunay triangulations, constrained Delaunay triangulations, conforming Delaunay triangulations, Voronoi diagrams,
and high-quality triangular meshes. The latter can be generated with no small or large angles, and are thus suitable for finite element
analysis.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/triangle)

### Exemples

[http://www.cs.cmu.edu/~quake/triangle.#demol](http://www.cs.cmu.edu/~quake/triangle.#demol)

<p>&nbsp;</p>

<!-- <<<trilinos>>> -->
## <a name="trilinos"></a> Trilinos

"*The Trilinos Project is an effort to develop and implement robust parallel algorithms using modern object-oriented software design, while
still leveraging the value of established numerical libraries such as [PETSc](#petsc), Aztec, the [BLAS](#blas) and [LAPACK](#lapack). It
emphasizes abstract interfaces for maximum flexibility of component interchanging, and provides a full-featured set of concrete classes that
implement all abstract interfaces.*"

### Web

[https://trilinos.org](https://trilinos.org)

<p>&nbsp;</p>

<!-- <<<TYPHON>>> -->
## <A NAME="TYPHON"></A> TYPHON

"*TYPHON is an open source project which aims to offer a development platform for many computational methods for gas dynamics. It is
structured as a multi-solver platform where it could be easily added a new solver. For now, it provides a finite volume solver for
compressible inviscid equations and a finite volume solver for heat transfer.*"

### Web

[http://typhon.sourceforge.net/](http://typhon.sourceforge.net/)

### Documentation

[http://typhon.sourceforge.net/#docl](http://typhon.sourceforge.net/#docl)

### Téléchargement

[http://typhon.sourceforge.net/#get_downloadl](http://typhon.sourceforge.net/#get_downloadl)

### Exemples

[http://typhon.sourceforge.net/#casel](http://typhon.sourceforge.net/#casel)

<p>&nbsp;</p>

<!-- <<<uBLAS>>> -->
## <a name="uBLAS"></a> uBLAS

"*uBLAS is a [C++](#cxx) template class library that provides [BLAS](#blas) level 1, 2, 3 functionality for dense, packed and sparse
matrices. The design and implementation unify mathematical notation via operator overloading and efficient code generation via expression
templates.*

*[…] uBLAS provides templated [C++](#cxx) classes for dense, unit and sparse vectors, dense, identity, triangular, banded, symmetric,
hermitian and sparse matrices. Views into vectors and matrices can be constructed via ranges or slices and adaptor classes. The library
covers the usual basic linear algebra operations on vectors and matrices: reductions like different norms, addition and subtraction of
vectors and matrices and multiplication with a scalar, inner and outer products of vectors, matrix vector and matrix matrix products and
triangular solver. The glue between containers, views and expression templated operations is a mostly STL conforming iterator interface.*"

### Téléchargement

"*The latest stable release of uBLAS is part of the [Boost](#boost) libraries.*"

<p>&nbsp;</p>

<!-- <<<UMFPACK>>> -->
## <A NAME="UMFPACK"></A> UMFPACK

"*UMFPACK is a set of routines for solving unsymmetric sparse linear systems, Ax=b, using the Unsymmetric MultiFrontal method. It uses
dynamic memory allocation, and has a symbolic preordering and analysis phase that also reports the upper bounds on the nonzeros in L and U,
flop count, and memory usage in the numeric phase. It can be used for real and complex matrices, rectangular and square, and both
non-singular and singular.*"

<p>&nbsp;</p>

<!-- <<<VisIt>>> -->
## <a name="VisIt"></a> VisIt

"*VisIt is a free interactive parallel visualization and graphical analysis tool for viewing scientific data on Unix and PC platforms. Users
can quickly generate visualizations from their data, animate them through time, manipulate them, and save the resulting images for
presentations. VisIt contains a rich set of visualization features so that you can view your data in a variety of ways. It can be used to
visualize scalar and vector fields defined on two- and three-dimensional (2D and 3D) structured and unstructured meshes. VisIt was designed
to handle very large data set sizes in the terascale range and yet can also handle small data sets in the kilobyte range. See the table
below for more details about the tool's features.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/visit)

<p>&nbsp;</p>

<!-- <<<Visualisation>>> -->
## <a name="Visualisation"></a> Visualisation

### Images

Quelques logiciels disponibles sur la plupart des machines pour créer des images à partir de vos résultats numériques :

<ul>
<li > [Gnuplot](#gnuplot) (Tutoriel : [http://www.duke.edu/~hpgavin/#gnuplotl](http://www.duke.edu/~hpgavin/#gnuplotl))
</li>
<li > Medit
</li>
<li > [Paraview](#paraview)
</li>
<li > [Scilab](#scilab)
</li>
</ul>

Pour retoucher une image une fois qu'elle a été enregistrée : [GIMP](http://www.gimp.org)

<ul>
<li > Une image JPEG de bonne qualité à partir d'une image EPS (fonctionne aussi à partir de PDF) :
</li>
</ul>
<pre >convert -density 200 -quality 100 &lt;image&gt;.eps &lt;image&gt;.jpg</pre>
<ul>
<li > Convertir toutes les images EPS du répertoire courant en JPEG :
</li>
</ul>
<pre >for i in *.eps;do echo $i;convert -density 200 -quality 100 $i $i.jpg;done</pre>

*Note pour Windows :* <strong>convert</strong>, ainsi que de nombreuses autres commandes utiles, est disponible en installant le logiciel
gratuit Cygwin ([http://www.cygwin.com](http://www.cygwin.com)).

### Films

#### Convertir une séquence d'images en film sous Linux
<ul>
<li > Une animation GIF (visible dans tout navigateur internet) à partir d'une séquence d'images EPS (NB: EPS n'est pas le seul format d'entrée possible. On peut aussi utiliser PPM, PNG, JPG, etc. Un fond transparent conduit à une superposition d'images) :
</li>
</ul>
<pre >convert -delay &lt;délai entre deux images en centièmes de secondes&gt; -loop 0 *.eps &lt;animation&gt;.gif</pre>
<ul>
<li > Un film MPEG à partir d'une séquence d'images JPEG nommées <strong>image1.jpg</strong>, <strong>image2.jpg</strong>, *etc* (more ffmpeg examples at [19 ffmpeg commands for all needs](http://www.catswhocode.com/blog/19-ffmpeg-commands-for-all-needs)):
</li>
</ul>
<pre >ffmpeg -i &lt;nom de l'image&gt;%d.jpg &lt;film&gt;.mpg</pre>
<ul>
<li > Un film MPEG-4 en 25 images/seconde à partir d'une séquence d'images&nbsp;.jpg&nbsp;: 
</li>
</ul>
<pre >mencoder mf://*.jpg -mf fps=25:type=jpg -ovc lavc -lavcopts vcodec=mpeg4 -oac copy -o &lt;film&gt;.avi</pre>

#### Convertir un film du format AVI au format MPEG
<pre >ffmpeg -i &lt;in&gt;.avi &lt;out&gt;.mpg</pre>

#### Extraire les images d'un film
<ul>
<li > Depuis une animation GIF :
</li>
</ul>
<pre >convert &lt;animation&gt;.gif &lt;images&gt;.jpg</pre>
<ul>
<li > Depuis tout format de film :
</li>
</ul>
<pre >mplayer -vo png &lt;film&gt;</pre>

#### Coller deux films
<pre >mencoder -ovc copy -oac copy &lt;film1&gt;.avi &lt;film2&gt;.avi -o &lt;film&gt;.avi</pre>

#### Convertir toutes les images EPS avec un fond transparent du répertoire courant en images PNG avec un fond blanc
<pre >for i in *.eps;do echo $i;convert -alpha Off -background white $i $i.png;done</pre>

### Autres logiciels de visualisation scientifique

* Sans programmation : [Geomview](#geomview), [MayaVi](#mayavi), Medit, [Povray](#povray), [Salomé](#salome), [VisIt](#visit), [xd3d](#xd3d)
* Programmation nécessaire : [Octave](#octave), [OpenDX](#opendx), OpenGL, [Plotmtv](#plotmtv), [rlabplus](#rlabplus), [Scilab](#scilab),
  [VTK](#vtk), [Yorick](#yorick)

<p>&nbsp;</p>

<!-- <<<VRML>>> -->
## <A NAME="VRML"></A> VRML

"*The Virtual Reality Modeling Language (VRML) is a file format for describing interactive 3D objects and worlds. VRML is designed to be
used on the Internet, intranets, and local client systems. VRML is also intended to be a universal interchange format for integrated 3D
graphics and multimedia. VRML may be used in a variety of application areas such as engineering and scientific visualization, multimedia
presentations, entertainment and educational titles, web pages, and shared virtual worlds.*"

### Documentation

[http://tecfa.unige.ch/guides/vrml/vrml97/spec/](http://tecfa.unige.ch/guides/vrml/vrml97/spec/)

### Logiciels capables d'écrire dans ce format

[ADMesh](#admesh), [Wings 3D](#wings_3d)

<p>&nbsp;</p>

<!-- <<<VTK>>> -->
## <A NAME="VTK"></A> VTK

"*The Visualization ToolKit (VTK) is an open source, freely available software system for 3D computer graphics, image processing, and
visualization used by thousands of researchers and developers around the world. VTK consists of a [C++](#cxx) class library, and several
interpreted interface layers including Tcl/Tk, Java, and [Python](#python). Professional support and products for VTK are provided by
Kitware, Inc. VTK supports a wide variety of visualization algorithms including scalar, vector, tensor, texture, and volumetric methods; and
advanced modeling techniques such as implicit modelling, polygon reduction, mesh smoothing, cutting, contouring, and Delaunay
triangulation. In addition, dozens of imaging algorithms have been directly integrated to allow the user to mix 2D imaging / 3D graphics
algorithms and data. The design and implementation of the library has been strongly influenced by object-oriented principles. VTK has been
installed and tested on nearly every Unix-based platform, PCs (Windows 98/ME/NT/2000/XP), and Mac OSX Jaguar or later.*"

[Fiche PLUME](http://www.projet-plume.org/fiche/vtk)

*Documentation:* [Online Tutorials](http://www.vtk.org/Wiki/VTK_Online_Tutorials),
[Documentation](http://www.vtk.org/Wiki/VTK_Documentation), [FAQ](http://www.vtk.org/Wiki/VTK_FAQ), [Wiki](http://www.vtk.org/Wiki/VTK)

*Autre:* See also [ParaView](#paraview)

<p>&nbsp;</p>

<!-- <<<Wings 3D>>> -->
## <a name="Wings 3D"></a> Wings 3D

"*Wings 3D is a subdivision modeler inspired by Nendo and Mirai from Izware.*

*It is possible to assign materials, vertex color, UV coordinates and textures, but there will be improvements in those features before Wings goes 1.0.*

*There is no support in Wings for doing animations.*"

### Web

[http://www.wings3d.com/](http://www.wings3d.com/)

### Documentation

[http://prdownloads.sourceforge.net/wings/wings3d_manual1.6.1.pdf?download](http://prdownloads.sourceforge.net/wings/wings3d_manual1.6.1.pdf?download)

### Format de données standard lus

[3D Studio (3DS)](#3d_studio)

### Format de données standard écrits

[3D Studio (3DS)](#3d_studio), [VRML](#vrml)

<p>&nbsp;</p>

<!-- <<<xd3d>>> -->
## <a name="xd3d"></a> xd3d

"*xd3d is a simple scientific visualization tool designed to be easy to learn. It can plot 2d and 3d meshes, with shadowing, contour plots,
vector fields, iso-contour (3d), as well as 3d surfaces z=f(x,y) defined by an algebraic expression or a cloud of points. It generates high
quality vector PostScript files for scientific publications and still or animated bitmap images. It includes the graph plotter xgraphic.*

*xd3d can be installed on any unix system using X windows: all the unix workstations, linux systems, Mac **OS** X, and Microsoft-Windows
computers with an X emulation like the freeware Cygwin/Xfree.*

*To compile and install xd3d and its related programs, you must have a [Fortran](#fortran) 77 and a [C](#c) compiler (like g77 and gcc). The
X11 library libX11.a and the include file X.h must be present on your computer.*

*To run xd3d you only need to have X. *"

### Web

[http://www.cmap.polytechnique.fr/~jouve/xd3d/index.php](http://www.cmap.polytechnique.fr/~jouve/xd3d/index.php)

### Format de données standard lus

Lit les fichiers au format NOPO (voir Modulef)

<p>&nbsp;</p>

<!-- <<<Y12M>>> -->
## <A NAME="Y12M"></A> Y12M

"*Y12MA solves sparse systems of linear algebraic equations by Gaussian elimination.  The subroutine is a “black box subroutine” designed to
solve efficiently problems which contain only one system with a single right hand side. The number of the input parameters is minimized. The
user must assign values only to NN, NN1, N, Z, A, SNR, RNR, IHA and B according to the rules described in Section 2.4 (see below).  It is
extremely easy to modify the subroutine to the cases: (a) a sequence of systems with the same matrix is to be solved (note that one system
with many right hand sides can be rewritten as a sequence of systems with the same matrix), (b) a sequence of systems whose matrices are
different but of the same structure is to be solved and © a sequence of systems whose matrices are of the same structure and some of them
are the same is to be solved.*"

### Web

[http://www.netlib.org/y12m/#indexl](http://www.netlib.org/y12m/#indexl)

### Documentation

[http://www.netlib.org/y12m/doc](http://www.netlib.org/y12m/doc)

<p>&nbsp;</p>

<!-- <<<Yorick>>> -->
## <a name="Yorick"></a> Yorick

"*Yorick is an interpreted programming language, designed for postprocessing or steering large scientific simulation codes. Smaller
scientific simulations or calculations, such as the flow past an airfoil or the motion of a drumhead, can be written as standalone yorick
programs. The language features a compact syntax for many common array operations, so it processes large arrays of numbers very
efficiently. Unlike most interpreters, which are several hundred times slower than compiled code for number crunching, yorick can approach
to within a factor of four or five of compiled speed for many common tasks. Superficially, yorick code resembles C code, but yorick
variables are never explicitly declared and have a dynamic scoping similar to many Lisp dialects. The yorick language is designed to be
typed interactively at a keyboard, as well as stored in files for later use. Yorick includes an interactive graphics package, and a binary
file package capable of translating to and from the raw numeric formats of all modern computers.*"

### Web

[http://www.maumae.net/yorick/doc/index.php](http://www.maumae.net/yorick/doc/index.php)

### Documentation

[http://www.maumae.net/yorick/doc/manual/yorick.php](http://www.maumae.net/yorick/doc/manual/yorick.php)

### Autres indications

"*[SpYorick](http://www.maumae.net/yorick/contrib/#spyorickl) is a plugin package for Yorick (&gt;= version 1.4) that, among other
interesting things, adds functions that operate both on dense and sparse matrices.*"

<p>&nbsp;</p>

<!-- <<<Z88>>> -->
## <a name="Z88"></a> Z88

"*Z88 is a fast, powerful and compact Finite Elements Analysis Program especially designed for PCs running the great LINUX, workstations and
large computers with UNIX and PCs with WindowsXP/95. Z88 features 20 finite element types covering plane stress, plate bending, axial
symmetric structures and spacial structures up to 20-node Serendipity hexahedrons. Z88 comes with a user-friendly interface, a powerful mesh
generator, a DXF-converter, two plot programs and, of course, two powerful solvers. Import of COSMOS files from Pro/ENGINEER and
Pro/MECHANICA is supported.*"

### Web

[http://z88.org/](http://z88.org/)

### Documentation

[http://www.z88.uni-bayreuth.de/download/z88mane.pdf](http://www.z88.uni-bayreuth.de/download/z88mane.pdf)

### Exemples

[http://www.z88.uni-bayreuth.de/#e_screenshotsl](http://www.z88.uni-bayreuth.de/#e_screenshotsl)

### Licence

"*The new version Z88 12.0 is GNU-**GPL** Freeware.*"

<!-- 
   - Local Variables:
   - mode:markdown
   - indent-tabs-mode:nil
   - mode:visual-line
   - ispell-local-dictionary:"british"
   - coding:utf-8
   - eval:(flyspell-mode)
   - eval:(outline-minor-mode)
   - End:
   -->
<!-- LocalWords: emacs
   -->
