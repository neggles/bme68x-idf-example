idf_component_register(
    SRCS "i2cdev.c"
    PRIV_REQUIRES "driver" "freertos"
    INCLUDE_DIRS "."
)
