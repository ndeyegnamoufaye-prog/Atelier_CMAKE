file(GLOB LIB . *.c)
add_library(lib ${LIB})
add_test(NAME test_car COMMAND calculator car 5)
set_tests_properties(test_car PROPERTIES PASS_REGULAR_EXPRESSION "25")
