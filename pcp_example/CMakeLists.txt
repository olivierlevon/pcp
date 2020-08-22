set(INC 
        ${CMAKE_SOURCE_DIR}/libpcp/src
        ${CMAKE_SOURCE_DIR}/libpcp/include)
		
include_directories(${INC})

add_executable(pcp-example pcp-example.c)

target_link_libraries(pcp-example ${LIB_LIBPCP} ${WIN_SOCK_LIBS})
