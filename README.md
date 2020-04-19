# FFmpeg Command
- Collect useful FFmpeg Command

## Command

### enable nvidia codec  (use nvidia GPU Accelerator)
```
# Clone nvidia codec header project
git clone https://github.com/FFmpeg/nv-codec-headers
cd nv-codec-headers
git checkout n9.1.23.1

# Not use prefix path
Makefile
make
make install 

# If you need prefix path, use below command instead it
export PREFIX_PATH=/type/your/prefix/dir/path
sed -i 's@/usr/local@'"$PREFIX_PATH"'@' Makefile
make
make install
```

### Export Library Package (use `apt-get install`)
- My 'ffmpeg dependency package list' is below.
- Since the cleanup has not been completed yet, I put up the entire list first.
- If you want to install all of the list below in one run, see [here](https://github.com/ej31/ffmpeg-command/deps.sh).

```
# Choose package if you need

apt-get -yqq update

apt-get install -yq --no-install-recommends autoconf
apt-get install -yq --no-install-recommends automake
apt-get install -yq --no-install-recommends make
apt-get install -yq --no-install-recommends build-essential
apt-get install -yq --no-install-recommends curl
apt-get install -yq --no-install-recommends nasm
apt-get install -yq --no-install-recommends bzip2
apt-get install -yq --no-install-recommends g++
apt-get install -yq --no-install-recommends gcc
apt-get install -yq --no-install-recommends perl
apt-get install -yq --no-install-recommends git
apt-get install -yq --no-install-recommends gperf
apt-get install -yq --no-install-recommends fonts-dejavu-core
apt-get install -yq --no-install-recommends fontconfig-config
apt-get install -yq --no-install-recommends libtool
apt-get install -yq --no-install-recommends pkg-config
apt-get install -yq --no-install-recommends texinfo
apt-get install -yq --no-install-recommends yasm
apt-get install -yq --no-install-recommends libass-dev
apt-get install -yq --no-install-recommends checkinstall
apt-get install -yq --no-install-recommends zlib1g-dev
apt-get install -yq --no-install-recommends libxvidcore-dev
apt-get install -yq --no-install-recommends libfontconfig1
apt-get install -yq --no-install-recommends cmake
apt-get install -yq --no-install-recommends libasound2
apt-get install -yq --no-install-recommends libasound2-data
apt-get install -yq --no-install-recommends libasound2-plugins
apt-get install -yq --no-install-recommends fontconfig
apt-get install -yq --no-install-recommends libaacs0
apt-get install -yq --no-install-recommends gfortran
apt-get install -yq --no-install-recommends libhdf5-dev
apt-get install -yq --no-install-recommends libfreetype6-dev
apt-get install -yq --no-install-recommends liblapack-dev
apt-get install -yq --no-install-recommends python
apt-get install -yq --no-install-recommends python-setuptools
apt-get install -yq --no-install-recommends libasyncns0
apt-get install -yq --no-install-recommends libbdplus0
apt-get install -yq --no-install-recommends libbs2b0
apt-get install -yq --no-install-recommends libcaca0
apt-get install -yq --no-install-recommends libcairo2
apt-get install -yq --no-install-recommends libcroco3
apt-get install -yq --no-install-recommends libcrystalhd3
apt-get install -yq --no-install-recommends libdatrie1
apt-get install -yq --no-install-recommends libdrm-amdgpu1
apt-get install -yq --no-install-recommends libdrm-intel1
apt-get install -yq --no-install-recommends libexpat1-dev
apt-get install -yq --no-install-recommends libdrm-nouveau2
apt-get install -yq --no-install-recommends libdrm-radeon1
apt-get install -yq --no-install-recommends libfftw3-double3
apt-get install -yq --no-install-recommends libflac8
apt-get install -yq --no-install-recommends libflite1
apt-get install -yq --no-install-recommends libgbm1
apt-get install -yq --no-install-recommends libgme0
apt-get install -yq --no-install-recommends libgomp1
apt-get install -yq --no-install-recommends libgraphite2-3
apt-get install -yq --no-install-recommends libgsm1
apt-get install -yq --no-install-recommends libharfbuzz0b
apt-get install -yq --no-install-recommends libjbig0
apt-get install -yq --no-install-recommends libjpeg-turbo8
apt-get install -yq --no-install-recommends libjpeg8
apt-get install -yq --no-install-recommends libmp3lame0
apt-get install -yq --no-install-recommends libogg0
apt-get install -yq --no-install-recommends libopenal-dev
apt-get install -yq --no-install-recommends libopenjp2-7-dev
apt-get install -yq --no-install-recommends libwebp-dev
apt-get install -yq --no-install-recommends libzvbi-dev
apt-get install -yq --no-install-recommends libopus0
apt-get install -yq --no-install-recommends libpango-1.0-0
apt-get install -yq --no-install-recommends libpangocairo-1.0-0
apt-get install -yq --no-install-recommends libpangoft2-1.0-0
apt-get install -yq --no-install-recommends libpciaccess0
apt-get install -yq --no-install-recommends libpgm-5.2-0
apt-get install -yq --no-install-recommends libpixman-1-0
apt-get install -yq --no-install-recommends libpulse0
apt-get install -yq --no-install-recommends libdrm-dev
apt-get install -yq --no-install-recommends libgme-dev
apt-get install -yq --no-install-recommends libgsm1-dev
apt-get install -yq --no-install-recommends libmp3lame-dev
apt-get install -yq --no-install-recommends libopus-dev
apt-get install -yq --no-install-recommends libpulse-dev
apt-get install -yq --no-install-recommends librubberband-dev
apt-get install -yq --no-install-recommends libshine-dev
apt-get install -yq --no-install-recommends libsnappy-dev
apt-get install -yq --no-install-recommends libssh-dev
apt-get install -yq --no-install-recommends libtheora-dev
apt-get install -yq --no-install-recommends libtwolame-dev
apt-get install -yq --no-install-recommends libvpx-dev
apt-get install -yq --no-install-recommends libwavpack-dev
apt-get install -yq --no-install-recommends libraw1394-11
apt-get install -yq --no-install-recommends librsvg2-2
apt-get install -yq --no-install-recommends libsamplerate0
apt-get install -yq --no-install-recommends libsdl2-dev
apt-get install -yq --no-install-recommends libsensors4
apt-get install -yq --no-install-recommends libshine3
apt-get install -yq --no-install-recommends libsndfile1
apt-get install -yq --no-install-recommends libsoxr0
apt-get install -yq --no-install-recommends libspeex1
apt-get install -yq --no-install-recommends libssh-gcrypt-4
apt-get install -yq --no-install-recommends libthai-data
apt-get install -yq --no-install-recommends libthai0
apt-get install -yq --no-install-recommends libtheora0
apt-get install -yq --no-install-recommends libtiff5
apt-get install -yq --no-install-recommends libtwolame0
apt-get install -yq --no-install-recommends libvdpau1
apt-get install -yq --no-install-recommends libvorbis0a
apt-get install -yq --no-install-recommends libvorbisenc2
apt-get install -yq --no-install-recommends libvorbisfile3
apt-get install -yq --no-install-recommends libwavpack1
apt-get install -yq --no-install-recommends libwayland-client0
apt-get install -yq --no-install-recommends libwayland-cursor0
apt-get install -yq --no-install-recommends libwayland-server0
apt-get install -yq --no-install-recommends libx11-xcb1
apt-get install -yq --no-install-recommends libxcb-dri2-0
apt-get install -yq --no-install-recommends libxcb-dri3-0
apt-get install -yq --no-install-recommends libxcb-present0
apt-get install -yq --no-install-recommends libxcb-render0
apt-get install -yq --no-install-recommends libxcb-shape0
apt-get install -yq --no-install-recommends libxcb-shm0
apt-get install -yq --no-install-recommends libxcb-sync1
apt-get install -yq --no-install-recommends libxcb-xfixes0
apt-get install -yq --no-install-recommends libxcursor1
apt-get install -yq --no-install-recommends libxdamage1
apt-get install -yq --no-install-recommends libxfixes3
apt-get install -yq --no-install-recommends libxi6
apt-get install -yq --no-install-recommends libxinerama1
apt-get install -yq --no-install-recommends libxkbcommon0
apt-get install -yq --no-install-recommends libxrandr2
apt-get install -yq --no-install-recommends libxrender1
apt-get install -yq --no-install-recommends libxshmfence1
apt-get install -yq --no-install-recommends libxss1
apt-get install -yq --no-install-recommends libxv1
apt-get install -yq --no-install-recommends libxvidcore4
apt-get install -yq --no-install-recommends libxxf86vm1
apt-get install -yq --no-install-recommends libzmq5
apt-get install -yq --no-install-recommends libzvbi-common
apt-get install -yq --no-install-recommends libzvbi0
apt-get install -yq --no-install-recommends x11-common
apt-get install -yq --no-install-recommends alsa-utils
apt-get install -yq --no-install-recommends libbluray-bdj
apt-get install -yq --no-install-recommends libfftw3-bin
apt-get install -yq --no-install-recommends libfftw3-dev
apt-get install -yq --no-install-recommends libportaudio2
apt-get install -yq --no-install-recommends opus-tools
apt-get install -yq --no-install-recommends frei0r-plugins-dev
apt-get install -yq --no-install-recommends tcl
apt-get install -yq --no-install-recommends pulseaudio
apt-get install -yq --no-install-recommends librsvg2-bin
apt-get install -yq --no-install-recommends lm-sensors
apt-get install -yq --no-install-recommends sndiod
apt-get install -yq --no-install-recommends speex
apt-get install -yq --no-install-recommends libvdpau-va-gl1
apt-get install -yq --no-install-recommends ladspa-sdk
apt-get install -yq --no-install-recommends libsoxr-dev
apt-get install -yq --no-install-recommends libspeex-dev
apt-get install -yq --no-install-recommends python-dev
apt-get install -yq --no-install-recommends python-pip
apt-get install -yq --no-install-recommends python-tk
apt-get install -yq --no-install-recommends libssl-dev
apt-get install -yq --no-install-recommends libx264-dev
apt-get install -yq --no-install-recommends libx265-dev
apt-get install -yq --no-install-recommends libnuma-dev
apt-get install -yq --no-install-recommends libvpx-dev
apt-get install -yq --no-install-recommends libfdk-aac-dev
apt-get install -yq --no-install-recommends libmp3lame-dev
apt-get install -yq --no-install-recommends libopus-dev
```
