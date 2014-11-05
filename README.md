Currently, there are 2 themes.
Both support [Stake House](https://github.com/hidden-id/stakehouse#readme).

* `stakehouse-default` is exactly like the default theme, but also lets you
make stake claims.
* `blavatsky` is a minimal design contributed by [Madame Blavatsky](https://idoru.pl/u/blavatsky).


### Installing themes
#### If needed, upgrade your HiddenID server

* Pull the latest [hidden-id](https://github.com/hidden-id/hidden-id).
* `git submodule update --init` (because there *was* a submodule update).

#### Per identity:

* Backup you id folder (better safe than sorry).
* Run `python2 hidden-id.py /path/to/my_id_folder` to create the `sstore/templates/` and `sstore/static/` subfolders.
* You can kill it (you don't need to wait until it establishes the hidden service).
* Copy the files from `themes/<the theme you want>/templates/` to `my_id_folder/sstore/templates/`.
* Edit `my_id_folder/sstore/profile.json` according to `themes/<the theme you want>/README.md`.

#### Creating a "fresh" identity:

Instead of the first 2 steps above, just run `python2 hidden-id.py /path/to/new_id_folder_to_create`.
