set(PROJECT_NAME spi_iqrf)

set(SPIDEV_SRC_FILES
	spi_iqrf.c
)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_library(${PROJECT_NAME}
                STATIC
		${SPIDEV_SRC_FILES}
)

install(TARGETS ${PROJECT_NAME} DESTINATION ${CMAKE_INSTALL_PREFIX}/lib)
