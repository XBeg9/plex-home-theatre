find_all_sources(. rendering_SRCS)
if(UNIX)
  find_all_sources(gles system_SRCS)
elseif(WIN32)
  find_all_sources(dx system_SRCS)
endif()
add_sources(${rendering_SRCS} ${system_SRCS})
