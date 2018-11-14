CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

project(dummylib)
#SET(PROJECT_NAME dummylib)
#SET(PROJECT_DESCRIPTION "C++ library with non-empty class for testing in other projects ( link/binds)")
#SET(PROJECT_URL "")

# Disable -Werror on Unix for now.
#SET(CXX_DISABLE_WERROR True)
#SET(CMAKE_VERBOSE_MAKEFILE True)
#SET(CMAKE_CXX_FLAGS "-std=c++0x")


# ----------------------------------------------------
# --- INSTALL PATH -----------------------------------
# ----------------------------------------------------
IF(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
  SET(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR} CACHE PATH "" FORCE)
ENDIF(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)

# ----------------------------------------------------
# --- DEPENDANCIES -----------------------------------
# ----------------------------------------------------


# ----------------------------------------------------
# --- INCLUDE ----------------------------------------
# ----------------------------------------------------

include_directories("include")

# Declare Headers -- Add here the header files
SET(${PROJECT_NAME}_HEADERS
  # dummy-module.hpp
)


ADD_SUBDIRECTORY(src)
#ADD_SUBDIRECTORY(tests)

