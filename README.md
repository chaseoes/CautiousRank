CautiousRank
============

Cautiously rank up players on your Bukkit server.

Commands:
/crank <rank as defined in the configuration> <player>
/crank reload

Permissions:
None. Defaults to OP's.

Default configuration:
confirm-message: '&aYou are now a(n) %rank%!'
# When a user successfully is ranked, send them the above message
# Please have the ability to use ChatColors in the message
ranks:
 newbie-to-member: #This is the "name" of the change, used as an argument in /crank
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
    - say %player% is now a Builder!