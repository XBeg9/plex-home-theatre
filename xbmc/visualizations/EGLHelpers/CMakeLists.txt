find_all_sources(. EGL_HELPER_SRC)
add_library(egl_helper MODULE ${EGL_HELPER_SRC})
target_link_libraries(egl_helper ${CONFIG_LIBRARY_OPENGL})
install(TARGETS egl_helper DESTINATION ${RESOURCEPATH}/addons/visualization.eglhelper)
