set(MODULE_NAME BRUTEFORCE)

set(${MODULE_NAME}_SOURCES
    binary_double.cpp
    binary_float.cpp
    binary_i_double.cpp
    binary_i_float.cpp
    binary_operator_double.cpp
    binary_operator_float.cpp
    binary_two_results_i_double.cpp
    binary_two_results_i_float.cpp
    common.cpp
    common.h
    function_list.cpp
    function_list.h
    i_unary_double.cpp
    i_unary_float.cpp
    macro_binary_double.cpp
    macro_binary_float.cpp
    macro_unary_double.cpp
    macro_unary_float.cpp
    mad_double.cpp
    mad_float.cpp
    main.cpp
    reference_math.cpp
    reference_math.h
    sleep.cpp
    sleep.h
    ternary_double.cpp
    ternary_float.cpp
    test_functions.h
    unary_double.cpp
    unary_float.cpp
    unary_two_results_double.cpp
    unary_two_results_float.cpp
    unary_two_results_i_double.cpp
    unary_two_results_i_float.cpp
    unary_u_double.cpp
    unary_u_float.cpp
    utility.cpp
    utility.h
)

# math_brute_force compiles cleanly with -Wall (except for a few remaining
# warnings), but other tests not (yet); so enable -Wall locally.
set_gnulike_module_compile_flags("-Wall -Wno-strict-aliasing -Wno-unknown-pragmas")

include(../CMakeCommon.txt)
