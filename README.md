CautiousRank
============

Cautiously rank up players on your Bukkit server.

Commands:
/crank <rank as defined in the configuration> <player>
/crank reload

Permissions:
None. Defaults to OP's.

Default configuration:
```confirm-message: '&aYou are now a(n) %rank%!'
ranks:
 newbie-to-member:
    from: newbie
    to: member
    commands:
    - money give %player% 10
    # This command is ran from the Console
  from-noob-to-builder:
    from: newbie
    to: builder
    commands:
    - give %player% 1 64
    - say %player% is now a Builder!```