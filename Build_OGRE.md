# Build OGRE from source

## Basic
* Cmake 3.16.4 or other
* Visual Studio 2017
* [OGRE 1.12.5](https://www.ogre3d.org/download/sdk/sdk-ogre)

## BUILD by Cmake

1. Open your Cmake.
2. Set "Where is the source code" path is the OGRE source code path.
3. Set "Where to build the bianries" path is the SDK save path.
4. Click "Configure" to choose the right generator, And the click the "Finish".
5. Waiting untill there are lists showing in the main window. Find the name "OGRE_DEPENDENCIES_DIR", and set the value is the "dependencies" folder path under the SDK save path. 
![show](https://github.com/LittleQBerry/Create_OGRE_project/blob/master/20200718141701.png)
6. Attention that the 1.12.5 version does not contain the 'imgui', so you also need unckeck it in the lists. 
7. Attention again that 1.12.5 only has the Realse version so you also set the build version is "Release" .
8. After that, click "configure" and "generate". Finally, there is a "OGRE.sln" in the output folder.

## BUILD by VS
1. After getting the "OGRE.sln",click it in the Visual studio.
2. Choose "Release".
3. First build the "BUILD_ALL".
4. Then build the "INSTALL". If there is no error, you will successfully build the OGRE.
5. Finally, you can run "ogre_sample_browser" to see the results. 


Attention that,you can also download the MSVC SDK which is suitable for your VS.
