# Copyright (c) Microsoft Corporation.
# Licensed under the MIT License.


set(SRC
    attribute.cpp
    instruction.cpp
    IR.cpp
)

add_library(nnfusion_ir STATIC ${SRC})
target_include_directories(nnfusion_ir SYSTEM PUBLIC
    ${GLOBAL_INCLUDE_PATH}
)
target_compile_options(nnfusion_ir PRIVATE "-fPIC")