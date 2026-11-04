<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="brave_dark.png">
    <source media="(prefers-color-scheme: light)" srcset="brave_light.png">
    <img alt="Brave Logo" src="brave_light.png">
  </picture>
</p>

another-brave-overlay-testing
=============================

![⚙️ Update](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fupdate.json&style=flat-square&logo=github&label=%E2%9A%99%EF%B8%8F%20Update)
![🧪 CI (stable)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-browser.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Status%20(stable))
![🧪 CI (beta)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-browser-beta.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Status%20(beta))
![🧪 CI (nightly)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-browser-nightly.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Status%20(nightly))
![🧪 Origin (stable)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-origin.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Origin%20(stable))
![🧪 Origin (beta)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-origin-beta.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Origin%20(beta))
![🧪 Origin (nightly)](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fbrave-origin-nightly.json&style=flat-square&logo=github&label=%F0%9F%A7%AA%20Origin%20(nightly))
![🔍 Divergence](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Ffalbrechtskirchinger%2Fanother-brave-overlay-testing%2Fbadges%2Fdivergence.json&style=flat-square&logo=github&label=%F0%9F%94%8D%20Divergence)
This Gentoo overlay provides automatically generated ebuilds for the [Brave browser](https://brave.com/), a privacy-focused, open-source web browser based on Chromium, and [Brave Origin](https://brave.com/origin/), a streamlined version of Brave Browser. The ebuilds are based on several official Gentoo ebuilds for other Chromium-based browsers, which are routinely checked for divergence, and adapted to deliver the stable, beta, and nightly versions of Brave Browser and Brave Origin via the following ebuilds:

- `www-client/brave-browser` (stable)
- `www-client/brave-browser-beta` (beta)
- `www-client/brave-browser-nightly` (nightly)
- `www-client/brave-origin` (stable)
- `www-client/brave-origin-beta` (beta)
- `www-client/brave-origin-nightly` (nightly)

These ebuilds install pre-built binary versions.

Installation
------------

To install Brave from this overlay, follow these steps:

1. Add the overlay:

    ```sh
    eselect repository enable another-brave-overlay
    ```

2. Sync the overlay to download the ebuilds:

    ```sh
    emaint sync -r another-brave-overlay
    ```

3. Install Brave from the desired release channel using `emerge`. Available packages are:

    - `www-client/brave-browser` (stable)
    - `www-client/brave-browser-beta` (beta)
    - `www-client/brave-browser-nightly` (nightly)

    For example, to install the stable version:

    ```sh
    emerge -av www-client/brave-browser
    ```

Issues and Contributions
------------------------

If you encounter any problems or have suggestions for improvement, please open an issue on the GitHub repository: https://github.com/falbrechtskirchinger/another-brave-overlay.


**Please do not submit pull requests at this time.**

The underlying automation is being completely rewritten. As of May 2026, I don't have a firm timeline, but I aim to have the rewrite finished before the end of the year.

License
-------

Ebuilds in this overlay are licensed under the GNU General Public License v2.0 (GPL-2).

See the `LICENSE.GPL-2` file in the repository for full details.

**Trademark Notice**: All Brave logos, marks, and designations are trademarks or registered trademarks of Brave Software, Inc.
