set(PROJECT_NAME sysfs_gpio)

set(SYSFS_GPIO_SRC_FILES
	sysfs_gpio.c
)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_library(${PROJECT_NAME}
		STATIC
		${SYSFS_GPIO_SRC_FILES}
)

install(TARGETS ${PROJECT_NAME} DESTINATION ${CMAKE_INSTALL_PREFIX}/lib)
