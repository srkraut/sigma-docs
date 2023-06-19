# Display Setting

Displays can be configured automatically from the CMS once they are connected and managed using Display Setting Profiles.

Each Display has a default Display Setting Profile which can be customised by an Administrator to suit required preferences.

New Display Setting Profiles can be created and assigned directly to a Display.

A list of available profiles can be viewed from Display Settings under the Display section of the main menu.

![Alt text](setting-img.png)

Each profile has a Name, Type and a flag indicating if it is the default or not. Default profiles are automatically assigned to Displays of the corresponding type.

## Editing Profiles

```
Use the row menu for the Profile you wish to view and click on Edit.
Use the Edit Profile form to adjust available settings.
```

Each setting is explained under each form field for each of the tabs.

```
Using the row menu click on Copy to make another version of a Profile.
Make adjustments as needed to quickly and simply create new Profiles.
```

## Notable Settings

Collect Interval Located on the General tab, use the drop-down menu select how often you would like the Player to check for new content. This means that once a Player has communicated with the CMS, it will check again for any changes by the time set here.

```
Scenario:

A Player has a collect interval set for 24 hours, it will check for any changes,
action pending changes and then wait for the next 24-hour collection.
If a change is made between this period of time, the Player will not
be aware of it until it is time to check again.
```

If a Display Profile for a Player is changed, the Player will only be aware of the change after it has connected according to its prior connection interval.

```
Scenario:

A Player with a collect interval set for 24 hours made a check at 12 pm,
it will not check again until 12 pm the following day for any changes that
have been made. Once the 24 hour interval has passed, it will update the new
changes and from this point will collect changes based on the new Profile.
```

XMR is configured by default for Sigma DS in the Cloud customers which allows for changes to be communicated immediately to the Player, regardless of the Collection Interval set. This means that fast and dynamic modifications can be made to your Display, without the need to modify a Display Profile.

For non-cloud customers the CMS can be configured to talk to an XMR instance if player actions are required, please contact your Administrator.

We recommend setting no lower than 5 minutes for production, generally a 15-30 minute setting would be sensible.

## Enable Stats Reporting

Tick/untick the box to enable/disable the collection of statistics for Proof of Play Reports for all Displays that use the selected Display Profile.

If enabled set the required level of collection for Proof of Play statistics to be applied to all Layouts / Media and Widget items using the Aggregation level drop down.

![Alt text](setting-img2.png)

- Individual - statistics are collected when specified by default.
- Hourly - statistics will be collected hourly by default.
- Daily - statistics will be collected daily by default.
- From v2.3.9 if the geolocation of the Display is known, enable the checkbox to record the location against each proof of play record. Users with mobile Displays can turn this setting on if desired.

Players aggregate ‘completed records’ only, with collection made at the end of the Widgets duration so if a Widget has a duration of 3 hours, the stat will be recorded once the Widget has expired.

## Expire Modified Layouts

Located on the Advanced tab, use this checkbox to tell Sigma DS to immediately expire and cut playback of a Layout when a Player receives an update from the CMS.
