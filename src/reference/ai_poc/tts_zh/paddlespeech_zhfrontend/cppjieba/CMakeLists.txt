PROJECT(CPPJIEBA)

CMAKE_MINIMUM_REQUIRED (VERSION 2.6)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/deps/limonp/include
  ${PROJECT_SOURCE_DIR}/include)
#
#if (CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
#    set (CMAKE_INSTALL_PREFIX "/usr/local/cppjieba" CACHE PATH "default install path" FORCE )
#endif()
#
#ADD_DEFINITIONS(-O3 -Wall -g)
#IF(APPLE) # mac os
#    ADD_DEFINITIONS(-std=c++0x)
#endif()

# cmake .. -DENC=GBK
# IF (DEFINED ENC)
#     ADD_DEFINITIONS(-DCPPJIEBA_${ENC})
# ENDIF()

ADD_SUBDIRECTORY(deps)

#ADD_SUBDIRECTORY(test)

#ENABLE_TESTING()
#ADD_TEST(NAME ./test/test.run COMMAND ./test/test.run)
#ADD_TEST(NAME ./load_test COMMAND ./load_test)
#ADD_TEST(NAME ./demo COMMAND ./demo)
