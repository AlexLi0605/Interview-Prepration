add_executable(
  unit_tests
  array_test.cpp
  linked_list_test.cpp
)

target_link_libraries(
  unit_tests
  gtest_main
  array
  linked_list
)

add_test(
  NAME
    unit
  COMMAND
    ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_BINDIR}/unit_tests
)
