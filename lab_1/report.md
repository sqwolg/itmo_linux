## Переменные окружения

Файл: `/etc/default/test.test`

```conf
VAR1=Hello
VAR2=world
```

## Лог работы

Файл: `/var/log/test.test.log`

```text
Fri Mar 20 04:37:28 PM UTC 2026: Hello world!
Fri Mar 20 04:37:33 PM UTC 2026: Hello world!
Fri Mar 20 04:37:38 PM UTC 2026: Hello world!
Fri Mar 20 04:37:43 PM UTC 2026: Hello world!
Fri Mar 20 04:37:48 PM UTC 2026: Hello world!
Fri Mar 20 04:37:53 PM UTC 2026: Hello world!
Fri Mar 20 04:37:58 PM UTC 2026: Hello world!
Fri Mar 20 04:38:03 PM UTC 2026: Hello world!
Fri Mar 20 04:38:08 PM UTC 2026: Hello world!
Fri Mar 20 04:38:13 PM UTC 2026: Hello world!
Fri Mar 20 04:38:18 PM UTC 2026: Hello world!
Fri Mar 20 04:38:23 PM UTC 2026: Hello world!
Fri Mar 20 04:38:28 PM UTC 2026: Hello world!
Fri Mar 20 04:38:33 PM UTC 2026: Hello world!
Fri Mar 20 04:38:38 PM UTC 2026: Hello world!
```

## Статус сервиса systemd

Команда: `systemctl status test.test.service`

```text
● test.test.service - Test test
     Loaded: loaded (/etc/systemd/system/test.test.service; disabled; preset: enabled)
     Active: active (running) since Fri 2026-03-20 16:34:13 UTC; 4min 30s ago
   Main PID: 191289 (test.test)
      Tasks: 2 (limit: 19105)
     Memory: 580.0K (peak: 1.1M)
        CPU: 170ms
     CGroup: /system.slice/test.test.service
             ├─191289 /bin/bash /root/itmo/linux/1_lab/test.test
             └─192190 sleep 5

Mar 20 16:34:13 ochernykh-personal-vm-01.spb.yadro.com systemd[1]: Started test.test.service - Test test.
```

