## Beginner Learning Materials on Reverse Engineering Video Games

A compiled list based on personally recommended learning materials to reverse engineer video games. <br>
Content focuses on Windows x86.


## Recommended order to learn

1. Learn using Cheat Engine
2. Learn hexadecimal, binary, & CPU memory
3. Learn x86 assembly
4. Learn C++
5. Learn using IDA/Ghidra
6. Learn basics of game programming
7. Learn fundamentals of the Win32 API / Windows Internals
8. Practice, the techniques.

## Software needed for reversing

Cheat Engine, and either IDA or Ghidra(open source).

- Memory scanners:
    - [Cheat Engine](https://www.cheatengine.org/)

- Disassemblers / Decompilers / Debuggers:
    - [IDA (freeware edition)](https://www.hex-rays.com/products/ida/support/download_freeware/)
    - [Ghidra](https://ghidra-sre.org/)
    - [x64dbg](https://x64dbg.com)
    - [dnSpy (decompiler, debugger, and editor for C# applications)](https://github.com/0xd4d/dnSpy)

- Process Tools:
    - [ProcessHacker (monitor process and system resources)](https://processhacker.sourceforge.io/)
    - [ProcessMonitor (monitor real-time file system, registry and process/thread activity)](https://docs.microsoft.com/sysinternals/downloads/procmon)
    - [API Monitor (monitor and control API calls)](http://www.rohitab.com/apimonitor)

- PE Tools:
    - [Explorer Suite (PE editor)](https://ntcore.com/?page_id=388)
    - [Detect It Easy (file type and packer identifier)](https://ntinfo.biz/index.html)
    - [TrIDNet (file identifier)](https://mark0.net/soft-tridnet-e.html)

- Network Tools:
    - [Wireshark](https://www.wireshark.org)
    - [mitmproxy](https://mitmproxy.org/)
    - [Fiddler](https://www.telerik.com/fiddler)

- Other:
    - [ReClass.NET (reverse-engineering data structures in memory)](https://github.com/ReClassNET/ReClass.NET)
    
## Picking the right tools

Before getting to work on a game you must know your target, so it's important to gather some information such as:
- What software technologies it uses
- What programming language and compiler it had been developed with
- Does it have any anti-reversing technology in place
- What engine is it running?

Similiar engines often use the same tools. For 3rd game engines such as Unreal Engine or Unity there are a lot of custom tools online that can ease the process of reverse engineering.

Games coded with interpreted programming languages such as C# or Java are much easier to reverse engineer as compared to C/C++, due to the metadata not being lost as they aren't compiled into low-level machine code.

For Unity-based games (and for any other games developed with the .Net Framework) use dnSpy instead of IDA/Ghidra.

Focus on reversing games coded in C++ as it's still the gold standard. (Tech Tax, no company can escape the C curse)

- Examples of games made with C++:
    - Counter-Strike
    - Grand Theft Auto V
    - Fortnite
    - World of Warcraft
    - Fallout 4
    - Destiny 2

- Examples of games made with C#:
    - Genshin Impact
    - Beat Saber
    - Rust
    - RimWorld
    - Hollow Knight
    - Cuphead

## Must-read beginner level materials

- Guides to game reversing:
    - [Game Hacking Academy](https://gamehacking.academy/)
    - [From coding to hacking: An introduction guide to practical (external) game hacking](https://www.unknowncheats.me/forum/programming-for-beginners/267073-coding-hacking-introduction-guide-practical-external-game-hacking.html)

- Intros to x86 assembly:
    - [What Is Assembly Language? - javidx9](https://www.youtube.com/watch?v=1FXhjErUz58)
    - [A Crash Course in x86 Assembly for Reverse Engineers - SensePost](https://sensepost.com/blogstatic/2014/01/SensePost_crash_course_in_x86_assembly-.pdf)

- Basic game programming concepts:
    - [Game Programming Algorithms and Techniques - Sanjay Madhav](https://www.informit.com/articles/article.aspx?p=2167437&seqNum=2) (This article has 7 pages in total, read up to page 5-6)

- Books:
    - [Practical Malware Analysis: The Hands-On Guide to Dissecting Malicious Software - Michael Sikorski and Andrew Honig](https://www.amazon.com/Practical-Malware-Analysis-Hands-Dissecting/dp/1593272901)   

## Must-watch youtube channels

- [Stephen Chapman's YouTube channel for Cheat Engine tutorials](https://www.youtube.com/c/StephenChapman/videos)

## Other really useful materials

- More x86 assembly learning material:
    - [x86 Assembly Language Applicable To Reverse Engineering: The Basics – Part 1](https://resources.infosecinstitute.com/x86-assembly-language-applicable-to-reverse-engineering-the-basics-part-1/)
    - [X86 Assembly Language, Part 2](https://resources.infosecinstitute.com/x86-assembly-language-part-2/)
    - Lena151 Assembly Tutorials (might be outdated, but it is still recommended a lot):
        - [LearnThenTeach YouTube channel](https://www.youtube.com/channel/UCVf5kcdOr535bta-XIdeb4Q/videos)
        - [Tuts 4 You - Collection 2011](https://forum.tuts4you.com/files/file/1865-tuts-4-you-collection-2011/)

- Other useful tools and tool guides:
    - [9 Best Reverse Engineering Tools for 2021](https://www.apriorit.com/dev-blog/366-software-reverse-engineering-tools)
    - [Steamless](https://github.com/atom0s/Steamless)
    - [RenderDoc](https://github.com/baldurk/renderdoc)

- Practical reverse engineering and game hacking materials:
    - [Reverse Engineering/Game Patching Tutorial: Full Res Roller Coaster Tycoon with Ghidra+x64dbg+Python](https://www.youtube.com/watch?v=cwBoUuy4nGc)
    - [Reverse Engineering and Weaponizing XP Solitaire (Mini-Course)](https://www.youtube.com/watch?v=ZmPArvsSii4)
    - [DOOM95 | Making an aimbot](https://web.archive.org/web/20200317042324/https://0x00sec.org/t/doom95-making-an-aimbot/19862)
    - [Game Hacking: Hack, Slash, Loot](https://0x00sec.org/t/game-hacking-hack-slash-loot/3711)
    - [User Mode Rootkits: IAT and Inline Hooking](https://0x00sec.org/t/user-mode-rootkits-iat-and-inline-hooking/1108)
    - [x86 API Hooking Demystified](http://jbremer.org/x86-api-hooking-demystified/)
    - [[C/C++] Reverse Engineering Tutorial for newbies](http://rohitab.com/discuss/topic/35537-cc-reverse-engineering-tutorial-for-newbies/)
    - [Reverse Engineering and Function Calling by Address](https://www.codeproject.com/Articles/29527/Reverse-Engineering-and-Function-Calling-by-Addres)
    - [Reverse Engineering Online Games - Dragomon Hunter](https://0xbaadf00dsec.blogspot.com/2016/01/reverse-engineering-online-games.html)
    - [[Tutorial] Packet Hacking and Reversing MMO](https://progamercity.net/ghack-tut/137-tutorial-packet-hacking-reversing-mmo.html)
    - [Run-time directx hooking using code injection and vtable](http://www.rohitab.com/discuss/topic/34411-run-time-directx-hooking-using-code-injection-and-vtable/)
    - [How to implement pattern-scanning to obtain offsets dynamically](https://www.unknowncheats.me/forum/general-programming-and-reversing/133228-implement-pattern-scanning-obtain-offsets-dynamically.html)
    - [C++:How to patch Bytes using PatternScan (AOB) + Explanation / Snippet](https://www.unknowncheats.me/wiki/C%2B%2B:How_to_patch_Bytes_using_PatternScan_(AOB)_%2B_Explanation_/_Snippet)

- Bit flags and bit masks:
    - [Bit manipulation with bitwise operators and bit masks](https://www.learncpp.com/cpp-tutorial/bit-manipulation-with-bitwise-operators-and-bit-masks/)

- Books and papers:
    - Reversing and game hacking:
        - [Practical Video Game Bots: Automating Game Processes using C++, Python, and AutoIt - Ilya Shpigor](https://www.amazon.com/Practical-Video-Game-Bots-Automating/dp/1484237358)
        - [X86 Disassembly - Wikibooks.org](https://upload.wikimedia.org/wikipedia/commons/5/53/X86_Disassembly.pdf)
        - [Learning Malware Analysis: Explore the concepts, tools, and techniques to analyze and investigate Windows malware - Monnappa K A](https://www.amazon.com/Learning-Malware-Analysis-techniques-investigate/dp/1788392507)
    - Game programming:
        - [Game Programming Patterns - Robert Nystrom](https://gameprogrammingpatterns.com/contents.html) below average book and outdated
    - Windows and Win32 API programming:
        - [Programming Windows: The Definitive Guide To The Win32 Api - Charles Petzold](https://www.amazon.com/Programming-Windows-Definitive-Guide-Win32/dp/9350041057) This literally teaches Windows98 API DELETE
        - [Windows Kernel Programming - Pavel Yosifovich](https://www.amazon.com/Windows-Kernel-Programming-Pavel-Yosifovich/dp/1977593372) (Effective book, not many on this subject)
        - [Windows Internals - Pavel Yosifovich, Alex Ionescu, Mark E. Russinovich, David A. Solomon](https://www.amazon.com/Windows-Internals-Part-architecture-management/dp/0735684189) 
    - Bypassing anti-debugging, anti-reversing, and anti-tamper techniques:
        - [The Ultimate Anti-Reversing Reference - Peter Ferrie](https://anti-reversing.com/Downloads/Anti-Reversing/The_Ultimate_Anti-Reversing_Reference.pdf)

- Curated lists of tools, tutorials, resources, and much more for reverse engineering video games:
    - [UnKnoWnCheaTs Game Hacking Wiki](https://www.unknowncheats.me/wiki/UnKnoWnCheaTs_Game_Hacking_Wiki)
    - [The Ultimate Online Game Hacking Resource](https://github.com/dsasmblr/hacking-online-games)
    - [A Study Path for Game Programmer](https://miloyip.github.io/game-programmer/game-programmer.pdf)

## Useful sites along the way

- [Official Microsoft documentation](https://docs.microsoft.com/en-us/) (includes documentations on MSVC, DirectX, Win32 API, etc.)
- [Godbolt](https://godbolt.org/) (Extremely useful to verify compiler generated C++ code)

## Keywords you want to learn about in general

- Memory scanning
- Memory editing
- Process debugging
- API hooking
- Dll injection
- Threads
- Windows PE format
- Win32 API
- Windows internals
- Software unpacking
