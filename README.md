# Shazam

A demo project that use Shazam algorithm to generate voice fingerprint and recognize voice.

<br/>

# How to install

Build from source:

```shell
cmake .

make
```

After which, will generate binary executable file `shazam_demo`.

<br/>

# How to use

Use `shazam_demo` to recognize the voice.

Here i provided some demo voices under `data/`.

The `shazam_demo` will read all voices under `data/`, then check the voice with given sound.

Example:

```shell
./shazam_demo ./data/sample-9s.wav
Audio Processing
shazam audio hash
running... 
Generating hashes for original files.. 
reading data/sample-9s.wav 
1:825 hashes for data/sample-9s.wav
Time taken: 0 seconds 16 milliseconds
reading data/sample-3s.wav 
2:275 hashes for data/sample-3s.wav
Time taken: 0 seconds 4 milliseconds
reading data/sample-15s.wav 
3:1651 hashes for data/sample-15s.wav
Time taken: 0 seconds 25 milliseconds
reading data/sample-12s.wav 
4:1100 hashes for data/sample-12s.wav
Time taken: 0 seconds 16 milliseconds
reading data/sample-6s.wav 
5:550 hashes for data/sample-6s.wav
Time taken: 0 seconds 8 milliseconds
Generating hashes for recorded file.. 
reading ./data/sample-9s.wav 
Calculating score.. 
Score for sample-9s.wav = 1.000000
Score for sample-3s.wav = 0.000000
Score for sample-15s.wav = 0.005451
Score for sample-12s.wav = 0.006364
Score for sample-6s.wav = 0.000000
Best Score: sample-9s.wav
Total time taken: 0 seconds 107 milliseconds
```

Here we can see that, `sample-9s.wav` is totally the same voice with our given voice!

<br/>

# Appendix

Reference:

- https://www.cnblogs.com/cpuimage/p/9439493.html
- https://willdrevo.com/fingerprinting-and-audio-recognition-with-python/
- https://www.bilibili.com/read/cv1904784/
