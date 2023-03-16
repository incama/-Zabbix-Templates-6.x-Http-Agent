#### Cron Schedule
Tested cron schedule:
```
0 */6 * * * /root/f2b/get_iptables_data.sh 2>&1
5 */6 * * * /usr/bin/python3 /root/f2b/main.py 2>&1
```
This way main.py runs five minutes later then the iptables query. Making sure it handles the newly generated
file in time. Adjust the timing setting when using very long lists of banned ip's