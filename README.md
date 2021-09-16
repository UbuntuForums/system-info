## Ubuntu Forums system-info Script
The Ubuntu Forums "system-info" script queries the users computer and prepares a report, so that Ubuntu Forums Community Members can see what they are recommending solutions for. This is the Stable Repository, whereas the TEST Repository is at: https://github.com/Mafoelffen1/system-info
## Details

- Creates the file `system-info.txt` at the base of the user's home directory.
- Masks all sensitive info, like IP addresses, MAC addresses, Full FQDN and Serial numbers, automatically in a meaningful way.
- The script displays the report results within the 'less' utility to review the results, one screen at a time. To navigate from there, press the space bar, left, right, up, down, page up or page down keys to navigate. If in a graphical terminal session, you can also use mouse navigation. Press the "q" key to exit "less" and continue. It will print the final report and offer to upload to pastebin site.
- Offers to post the results to the Ubuntu `pastebinit` provider if that program is installed, and a sufficiently reliable internet connection is available. This is the easiest way to share the sanitized results with the Ubuntu Community for support. After succssful upload to the pastebin, it will both display and log the URL of the uploaded report (`~/system-info-link.log`), for you to copy and paste in your post on the Ubuntu Forums.
- Future versions may have an option to create the archive `system-info.tar.gz` if the report exceeds 19.5 kB in size.


## Run from CLI

You can either run it from the command line (Console or Terminal Session) with these commands:

    wget -N -t 5 -T 10 https://github.com/UbuntuForums/system-info/raw/main/system-info && \
    chmod +x system-info && \
    ./system-info

This will download the script, make it executable, and run it, all in a row.

## Run from GUI

Or, from a GUI Desktop, this way:

1. [Download][1] the script
2. In Nautilus or other file broswer, From File Properties, Permissions, Make it executable.
3. Run it from your file browser or a Run dialog from kdialog

[1]: https://github.com/UbuntuForums/system-info/raw/main/system-info

