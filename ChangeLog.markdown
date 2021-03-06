# 0.5.0

 * Fixed listing of castles cloned using `homesick clone <github-user>/<github-repo>` (issue 3)
 * Added `homesick pull <CASTLE>` for updating castles (thanks Jorge Dias!)
 * Added a very basic `homesick generate <CASTLE>`

# 0.4.1

 * Improved error message when a castle's home dir doesn't exist

# 0.4.0

 * `homesick clone` can now take a path to a directory on the filesystem, which will be symlinked into place
 * `homesick clone` now tries to `git submodule init` and `git submodule update` if git submodules are defined for a cloned repo
 * Fixed missing dependency on thor and others
 * Use HOME environment variable for where to store files, instead of assuming ~

# 0.3.0

 * Renamed 'link' to 'symlink'
 * Fixed conflict resolution when symlink destination exists and is a normal file

# 0.2.0

 * Better support for recognizing git urls (thanks jacobat!)
	 * if it looks like a github user/repo, do that
	 * otherwise hand off to git clone
 * Listing now displays in color, and show git remote
 * Support pretend, force, and quiet modes

# 0.1.1

 * Fixed trying to link against castles that don't exist
 * Fixed linking, which tries to exclude . and .. from the list of files to
 link (thanks Martinos!)

# 0.1.0

 * Initial release
