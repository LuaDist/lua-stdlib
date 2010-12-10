# Copyright (C) 2007-2010 LuaDist.
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(lua-stdlib NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# stdlib modules
INSTALL (DIRECTORY modules/ DESTINATION ${INSTALL_LMOD})
INSTALL(FILES AUTHORS README DESTINATION ${INSTALL_DATA})
INSTALL(DIRECTORY utils/ DESTINATION ${INSTALL_FOO})
