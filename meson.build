project('chinook-sqlite', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])

sqlite3_dep = dependency('sqlite3', fallback : ['sqlite3', 'sqlite3_dep'])

exe = executable('chinook_sqlite', 'src/chinook_sqlite.c', dependencies : sqlite3
  install : true)

test('basic', exe)
