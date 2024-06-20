project (lua)

set (LUALIB_SOURCES lapi.c lcode.c lctype.c ldebug.c ldo.c ldump.c lfunc.c lgc.c llex.c lmem.c lobject.c lopcodes.c lparser.c lstate.c lstring.c ltable.c ltm.c lundump.c lvm.c lzio.c
 lauxlib.c lbaselib.c lcorolib.c ldblib.c liolib.c lmathlib.c loadlib.c loslib.c lstrlib.c ltablib.c lutf8lib.c linit.c)

set (LUAC_SOURCES luac.c)
set (LUA_SOURCES lua.c)

add_executable(luac ${LUAC_SOURCES} ${LUALIB_SOURCES})
add_executable(lua ${LUA_SOURCES} ${LUALIB_SOURCES})