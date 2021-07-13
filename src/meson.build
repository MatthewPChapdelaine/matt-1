matt_1_sources = [
  'main.c',
  'matt_1-window.c',
]

matt_1_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk+-3.0', version: '>= 3.22'),
]

gnome = import('gnome')

matt_1_sources += gnome.compile_resources('matt_1-resources',
  'matt_1.gresource.xml',
  c_name: 'matt_1'
)

executable('matt-1', matt_1_sources,
  dependencies: matt_1_deps,
  install: true,
)
