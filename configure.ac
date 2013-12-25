
AC_PREREQ([2.68])
AC_INIT([CppUTestSimulatedGMock], [0.2], [https://github.com/cpputest/cpputest_simulated_gmock])
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([src/GTest.cpp])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([cpputest_simulated_gmock.pc])
AC_CONFIG_MACRO_DIR([m4])

AC_CANONICAL_HOST
AM_MAINTAINER_MODE([enable])

AC_PROG_CC
AC_PROG_CPP
AC_PROG_CXX
AC_PROG_LN_S
AC_PROG_MAKE_SET
AM_PROG_CC_C_O
AM_SILENT_RULES

AC_CHECK_HEADERS([stddef.h stdint.h stdlib.h string.h sys/time.h unistd.h])

AC_C_INLINE
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_INT8_T
AC_TYPE_PID_T
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_TYPE_UINT8_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_CHECK_FUNCS([gettimeofday memset strstr])

# Assume CppUTest is at /usr/local/include. This needs to be fixed to make the checking proper
CPPUTEST_GTEST_CPPFLAGS="${CPPUTEST_GTEST_CPPFLAGS} -I /usr/local/include"

CPPUTEST_GTEST_CPPFLAGS="${CPPUTEST_GTEST_CPPFLAGS} -I ${srcdir}/include"
AC_SUBST([CPPUTEST_GTEST_CPPFLAGS])

LT_INIT
AC_CONFIG_FILES([Makefile])
AC_OUTPUT

echo \
"----------------------------------------------------------------

${PACKAGE_NAME} Version ${PACKAGE_VERSION}

Current compiler options:
   CC:                                  ${CC}
   CXX:                                 ${CXX}
   LD:                                  ${LD}
      
----------------------------------------------------------------"
