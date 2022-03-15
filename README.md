# jetson_nano_tricks

#Managing fan control on NVIDIA jetson nano

##Manual activity, has to be done after every boot:

ON: `sudo sh -c ‘echo 255 > /sys/devices/pwm-fan/target_pwm’`
OFF: `sudo sh -c ‘echo 0 > /sys/devices/pwm-fan/target_pwm’`

##Another way of setting fan PWM, but this too doesn't persist across boots.

[Using Jetson Clocks](https://arcanesciencelab.wordpress.com/2019/12/23/jason-nano-and-using-jason_clocks-for-the-fan/)



##The best way for automatic fan speed control that persists across boots:

[](https://github.com/Pyrestone/jetson-fan-ctl)


###Follow these steps:
```
git clone https://github.com/Pyrestone/jetson-fan-ctl.git
cd jetson-fan-ctl
./install.sh
```

And that's it!!



**Changes in config can be done by simply updating the config.json file:**

`sudo gedit /etc/automagic-fan/config.json`

`sudo service automagic-fan restart`

