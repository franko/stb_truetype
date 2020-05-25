project('stb_truetype', 'c', version: '1.24', default_options : ['c_std=gnu89'])

cc = meson.get_compiler('c')
libm = cc.find_library('m', required : false)

stb_truetype_lib = static_library('stb_truetype', 'stb_truetype.c', install: true)

install_headers('stb_truetype.h')

pkg = import('pkgconfig')

pkg.generate(stb_truetype_lib,
    filebase : 'stb_truetype',
    name : 'stb_truetype',
    libraries : libm,
    description : 'truetype stb library for C/C++',
    url : 'https://github.com/nothings/stb',
)
