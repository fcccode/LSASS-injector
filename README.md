# LSASS-injector
 

[ANNOUNCEMENT]
Some anti-cheat program now strip handle permission of lsass.
So to use this injector actaully , you need some modifications.

[HOW IT WORKS]
LSASS has a handle that has read and write permission to processes that need network connection.
This injector uses that handle which noramlly is prohibited in normal process.

This solution contains two project.
One is manual map injector, and the other is manual map injector that runs in lsass.

The DedicatedInjector.exe map The LsassInjector.dll.
Then the LsassInjector map our dll to target process.
After the injection is done, DedicatedInjector.exe erase every traces that it left in lsass.exe.
