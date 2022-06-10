gnomeban_sources = [
  'main.vala',
  'window.vala',
  'application.vala',
]

gnomeban_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

gnomeban_sources += gnome.compile_resources('gnomeban-resources',
  'gnomeban.gresource.xml',
  c_name: 'gnomeban'
)

executable('gnomeban', gnomeban_sources,
  vala_args: '--target-glib=2.50',  dependencies: gnomeban_deps,
  install: true,
)
