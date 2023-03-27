test_hpp = custom_target(
    'server.hpp',
    capture: true,
    command: [
        sdbuspp,
        '-r', meson.source_root() / '10_dbus_fan/interfaceAdded_yaml_object_interface_fan_ctrl',
        'interface',
        'server-header',
        'xyz.openbmc_project.fanctrl',
    ],
    input: '../test.interface.yaml',
    install: true,
    install_dir: get_option('includedir') / 'xyz/openbmc_project/test',
    output: 'server.hpp',
)

test_cpp = custom_target(
    'server.cpp',
    capture: true,
    command: [
        sdbuspp,
        '-r', meson.source_root() / '10_dbus_fan/interfaceAdded_yaml_object_interface_fan_ctrl',
        'interface',
        'server-cpp',
        'xyz.openbmc_project.fanctrl',
    ],
    input: '../test.interface.yaml',
    output: 'server.cpp',
)
