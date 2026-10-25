<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=230&color=0:050b0a,45:063b2b,100:00ff99&text=GABRIEL%20GAMA&fontColor=ddfff0&fontSize=55&fontAlignY=38&desc=I%20ARGUE%20WITH%20OLD%20GPUS%20FOR%20FUN&descAlignY=60&descSize=16&animation=fadeIn" alt="Gabriel Gama — GPU reverse engineering, Linux, Mesa" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=3200&pause=900&color=00FF99&center=true&vCenter=true&width=750&lines=I+reverse+engineer+GPUs+for+fun;My+test+machine+has+1GB+of+RAM;The+datasheet+is+missing.+Of+course.;One+more+register+and+I+can+sleep;ENOTSUP+is+not+a+personality+trait" alt="Animated terminal-style introduction" />

<br />

<a href="https://github.com/gabrieelgama"><img src="https://img.shields.io/badge/GitHub-gabrieelgama-0b1411?style=for-the-badge&logo=github&logoColor=00ff99" alt="GitHub profile" /></a>
<img src="https://img.shields.io/badge/FOCUS-GPU%20DRIVERS-0b1411?style=for-the-badge&labelColor=063b2b&color=00a86b" alt="Focus: GPU drivers" />
<img src="https://img.shields.io/badge/LOCATION-BRAZIL-0b1411?style=for-the-badge&labelColor=063b2b&color=00a86b" alt="Brazil" />

</div>

```console
$ whoami
gabriel

$ cat /proc/hobbies
gpu drivers, disassemblers, Linux, making questionable hardware decisions

$ uptime
not enough sleep to explain the PDS🤤
```

## `01 / HI, I'M GABRIEL` 

I'm Gabriel, from Brazil. I write low-level software, reverse engineer PowerVR GPUs, and spend an unreasonable amount of time staring at hexadecimal numbers. (yes)

Most people see an old laptop and think *"ewaste"*. I see a GPU with undocumented instructions and think *"well, there goes my weekend"*.

I'm currently building open-source graphics drivers around **Mesa/Gallium3D**, poking at **Linux DRM**, and trying to convince hardware from the 2000s to draw triangles without having a nervous breakdown. The hardware, I mean. Mostly.

> My debugging strategy is 10% documentation, 30% experiments, and 60% wondering why changing one bit fixed everything.

## `02 / FEATURED PROJECTS`

<table>
<tr>
<td width="50%" valign="top">

### [SGX535-reMESA](https://github.com/gabrieelgama/SGX535-reMESA)

**Trying to give Intel Poulsbo / PowerVR SGX535 (GMA 500) a second life. Against its will.**

`C` `Mesa` `Gallium3D` `Linux DRM` `USSE` `PDS`

- Reverse engineering SGX535 shader and microprogram behavior
- GPU memory management, command submission and synchronization
- **Verified physical GPU execution** of OpenGL-originated draws
- Verified readback and X11 presentation of GPU-rendered output
- Continuing work on broader rendering and graphics workloads

**Status:** actual GPU pixels have happened. Full compatibility has not. The GPU is negotiating.

