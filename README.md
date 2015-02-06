This is a backport of the fixed zpool provider for pre Puppet 4.0 systems.

This adds a new provider called 'hotfixzpool' that allows you to use the new provider.

To implement this, install this module in your basemodulepath, and add this resource default to your site.pp for each environment:

Zpool {
  provider => 'hotfixzpool',
}
