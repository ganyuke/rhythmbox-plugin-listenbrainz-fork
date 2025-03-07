## Listenbrainz plugin fork
This is a personal fork of the bundled [Listenbrainz plugin](https://gitlab.gnome.org/GNOME/rhythmbox/-/tree/master/plugins/listenbrainz) in GNOME [Rhythmbox](https://gitlab.gnome.org/GNOME/rhythmbox), modified to support scrobbling to custom, Listenbrainz-compatible servers (e.g. [Maloja](https://github.com/krateng/maloja)).

## How to use
1. Clone the repository to `~/.local/share/rhythmbox/plugins/` as a directory named `listenbrainz`.
2. Copy `com.github.ganyuke.rhythmbox-plugin-listenbrainz-fork.gschema.xml` to `/usr/share/glib-2.0/schemas/`.
3. Run `sudo glib-compile-schemas /usr/share/glib-2.0/schemas/`.
4. Open Rhythmbox and configure "ListenBrainz Fork" preferences as follows:
    - **User token** is the MusicBrainz user token.
    - **Server URL** is an URL to a ListenBrainz API endpoint.
      - It only accepts HTTPS URLs and requires a slash at the end to work.
      - For example: `maloja.example.org/apis/listenbrainz/`.

Note that this fork will replace the ListenBrainz plugin entry in Rhythmbox. I don't know why.
