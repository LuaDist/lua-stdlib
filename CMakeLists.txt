# Copyright (C) 2007-2010 LuaDist.
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( lua-stdlib NONE )
cmake_minimum_required ( VERSION 2.6 )
include ( dist.cmake )

# collect sources
file ( GLOB ${LUA_FILES} modules/*.lua )

# Install lua modules using glob
install ( FILES ${LUA_FILES} DESTINATION ${INSTALL_LMOD} )

# Macro install rest
install_data ( AUTHORS README )
install_foo ( utils/ )
