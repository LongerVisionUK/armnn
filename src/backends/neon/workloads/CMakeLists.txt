#
# Copyright © 2017 Arm Ltd. All rights reserved.
# SPDX-License-Identifier: MIT
#

list(APPEND armnnNeonBackendWorkloads_sources
    NeonActivationWorkload.cpp
    NeonActivationWorkload.hpp
    NeonAdditionWorkload.cpp
    NeonAdditionWorkload.hpp
    NeonBatchNormalizationWorkload.cpp
    NeonBatchNormalizationWorkload.hpp
    NeonConcatWorkload.cpp
    NeonConcatWorkload.hpp
    NeonConstantWorkload.cpp
    NeonConstantWorkload.hpp
    NeonConvertFp16ToFp32Workload.cpp
    NeonConvertFp16ToFp32Workload.hpp
    NeonConvertFp32ToFp16Workload.cpp
    NeonConvertFp32ToFp16Workload.hpp
    NeonConvolution2dWorkload.cpp
    NeonConvolution2dWorkload.hpp
    NeonDepthwiseConvolutionWorkload.cpp
    NeonDepthwiseConvolutionWorkload.hpp
    NeonFloorFloatWorkload.cpp
    NeonFloorFloatWorkload.hpp
    NeonFullyConnectedWorkload.cpp
    NeonFullyConnectedWorkload.hpp
    NeonGreaterWorkload.cpp
    NeonGreaterWorkload.hpp
    NeonL2NormalizationFloatWorkload.cpp
    NeonL2NormalizationFloatWorkload.hpp
    NeonLstmFloatWorkload.cpp
    NeonLstmFloatWorkload.hpp
    NeonMaximumWorkload.cpp
    NeonMaximumWorkload.hpp
    NeonMeanWorkload.cpp
    NeonMeanWorkload.hpp
    NeonMinimumWorkload.cpp
    NeonMinimumWorkload.hpp
    NeonMultiplicationWorkload.cpp
    NeonMultiplicationWorkload.hpp
    NeonNormalizationFloatWorkload.cpp
    NeonNormalizationFloatWorkload.hpp
    NeonPadWorkload.cpp
    NeonPadWorkload.hpp
    NeonPermuteWorkload.cpp
    NeonPermuteWorkload.hpp
    NeonPooling2dWorkload.cpp
    NeonPooling2dWorkload.hpp
    NeonReshapeWorkload.cpp
    NeonReshapeWorkload.hpp
    NeonResizeBilinearWorkload.cpp
    NeonResizeBilinearWorkload.hpp
    NeonSoftmaxBaseWorkload.cpp
    NeonSoftmaxBaseWorkload.hpp
    NeonSoftmaxFloatWorkload.cpp
    NeonSoftmaxFloatWorkload.hpp
    NeonSoftmaxUint8Workload.cpp
    NeonSoftmaxUint8Workload.hpp
    NeonSplitterWorkload.cpp
    NeonSplitterWorkload.hpp
    NeonSubtractionWorkload.cpp
    NeonSubtractionWorkload.hpp
    NeonWorkloads.hpp
    NeonWorkloadUtils.hpp
)

add_library(armnnNeonBackendWorkloads OBJECT ${armnnNeonBackendWorkloads_sources})
target_include_directories(armnnNeonBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/armnn)
target_include_directories(armnnNeonBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/armnnUtils)
target_include_directories(armnnNeonBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/backends)
