project('libbacktrace', 'c',
  version: '1.0',
  meson_version: '>= 0.56.0',
  license: 'BSD',
)

mod = import('unstable_external_project')

p = mod.add_project('configure',
  configure_options: [
    '--prefix=@PREFIX@',
    '--libdir=@PREFIX@/@LIBDIR@',
  ],
)

libbacktrace_dep = p.dependency('backtrace')
