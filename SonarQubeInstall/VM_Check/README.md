# 申請規格如下

* 作業系統：Ubuntu 16.04 LTS
* 記憶體：8G
* 處理器數量(預設4core)：4
* 硬碟:
  * system : 100 GB
  * data   : 300 GB

---

## Check OS

### command line : cat /etc/*release

``` txt
> server@MeSonar:~$ cat /etc/*release
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=16.04
DISTRIB_CODENAME=xenial
DISTRIB_DESCRIPTION="Ubuntu 16.04.4 LTS"
NAME="Ubuntu"
VERSION="16.04.4 LTS (Xenial Xerus)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 16.04.4 LTS"
VERSION_ID="16.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
VERSION_CODENAME=xenial
UBUNTU_CODENAME=xenial
```

---

## Check cpu

### command line : sudo lshw -C cpu

``` txt
server@MeSonar:~$ sudo lshw -C cpu
[sudo] password for server: 
  *-cpu:0                 
       description: CPU
       product: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       vendor: Intel Corp.
       physical id: 4
       bus info: cpu@0
       version: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       slot: CPU socket #0
       size: 2400MHz
       capacity: 4230MHz
       width: 64 bits
       capabilities: fpu fpu_exception wp vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp x86-64 constant_tsc arch_perfmon pebs bts nopl xtopology tsc_reliable nonstop_tsc eagerfpu pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm abm invpcid_single spec_ctrl retpoline kaiser fsgsbase tsc_adjust bmi1 avx2 smep bmi2 invpcid xsaveopt arat
  *-cpu:1
       description: CPU
       product: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       vendor: Intel Corp.
       physical id: 5
       bus info: cpu@1
       version: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       slot: CPU socket #1
       size: 2400MHz
       capacity: 4230MHz
       width: 64 bits
       capabilities: fpu fpu_exception wp vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp x86-64 constant_tsc arch_perfmon pebs bts nopl xtopology tsc_reliable nonstop_tsc eagerfpu pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm abm invpcid_single spec_ctrl retpoline kaiser fsgsbase tsc_adjust bmi1 avx2 smep bmi2 invpcid xsaveopt arat
  *-cpu:2
       description: CPU
       vendor: GenuineIntel
       physical id: 6
       bus info: cpu@2
       version: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       slot: CPU socket #2
       size: 2400MHz
       capacity: 4230MHz
  *-cpu:3
       description: CPU
       vendor: GenuineIntel
       physical id: 7
       bus info: cpu@3
       version: Intel(R) Xeon(R) CPU E5-2630 v3 @ 2.40GHz
       slot: CPU socket #3
       size: 2400MHz
       capacity: 4230MHz
  *-cpu:4 DISABLED
       description: CPU [empty]
       vendor: 000000000000
       physical id: 8
       version: Unknown Processor
       slot: CPU socket #4
  *-cpu:5 DISABLED
       description: CPU [empty]
       vendor: 000000000000
       physical id: 9
       version: Unknown Processor
       slot: CPU socket #5

   ...
   ... 以下都是 DISABLED

```

---

## Check memory

### command line : cat /proc/meminfo

``` txt
server@MeSonar:~$ cat /proc/meminfo
MemTotal:        8174928 kB
MemFree:         3910364 kB
MemAvailable:    5750536 kB
Buffers:          335508 kB
Cached:          1635148 kB
SwapCached:          232 kB
Active:          2655556 kB
Inactive:        1190316 kB
Active(anon):    1277992 kB
Inactive(anon):   660388 kB
Active(file):    1377564 kB
Inactive(file):   529928 kB
Unevictable:        3652 kB
Mlocked:            3652 kB
SwapTotal:        999420 kB
SwapFree:         998920 kB
Dirty:                76 kB
Writeback:             0 kB
AnonPages:       1878684 kB
Mapped:           152780 kB
Shmem:             60748 kB
Slab:             315648 kB
SReclaimable:     238652 kB
SUnreclaim:        76996 kB
KernelStack:       10496 kB
PageTables:        10684 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     5086884 kB
Committed_AS:    4295072 kB
VmallocTotal:   34359738367 kB
VmallocUsed:           0 kB
VmallocChunk:          0 kB
HardwareCorrupted:     0 kB
AnonHugePages:   1527808 kB
CmaTotal:              0 kB
CmaFree:               0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
DirectMap4k:     1236928 kB
DirectMap2M:     7151616 kB
DirectMap1G:     2097152 kB
```

---

## Check Hard Drive:

### command line : df -h

``` txt
    server@MeSonar:~$ df -h
    Filesystem                   Size  Used Avail Use% Mounted on
    udev                         3.9G  4.0K  3.9G   1% /dev
    tmpfs                        799M   66M  733M   9% /run
    /dev/mapper/ubuntu--vg-root   97G  3.3G   90G   4% /
    tmpfs                        3.9G  1.9M  3.9G   1% /dev/shm
    tmpfs                        5.0M     0  5.0M   0% /run/lock
    tmpfs                        3.9G     0  3.9G   0% /sys/fs/cgroup
    /dev/sdb1                    296G  131M  281G   1% /data
    /dev/sda1                    472M   58M  390M  13% /boot
    tmpfs                        799M     0  799M   0% /run/user/0
    tmpfs                        799M     0  799M   0% /run/user/1000
```

---

## 綜合上述檢查與規格無誤