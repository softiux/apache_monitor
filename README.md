# apache_monitor
#!/bin/bash

while true; do
        now=$(date)
        cmd=$(netstat -antp | grep :80 | wc -l)

        echo $now "-" $cmd
        sleep 30
done
