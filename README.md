# Etienne

user@user-HP-ProBook-4720s:~$ youtube-dl https://ondemand-cf-vrt.akamaized.net/content/vod/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1_drm_dec3bc59-b122-4f1e-a143-3df98c008eed.ism/.mpd
[generic] .mpd: Requesting header
WARNING: Falling back on generic information extractor.
[generic] .mpd: Downloading webpage
[generic] .mpd: Extracting information
ERROR: No video formats found; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
user@user-HP-ProBook-4720s:~$ https://yt-dl.org/update
bash: https://yt-dl.org/update: No such file or directory
user@user-HP-ProBook-4720s:~$ sudo youtube-dl -U
[sudo] password for user:     
Usage: youtube-dl [OPTIONS] URL [URL...]

youtube-dl: error: youtube-dl's self-update mechanism is disabled on Debian.
Please update youtube-dl using apt(8).
See https://packages.debian.org/sid/youtube-dl for the latest packaged version.

user@user-HP-ProBook-4720s:~$ youtube-dl https://ondemand-cf-vrt.akamaized.net/content/vod/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1_drm_dec3bc59-b122-4f1e-a143-3df98c008eed.ism/.mpd
[generic] .mpd: Requesting header
WARNING: Falling back on generic information extractor.
[generic] .mpd: Downloading webpage
[generic] .mpd: Extracting information
ERROR: No video formats found; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
user@user-HP-ProBook-4720s:~$ sudo youtube-dl --verbose
[debug] System config: []
[debug] User config: []
[debug] Custom config: []
[debug] Command-line args: ['--verbose']
[debug] Encodings: locale UTF-8, fs utf-8, out UTF-8, pref UTF-8
[debug] youtube-dl version 2018.03.14
[debug] Python version 3.6.8 (CPython) - Linux-4.15.0-66-generic-x86_64-with-LinuxMint-19.2-tina
[debug] exe versions: ffmpeg 3.4.6-0ubuntu0.18.04.1, ffprobe 3.4.6-0ubuntu0.18.04.1
[debug] Proxy map: {}
Usage: youtube-dl [OPTIONS] URL [URL...]

youtube-dl: error: You must provide at least one URL.
Type youtube-dl --help to see a list of all options.
user@user-HP-ProBook-4720s:~$ sudo pip install -U youtube-dl
sudo: pip: command not found
user@user-HP-ProBook-4720s:~$ sudo apt-get remove -y youtube-dl
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following packages were automatically installed and are no longer required:
  flac lame libhttp-parser2.7.1 libjs-jquery libsox-fmt-alsa libsox-fmt-base libsox3 libuv1 nodejs python3-click python3-colorama
  python3-flask python3-itsdangerous python3-jinja2 python3-protobuf python3-pychromecast python3-werkzeug python3-zeroconf sox
  vorbis-tools
Use 'sudo apt autoremove' to remove them.
The following packages will be REMOVED:
  youtube-dl
0 upgraded, 0 newly installed, 1 to remove and 37 not upgraded.
After this operation, 5.271 kB disk space will be freed.
(Reading database ... 351705 files and directories currently installed.)
Removing youtube-dl (2018.03.14-1ubuntu18.04.1) ...
Processing triggers for man-db (2.8.3-2ubuntu0.1) ...
user@user-HP-ProBook-4720s:~$ sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl
--2019-11-23 08:41:33--  https://yt-dl.org/downloads/latest/youtube-dl
Resolving yt-dl.org (yt-dl.org)... 95.143.172.170, 2001:1a50:11:0:5f:8f:acaa:177
Connecting to yt-dl.org (yt-dl.org)|95.143.172.170|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://yt-dl.org/downloads/2019.11.22/youtube-dl [following]
--2019-11-23 08:41:34--  https://yt-dl.org/downloads/2019.11.22/youtube-dl
Connecting to yt-dl.org (yt-dl.org)|95.143.172.170|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://github.com/ytdl-org/youtube-dl/releases/download/2019.11.22/youtube-dl [following]
--2019-11-23 08:41:35--  https://github.com/ytdl-org/youtube-dl/releases/download/2019.11.22/youtube-dl
Resolving github.com (github.com)... 140.82.118.3
Connecting to github.com (github.com)|140.82.118.3|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://github-production-release-asset-2e65be.s3.amazonaws.com/1039520/03cccc80-0cc7-11ea-8b15-4ecf4e3f0bb7?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191123%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191123T074136Z&X-Amz-Expires=300&X-Amz-Signature=eb2ea59a6508b72df801a21a87a4a85ef65a51a0c901fe3e9ac7d1ee7d4120a4&X-Amz-SignedHeaders=host&actor_id=0&response-content-disposition=attachment%3B%20filename%3Dyoutube-dl&response-content-type=application%2Foctet-stream [following]
--2019-11-23 08:41:36--  https://github-production-release-asset-2e65be.s3.amazonaws.com/1039520/03cccc80-0cc7-11ea-8b15-4ecf4e3f0bb7?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191123%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191123T074136Z&X-Amz-Expires=300&X-Amz-Signature=eb2ea59a6508b72df801a21a87a4a85ef65a51a0c901fe3e9ac7d1ee7d4120a4&X-Amz-SignedHeaders=host&actor_id=0&response-content-disposition=attachment%3B%20filename%3Dyoutube-dl&response-content-type=application%2Foctet-stream
Resolving github-production-release-asset-2e65be.s3.amazonaws.com (github-production-release-asset-2e65be.s3.amazonaws.com)... 52.216.81.16
Connecting to github-production-release-asset-2e65be.s3.amazonaws.com (github-production-release-asset-2e65be.s3.amazonaws.com)|52.216.81.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1748039 (1,7M) [application/octet-stream]
Saving to: ‘/usr/local/bin/youtube-dl’

/usr/local/bin/youtube-dl        100%[==========================================================>]   1,67M  61,7KB/s    in 25s     

2019-11-23 08:42:02 (68,2 KB/s) - ‘/usr/local/bin/youtube-dl’ saved [1748039/1748039]

user@user-HP-ProBook-4720s:~$ sudo chmod a+rx /usr/local/bin/youtube-dl
user@user-HP-ProBook-4720s:~$ hash -r
user@user-HP-ProBook-4720s:~$ sudo youtube-dl -U
youtube-dl is up-to-date (2019.11.22)
user@user-HP-ProBook-4720s:~$ sudo youtube-dl https://ondemand-cf-vrt.akamaized.net/content/vod/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1/vid-aefd90e8-8d39-43d5-8666-17854ef47f33-CDN_1_drm_dec3bc59-b122-4f1e-a143-3df98c008eed.ism/.mpd
[generic] .mpd: Requesting header
WARNING: Falling back on generic information extractor.
[generic] .mpd: Downloading webpage
[generic] .mpd: Extracting information
ERROR: No video formats found; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; type  youtube-dl -U  to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
user@user-HP-ProBook-4720s:~$ 
