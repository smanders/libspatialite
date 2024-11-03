set(exe spatialite)
add_executable(${exe} shell.c)
target_link_libraries(${exe} PRIVATE libspatialite xpro::libiconv)
target_compile_definitions(${exe} PRIVATE SQLITE_OMIT_TRACE)
