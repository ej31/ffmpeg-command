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
