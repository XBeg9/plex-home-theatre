find_all_sources(. cdrip_SRCS)
if(TARGET_WIN32)
  list(REMOVE_ITEM cdrip_SRCS ./EncoderFFmpeg.cpp)
  list(REMOVE_ITEM cdrip_SRCS ./EncoderFFmpeg.h)
endif(TARGET_WIN32)
add_sources(${cdrip_SRCS})
