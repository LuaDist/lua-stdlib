# Copyright (C) 2007-2010 LuaDist.
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( lua-stdlib NONE )
cmake_minimum_required ( VERSION 2.6 )
include ( dist.cmake )

set ( VERSION 26 )  #~2DO: get from dist.info
configure_file ( src/std.lua.in ${CMAKE_CURRENT_BINARY_DIR}/std.lua )

install_lua_module ( base src/base.lua )
install_lua_module ( bin src/bin.lua )
install_lua_module ( debug_ext src/debug_ext.lua )
install_lua_module ( debug_init src/debug_init.lua )
install_lua_module ( fstable src/fstable.lua )
install_lua_module ( getopt src/getopt.lua )
install_lua_module ( io_ext src/io_ext.lua )
install_lua_module ( lcs src/lcs.lua )
install_lua_module ( list src/list.lua )
install_lua_module ( math_ext src/math_ext.lua )
install_lua_module ( mbox src/mbox.lua )
install_lua_module ( modules src/modules.lua )
install_lua_module ( object src/object.lua )
install_lua_module ( package_ext src/package_ext.lua )
install_lua_module ( parser src/parser.lua )
install_lua_module ( set src/set.lua )
install_lua_module ( strbuf src/strbuf.lua )
install_lua_module ( strict src/strict.lua )
install_lua_module ( string_ext src/string_ext.lua )
install_lua_module ( table_ext src/table_ext.lua )
install_lua_module ( tree src/tree.lua )
install_lua_module ( xml src/xml.lua )
install_lua_module ( std ${CMAKE_CURRENT_BINARY_DIR}/std.lua )

install_data ( AUTHORS README )  # ignore: INSTALL
