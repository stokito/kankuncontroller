# kankuncontroller
scripts from my kankun hacking

```
Usage:  script.py -a on

    make sure to vi this script and set the IP to that of your target

    arguments:
        required:
        -a, --action    <action name> what action to perform, e.g., -a heart
        actions: on, off, heart, check, brmode, totalTimer, checkTimer, setTimer, unsetTimer, wifiConfig

        optional:
        -v              verbose output

        actions that take additional arguments:

            unsetTimer
                script.py -a unsetTimer --num 3

                --num           a number, this is an argument required for checkTimer and unsetTimer actions


            setTimer
                script.py -a setTimer --start-time "`date +%y-%m-%d-%T`" --stop-time "2015-02-10-11:22:22" --enabled y [...] --repeatstr "1,2,3"

                --start-time    <date +%y-%m-%d-%T> this is a date-string
                --stop-time     ditto
                --enabled       <y|n> timer enabled?
                --on-enabled    <y|n> on-time enabled?
                --off-enabled   <y|n> off-time enabled?
                --repeatstr     <1,2,4,5,6,7>, setTimer argument, repeat on which days?


            wifiConfig
                script.py -a wifiConfig --ssid Linksys --key "P@ssw0rd!"

                --ssid          <string>, the ssid of the network to join the device to
                --key           <string>, the key for the network to join the device to
                --initial-password <string>, the password to set for the device (default is "noPASSWORD")
                --device-name   <string>, the name to give the device (this doesnt always take and changes with the wind)
```

See [Kankun KK-SP3: Complite Guide](https://github.com/yurt-page/Kankun_KK-SP3) for other details.

