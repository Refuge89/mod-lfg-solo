CU_SET_PATH("CMAKE_LFG_SOLO_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/Lfg_Solo.cpp")

AC_ADD_SCRIPT_LOADER("SC_LFG_SoloMode" "${CMAKE_CURRENT_LIST_DIR}/src/loader.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")

message("-- Solo LFG CONFIGURED --")
