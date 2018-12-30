cmake_minimum_required (VERSION 3.7)

include (ExternalProject)

ExternalProject_Add (
  ncurses
  SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}
  CONFIGURE_COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/configure --prefix=<INSTALL_DIR>
  BUILD_COMMAND ${MAKE}
)
