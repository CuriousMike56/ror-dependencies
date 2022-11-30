ExternalProject_Add(
        fmt 
        URL https://github.com/fmtlib/fmt/releases/download/8.0.1/fmt-8.0.1.zip
        URL_MD5 21039fb4c826c81829a6c4d600e2b11c
        CMAKE_ARGS
        -DFMT_TEST=OFF
        -DCMAKE_INSTALL_PREFIX=${DEPENDENCIES_OUTPUT_DIR}
        -DCMAKE_BUILD_TYPE=${CMAKE_BUILD_TYPE}
        -DCMAKE_CXX_FLAGS=${CMAKE_CXX_FLAGS}
        -DCMAKE_C_COMPILER=${CMAKE_C_COMPILER}
        -DCMAKE_CXX_COMPILER=${CMAKE_CXX_COMPILER}
)