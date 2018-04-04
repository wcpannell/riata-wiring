========
Controls
========

The car has had the majority of the factory wiring harness gutted.

.. _controls.dash-cluster:

Dash Cluster
============

As of right now, the gauge cluster is non-functional. The cluster wiring 
has been run to the ECU area in the passenger footwell.

.. _controls.center-console:

Center Console
==============

The switches are mounted to a carbon fiber plate located in the OE radio
location. All switches are currently wired high-side, directly driving
their loads. Switches should control the low side of a relay.

SW1
        Starter switch. This switch is already starting to get flakey.
        Switch should control the low side of a relay or be replaced with
        one capable of handling the starter solenoid load.

SW2
        Fuel Pump Relay. This relay is also controlled by the Megasquirt.
        This switch provides power, while the MS controls the ground.
        dumb. Remove this functionality and reassign this switch.

SW3
        Ignition Coils. This functionality should be combined with the
        injectors.

SW4
        Injectors. Combine with Ignition

SW5
        ECM. ECU should be turned on with master switch

SW6
        start enable. Should control relay that provides power to other
        relays on panel
