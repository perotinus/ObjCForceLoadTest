# ObjCForceLoadTest

Test project for the behavior of -ObjC vs -force_load as linker flags.

Has a few application targets:

- Linking_ObjCFlag – links using ```-ObjC```
- Linking_ForceLoadFlag – links using ```-force_load```

Each target contains one library with only Objective C code, and one 
with C++ code as well. Run ```nm``` on the resultant binaries to see 
which symbols are linked into each binary.
