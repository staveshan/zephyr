# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.13.1)
set(QEMU_EXTRA_FLAGS -s)

find_package(Zephyr HINTS $ENV{ZEPHYR_BASE})
project(onoff-app)

target_sources(app PRIVATE src/main.c)