[Explore source →](https://github.com/gabrieelgama/SGX535-reMESA)

</td>
<td width="50%" valign="top">

### [SGX544-reMESA](https://github.com/gabrieelgama/SGX544-reMESA)

**Because apparently reverse engineering one PowerVR GPU wasn't enough.**

`x86` `Android` `GLSL` `UniFlex` `USSE` `PDS`

- Investigating PowerVR userspace graphics libraries
- Mapping GLSL compiler interfaces and callbacks
- Researching UniFlex, shader objects and backend behavior
- Documenting findings without redistributing proprietary binaries

**Status:** early research. Currently making friends with stripped binaries. They are not friendly.

[Explore research →](https://github.com/gabrieelgama/SGX544-reMESA)

</td>
</tr>
</table>

## `03 / YES, THE GPU ACTUALLY DID SOMETHING`

```text
SGX535 / PHYSICAL HARDWARE
[PASS] OpenGL-originated draw submitted to SGX535
[PASS] GPU completion / retirement observed
[PASS] Hardware-rendered pixels verified by readback
[PASS] GPU-rendered output published through X11
[PASS] Expanded render targets, shader support, continuous workloads

No, this does not mean every OpenGL game works. I wish.
```

## `04 / THINGS I USE TO CAUSE PROBLEMS`

<div align="center">

<img src="https://skillicons.dev/icons?i=c,python,bash,linux,git,github,cmake,java&theme=dark" alt="C, Python, Bash, Linux, Git, GitHub, CMake and Java" />

<br /><br />

<img src="https://img.shields.io/badge/Mesa%20%2F%20Gallium3D-0b1411?style=flat-square&logoColor=00ff99" alt="Mesa and Gallium3D" />
<img src="https://img.shields.io/badge/PowerVR%20SGX-0b1411?style=flat-square&logoColor=00ff99" alt="PowerVR SGX" />
<img src="https://img.shields.io/badge/Linux%20DRM-0b1411?style=flat-square&logoColor=00ff99" alt="Linux DRM" />
<img src="https://img.shields.io/badge/Ghidra-0b1411?style=flat-square&logoColor=00ff99" alt="Ghidra" />
<img src="https://img.shields.io/badge/GCC%20%2F%20LLVM-0b1411?style=flat-square&logoColor=00ff99" alt="GCC and LLVM" />

</div>

## `05 / THE WORLD'S MOST QUESTIONABLE LAB`

```text
My """"PC""""
│ Samsung Galaxy Tab S7                                      
│ ARM64 / Snapdragon 865+                                      
│ Termux + PRoot + Debian Linux                      
│ Writing code, building toolchains, analyzing blobs

My Device 2
│ Dell Inspiron Mini 12 (1210)                       
│ Intel Atom Z520 / 1 GB RAM                         
│ PowerVR SGX535 / Intel GMA 500                     
│ antiX Linux                                        
│ Real GPU execution, readback, hardware experiments  
```

Yes, I develop the driver on a **Samsung tablet running Linux userspace**, then test it on a **netbook with 1 GB of RAM**. No, the netbook is not my development workstation. It has suffered enough.

Somewhere out there is a perfectly good workstation. I have chosen this instead.

## `06 / SIDE QUESTS (I HAVE A PROBLEM)`

- **Linux `gma500` DRM:** experimental RFC patch work on mapping lifetime, page-table tracking, synchronization and KUnit coverage.
- **Anland:** contributed Brazilian Portuguese localization.
- **ShimeLinux:** Linux desktop mascot work involving Java, Wayland and ARM64.
- **Toolchains:** i386 builds, GCC/LLVM tooling, Ghidra-assisted binary analysis, X11 and Wayland experiments.

## `07 / NUMBERS THAT MAY OR MAY NOT LOAD`

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=gabrieelgama&show_icons=true&hide_border=true&bg_color=050b0a&title_color=00ff99&icon_color=00ff99&text_color=c9e8db" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=gabrieelgama&layout=compact&hide_border=true&bg_color=050b0a&title_color=00ff99&text_color=c9e8db" alt="Top GitHub repository languages" />

<sub>Statistics are generated by a third-party service and may occasionally be unavailable.</sub>

</div>

## `08 / SEND HELP (OR DOCUMENTATION)`

Got an old PowerVR device, SGX documentation, hardware test results, or a mysterious register dump? I would genuinely love to hear about it. Open an issue or discussion in the relevant repo.

Please do not send me another undocumented GPU. I will absolutely start a third project.

**GitHub:** [github.com/gabrieelgama](https://github.com/gabrieelgama)

```asm
; I have seen this number more than some of my relatives.
MOV  EAX, 0x07000345
; Do I understand everything yet? No.
; Am I going to stop? Also no.
```

<div align="center">

**`less ENOTSUP, more pixels, probably less sleep😎😎😎🔥`**

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=105&section=footer&color=0:00ff99,100:050b0a" alt="Green wave footer" />

</div>
