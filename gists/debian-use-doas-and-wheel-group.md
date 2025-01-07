# Use doas and Resurrect the Wheel Group

Quick tip for Debian/Devuan users: replace sudo with doas and resurrect the wheel group:

    # apt-get install -y doas
    # sed '15 s/^# //' /etc/pam.d/su
    # addgroup --system wheel
    # echo "permit :wheel" > /etc/doas.conf

Or, just switch to Ragnarok, it uses them by default.
