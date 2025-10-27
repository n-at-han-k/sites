# Change Alpha

A patch that allows for updating terminal transparency natively.

### Description

This patch is an extension to the [alpha](https://st.suckless.org/patches/alpha) patch,
which _must_ be applied prior.

### Notes

* This patch assumes that the alpha variable is a float, which was only updated in alpha
patch version 0.8.2 i.e., 0.8.2 is the minimum compatible version.
* Don't forget to append "config.h" to the end of the rm command under the clean rule in
Makefile if you are having issues running make install.

### Purpose

Later versions of the default alpha patch provide a method of changing window opacity via
the -A flag, however, with no method of querying the current alpha level, it is difficult
to write scripts which increment or decrement this value. It is typically possible to update
the opacity via your compositor, but not all compositors support this, and even if they do,
your setup is still less portable at the end of the day. The
[transset-df](https://aur.archlinux.org/packages/transset-df) package
located in the AUR is the closest I've come to changing opacity on a per-window basis,
however, it still requires writing a script and binding that script to some keys using a
keybinding manager of some sort. Not to mention, it's fatal flaw - you cannot increase the
opacity beyond the default value set with the alpha patch.

### Changelog
* **20251027-0.9.3**: Fixes a bug where increasing opacity from certain alpha values (e.g. 0.85 → 0.95 → 1.05) caused the terminal to become fully transparent instead of opaque.
The patch clamps alpha between 0.1 and 1.0 to prevent overflow and compositor misbehavior.

### Download

#### Patch: alpha (0.8.5) + changealpha

* [st-alpha-changealpha-0.1.diff](st-alpha-changealpha-20230519-b44f2ad.diff)
* [st-alpha-changealpha-20251027-0.9.3.diff](st-alpha-changealpha-20251027-0.9.3.diff)

#### Patch: changealpha

* [st-changealpha-0.1.diff](st-changealpha-20230519-b44f2ad.diff)
* [st-changealpha-20251027-0.9.3.diff](st-changealpha-20251027-0.9.3.diff)

### Author

* Neil Kingdom - <neil@neilkingdom.xyz>
* Abhishek Kumar - <abhiiishekparmar@gmail.com> (fixed transparency overflow issue)
