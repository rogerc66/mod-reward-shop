CU_SET_PATH("CMAKE_REWARD_SHOP_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/reward_shop.cpp")

AC_ADD_SCRIPT_LOADER("RewardShop"      "${CMAKE_CURRENT_LIST_DIR}/src/loader.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")

message("-- REWARD SHOP CONFIGURED --")
