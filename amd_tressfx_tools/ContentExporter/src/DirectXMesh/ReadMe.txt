DIRECTX MESH LIBRARY (DirectXMesh)
------------------------------------

Copyright (c) Microsoft Corporation. All rights reserved.

October 30, 2015

This package contains DirectXMesh, a shared source library for performing various geometry
content processing operations including generating normals and tangent frames, triangle
adjacency computations, and vertex cache optimization.

The source is written for Visual Studio 2012, 2013, or 2015. It is recommended that you
make use of the Windows 8.1 SDK and Windows 7 Service Pack 1 or later.

These components are designed to work without requiring any content from the DirectX SDK. For details,
see "Where is the DirectX SDK?" <http://msdn.microsoft.com/en-us/library/ee663275.aspx>.

DirectXMesh\
    This contains the DirectXMesh library.

    Note that the majority of the header files here are intended for internal implementation
    of the library only (DirectXMeshP.h and scoped.h). Only DirectXMesh.h is meant as a
    'public' header for the library.

Utilities\
    This contains helper code related to mesh processing that is not general enough to be
    part of the DirectXMesh library.

         WaveFrontReader.h - Contains a simple C++ class for reading mesh data from a WaveFront OBJ file.

Meshconvert\
    This DirectXMesh sample is an implementation of the "meshconvert" command-line texture utility
    from the DirectX SDK utilizing DirectXMesh rather than D3DX.

    Note this tool does not support legacy .X files, but can export CMO, SDKMESH, and VBO files.

All content and source code for this package are subject to the terms of the MIT License.
<http://opensource.org/licenses/MIT>.

Documentation is available at <https://github.com/Microsoft/DirectXMesh/wiki>.

For the latest version of DirectXMesh, bug reports, etc. please visit the project site.

http://go.microsoft.com/fwlink/?LinkID=324981


---------------
RELEASE HISTORY
---------------

October 30, 2015
    Minor code cleanup

August 18, 2015
    Xbox One platform updates

July 29, 2015
    Updated for VS 2015 and Windows 10 SDK RTM
    Retired VS 2010 projects
    WaveFrontReader: updated utility to minimize debug output

July 8, 2015
    Minor SAL fix and project cleanup

March 27, 2015
    Added projects for Windows apps Technical Preview
    Fixed attributes usage for OptimizeFacesEx
    meshconvert: fix when importing from .vbo
    Minor code cleanup

November 14, 2014
    meshconvert: sample improvements and fixes
    Added workarounds for potential compiler bug when using VB reader/writer

October 28, 2014
    meshconvert command-line sample
    Added VBReader/VBWriter::GetElement method
    Added more ComputeTangentFrame overloads
    Explicit calling-convention annotation for public headers
    Windows phone 8.1 platform support
    Minor code and project cleanup

June 27, 2014
    Original release