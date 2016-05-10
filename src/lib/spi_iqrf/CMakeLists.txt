set(SPIDEV_SRC_FILES
	spi_iqrf.c
)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_library(spi_iqrf
                SHARED
		${SPIDEV_SRC_FILES}
)

install(TARGETS spi_iqrf DESTINATION ${CMAKE_INSTALL_PREFIX}/lib)
