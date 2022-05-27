project('chinook-sqlite', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])

sqlite3_proj = subproject('sqlite3')
sqlite3_dep = sqlite3_proj.get_variable('sqlite3_dep')

exe = executable('chinook_sqlite', 'src/chinook_sqlite.c', dependencies : sqlite3_dep,
  install : true)

test('basic', exe)
