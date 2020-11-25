# XBASE
PostgreSQL As Oracle  --  Make PostgreSQL compatible with Oracle


# Projects XBASE depends on
* postgresql
* orafce

# Implemented features including
* a switch configuration parameter "sql_dialect" to use postgresql
  or oracle sql dialect, which can be set during session, but I
  strongly recommend that you just change sql dialect during postgresql
  startup, since if you change sql dialect during session the current
  implementation will create or drop orafce extension, that will touch
  other session(s) like any other extensions.



