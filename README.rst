x201fancontrol: Control the fan when the ME stops sending temperature reports
=============================================================================

If you've used `me_cleaner <https://github.com/corna/me_cleaner>`__,
disabled AMT in the BIOS or the ME has just inexplicably died,
you will no longer get readings from the internal temperature sensor.

The following simple bash daemon uses the CPU coretemp readings to control ``/proc/acpi/ibm/fan``.

Installation
------------

Check out the repository and run ``x201fancontrol --install``,
which sets up a systemd service for wherever you checked it out.
