`su postgres`

`pg_ctl -D $PGDATA start/restart`

```
SELECT * FROM pg_stat_activity WHERE datname='test';

SELECT pg_cancel_backend(pid);

SELECT pg_terminate_backend(pid)；

```
