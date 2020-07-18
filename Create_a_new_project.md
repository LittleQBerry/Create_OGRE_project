# Create a new OGRE project

## Basic
 * OGRE SDK
 * visual studio 2017

## Create
1. Add OGRE SDK path to the "enviroment path" of your PC. Name: OGRE_HOME, Value: sdk folder path. 
2. create an empty project in VS. You can import a cpp file from Sample/Tutotials (in the source code folder).
3. Change to "Release" mode.
4. Click the "property" of the project.
5. Debugging->command: \$(OGRE_HOME)\Bin\\$(ProjectName).exe
6. Working Directory: \$(OGRE_HOME)\$\Bin
7. C/C++ -> General -> Additional Include Diretories:   
    \$(OGRE_HOME)\include\OGRE  
    \$(OGRE_HOME)\Samples\Common\include  
    \$(OGRE_HOME)\include\OGRE\Overlay  
    \$(OGRE_HOME)\include\OGRE\Bites  
    \$(OGRE_HOME)\include\OGRE\RTShaderSystem   

8. Linker -> General -> Additional Library Diretories:   
     \$(OGRE_HOME)\lib
9. Liner ->input -> Additional Dependencies:  
    OgreMain.lib  
    OgreOverlay.lib  
    OgreBites.lib  
    OgreRTShaderSystem.lib  


10. Build Events->Post-Build Event -> Command Line :  
   copy "\$(OutDir)\ \$(TargetFileName)" "\$(OGRE_HOME)\Bin" 

11. General->Character Set:  
    Use multi-byte Character set
12. Now you can run this cpp file.
     