set(tidy_SRC
  access.c
  attrs.c
  istack.c
  parser.c
  tags.c
  entities.c
  lexer.c
  pprint.c
  clean.c
  localize.c
  config.c
  alloc.c
  attrask.c
  attrdict.c
  attrget.c
  buffio.c
  fileio.c
  streamio.c
  tagask.c
  tmbstr.c
  utf8.c
  tidylib.c
  mappedio.c
  )
add_library(tidy ${tidy_SRC})

install(TARGETS tidy
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib
  ARCHIVE DESTINATION lib
  )


# set(tidy_HDRS
#   access.h
#   attrdict.h
#   attrs.h
#   clean.h
#   config.h
#   entities.h
#   fileio.h
#   forward.h
#   lexer.h
#   mappedio.h
#   message.h
#   parser.h
#   pprint.h
#   streamio.h
#   tags.h
#   tmbstr.h
#   utf8.h
#   tidy-int.h
#   version.h)

# INSTALL(FILES ${tidy_HDRS}
#   DESTINATION include
#   )
