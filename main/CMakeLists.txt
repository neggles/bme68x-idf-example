# uncomment one of 3 below to choose your desired mode
set(project_srcs "src/forced_mode.c")
#set(project_srcs "src/parallel_mode.c")
#set(project_srcs "src/sequential_mode.c")

idf_component_register(
    SRCS ${project_srcs}
    REQUIRES "i2cdev" "bme68x-idf"
    INCLUDE_DIRS "."
)
