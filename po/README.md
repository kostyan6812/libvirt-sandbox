Libvirt-Sandbox Message Translation
================================

Libvirt-Sandbox translatable messages are maintained using the GNU Gettext tools
and file formats, in combination with the Zanata web service.

Source repository
=================

The libvirt-sandbox GIT repository stores the master "libvirt-sandbox.pot"
file and full "po" files for translations. The master "libvirt-sandbox.pot"
file can be re-generated using

   make libvirt-sandbox.pot

The full po files can have their source locations and msgids updated using

   make update-po

Normally these updates are only done when either refreshing translations from
Zanata, or when creating a new release.

Zanata web service
==================

The translation of libvirt-sandbox messages has been outsourced to the Fedora
translation team using the Zanata web service:

  https://fedora.zanata.org/project/view/libvirt-sandbox

As such, changes to translations will generally NOT be accepted as patches
directly to libvirt-sandbox GIT. Any changes made to "$LANG.mini.po" files in
libvirt-sandbox GIT will be overwritten and lost the next time content is
imported from Zanata.

The master "libvirt-sandbox.pot" file is periodically pushed to Zanata to
provide the translation team with content changes. New translated text is
then periodically pulled down from Zanata to update the po files.
