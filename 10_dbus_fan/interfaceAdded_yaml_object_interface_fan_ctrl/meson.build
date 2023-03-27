# use to create a test interface
subdir('xyz/openbmc_project/test')

executable(
  'fan_ctrl_speed',
  'main_server.cpp',
  test_cpp,
  test_hpp,
  dependencies: [
    sdbusplus_dep,
    phosphor_logging_dep,
  ],
  implicit_include_directories: true,
  install: true
)

