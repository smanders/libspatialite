foreach(demo demo1 demo2 demo3 demo4 demo5)
  add_executable(${demo} ${demo}.c)
  target_link_libraries(${demo} PRIVATE libspatialite)
endforeach()
