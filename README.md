# Privacy policy site (source)

This folder is the source of the public privacy policy at
https://enpotatoes.github.io/palermo-privacy/ . The main repository stays
private, so these files are copied into the separate public repository
`palermo-privacy` (GitHub Pages, branch main, folder / (root)).

Files: index.html (English), el/index.html (Greek), join/index.html (the page invite
links and room QR codes open: it shows the code and opens the app), download/index.html
(the page the app's "Share the game" QR code opens, Greek and English; its Download button
is the one place the APK address lives, see tool/release_apk.md), style.css, .nojekyll.

The APK itself is not in this folder: it is attached to a GitHub Release of
palermo-privacy as palermo.apk, so
https://github.com/EnPotatoes/palermo-privacy/releases/latest/download/palermo.apk
always gets the newest one. When the game is on Google Play, change the download
page's button (and AppLinks.download in the app if the QR code should open the store).

Before publishing, replace every enpotatoes@gmail.com, Philippos Mesina / Philippos Mesina
and Larnaca / Λάρνακα in both pages. Update both pages, and the date at the top,
before any version that collects new data is released.

To publish a change (Git Bash, from this repository's folder):

    cp -r docs/site/. ../palermo-privacy/
    cd ../palermo-privacy && git add -A && git commit -m "Update privacy policy" && git push
