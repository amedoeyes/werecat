project(
  'werecat',
  'cpp',
  version: '0.1.0',
  default_options: [
    'warning_level=3',
    'cpp_std=c++20',
    'prefer_static=true',
    'werror=true',
  ],
)

sources = files('./src/main.cpp')
include = include_directories('./include')
dependencies = [
  subproject('void_engine').get_variable('void_engine_dep'),
]

executable(
  'werecat',
  sources,
  include_directories: include,
  dependencies: dependencies,
)
