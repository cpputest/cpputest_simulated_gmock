
ACLOCAL_AMFLAGS = -I m4

CPPUTEST_TESTS = CppUTestSimulatedGMockTests

lib_LIBRARIES = lib/libCppUSimulatedGMock.a
check_PROGRAMS = $(CPPUTEST_TESTS)

TESTS = $(check_PROGRAMS)

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = cpputest_simulated_gmock.pc

EXTRA_DIST = \
	cpputest_simulated_gmock.pc.in \
	$(ALL_FILES_IN_GIT)

lib_libCppUSimulatedGMock_a_CPPFLAGS = $(AM_CPPFLAGS) $(CPPUTEST_GTEST_CPPFLAGS) 

lib_libCppUSimulatedGMock_a_SOURCES = \
	src/GTest.cpp 

CppUTestSimulatedGMockTests_SOURCES = \
    tests/TestGTest.cpp 

