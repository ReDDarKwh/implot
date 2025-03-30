# Define an ImGui target that fits our use case
add_library(implot STATIC
  implot.h
  implot_internal.h
  implot.cpp
  implot_items.cpp
)

target_include_directories(implot PUBLIC .)
target_link_libraries(implot PUBLIC imgui)
