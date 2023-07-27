xdg_user_dirs_gtk_sources = [
  'main.c',
  'xdg-user-dirs-gtk-application.c',
  'xdg-user-dirs-gtk-window.c',
]

xdg_user_dirs_gtk_deps = [
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.2'),
]

xdg_user_dirs_gtk_sources += gnome.compile_resources('xdg-user-dirs-gtk-resources',
  'xdg-user-dirs-gtk.gresource.xml',
  c_name: 'xdg_user_dirs_gtk'
)

executable('xdg-user-dirs-gtk', xdg_user_dirs_gtk_sources,
  dependencies: xdg_user_dirs_gtk_deps,
       install: true,
)
