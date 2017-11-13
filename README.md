# AFL Fuzzing (djpeg)
## Install AFL
```bash
git clone https://github.com/mirrorer/afl
cd afl
make && sudo make install
```
## Run
```bash
./run_djpeg
```
+ `tests` folder contains seed test cases
+ `results` folder contains fuzzing output
## Troubleshoot
Execution Permission Error:
```bash
chmod +x run_djpeg
```
**"Pipe at the beginning of 'core_pattern'"** Error
```bash
sudo bash
echo core > /proc/sys/kernel/core_pattern
exit
```