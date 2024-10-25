#
# Copyright 2024 NXP
#
# SPDX-License-Identifier: MIT
#

if (CONFIG_MCUX_COMPONENT_middleware.freertos.corehttp)
    mcux_add_source(
        SOURCES source/core_http_client.c source/include/core_http_client.h source/include/core_http_client_private.h source/include/core_http_config_defaults.h source/interface/transport_interface.h
    )
    mcux_add_include(
        INCLUDES source/include source/interface
    )
endif()
