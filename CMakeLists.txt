cmake_minimum_required(VERSION 2.8)

project(test)

add_executable(
	test
	src/main.cpp
	)

target_link_libraries(
	test
	curl
	)

install(TARGETS test
	RUNTIME DESTINATION /media/nas/dev/
	)