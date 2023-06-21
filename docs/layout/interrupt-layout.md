# Interrupt Layouts

When a Layout is scheduled as an Interrupt Layout, Sigma-DS will work out how it should be played between Layouts in the ‘usual schedule’ using the Share of Voice time or percentage entered on the event.

```
This can be useful if you have, for example, Announcements that
 need to be shown for a particular amount of time within the usual schedule.
```

### Create an Interrupt Layout

Interrupt Layouts are created in exactly the same way as all other Layouts.

## Scheduling

Interrupt Layouts are selected as an Event type when Scheduling an Event.

Once selected, complete the form fields:

![Alt text](interrupy1.png)

## Share of Voice

Enter the amount of time the Layout should be shown in seconds per hour or as a percentage (0 - 100%) of the events duration (the difference between the from date and the to date) that the Interrupt Layout should occupy the usual schedule.

```
Please note: If your ‘main’ Layout has a long duration,
 the Interrupt Layout may show in a block in order
  to satisfy the SoV criteria entered!
```
