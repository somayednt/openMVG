
add_executable(openMVG_sample_multiview_robustFundamental_guided robust_fundamental_guided.cpp)
target_link_libraries(openMVG_sample_multiview_robustFundamental_guided
  openMVG_image
  openMVG_multiview
  openMVG_features
  openMVG_matching
  ${STLPLUS_LIBRARY})
target_compile_definitions(openMVG_sample_multiview_robustFundamental_guided
  PRIVATE -DTHIS_SOURCE_DIR="${CMAKE_CURRENT_SOURCE_DIR}")
set_property(TARGET openMVG_sample_multiview_robustFundamental_guided PROPERTY FOLDER OpenMVG/Samples)
